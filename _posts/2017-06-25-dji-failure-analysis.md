---
layout:     post
title:      2016 DJI Dev Challenge Failure Analysis and Lessons Learned
date:       2017-06-25 02:00:00
summary:    I present what went wrong and analyze what could have been done better to prevent future catastrophes
categories: robotics drones
---
In the time after the competition Alex figured out what had gone wrong. On august 26th 2016, just two days before the competition, a commit had gone in to refactor some flight parameters and simplify things. 

<figure>
    <img src="/images/dji_final_commit.png" />
</figure>

Seems like a simple enough change right? Move away from ROS' [dynamic reconfigure](http://wiki.ros.org/dynamic_reconfigure) infrastructure and simply use parameters written in launch files. The dynamic reconfigure
was important for field trials where we were empirically tuning flight parameters and we needed a way of quickly changing things on the fly. Let's go through the changes introduced by this commmit

<figure>
    <img src="/images/dji_commit_change1.png"/>
</figure>

So the first change we can see that the parameters are removed from the parameter generation file and put into the launch file. Some parameters are outright removed and some values are changed but nothing too out of the ordinary. Yaw parameters were removed (but reintroduced farther down) and the `flight_leve_low` was reduced from 3.75m to 3.5m.

<figure>
    <img src="/images/dji_commit_change2.png"/>
</figure>

Next, we had changes in the moving landing node itself. The callback is simplified to remove parameters which are no longer in the `.cfg` file and lines are added to fetch them directly in the parameter server. Can you spot the mistake? To fully grasp the mistake we need a little bit of [background information](http://answers.ros.org/question/28327/dynamic-reconfigure-default-parameters/) on  `dynamic reconfigure`. As Jack O'Quin explains:

>
When you register your [dynamic reconfigre] callback, it gets invoked immediately with the values currently defined in the parameter server and a level of `0xffffffff`. Those initial values will include anything set in your launch file. You don't need to read the parameters yourself using `getParam()`.

If you look at the configure callback of `MovingLanding_node.cpp` you can see that most lines are simple assignment except on line 91 where the landing speed also has a minus sign in front of it. Whereas before this commit, the callback would be immediately called and the parameter would set a negative landing velocity, now the velocity stayed positive. 

Here is the best explanation we can give for what happened at the DJI challenge. The quad approached the truck and as it saw the landing tag it started climbing in altitude due to the positive velocity. Once it got high enough that the AprilTag detection failed, it lowered down back to its `flight_level_low` altitude to search for the tag. Loop and repeat, this was the oscillation we saw instead of the landing.

As for the "air breakdancing" we saw where the quad didn't seem to come back to the truck remains to be explained. My best theory is that somewhere along the way, DJI's data transparent transmission which we used to send IMU and GPS data failed or become intermittent while the quad was far away (lower the quad seemed to have helped with this). As the connection cut off and came back while the truck drove away in a loop, some buffered GPS positions were sent to the quad. As both the current and older positions were sent back, the quad would constantly switch between trying to fly to the current position and flying to a position somewhere on the track.

In summary, **we lost 100 000$ because of a minus sign**.

## Cascading human errors

As I look over the entire challenge, it is clear that this failure wasn't only due to the minus sign. For example, suppose practice day had gone our way, we would have caught this bug on practice day. But practice day would only have succeeded if we hadn't had so much confusion about wifi. Somewhere along the way, we were also the only team
so concerned by having wireless connectivity. Not only for IMU and GPS data for the landing but also to send back survivor detection data.

Furthermore, we *did* detect this failure scenario the night before the competition but we dismissed it by saying the DJI simulator wasn't behaving right. Why would we say that? A combination of being too tired to invest more energy in debugging things with a lack of trust in DJI's tools after some of the headaches they caused.

## Lessons learned

## Preventive measures