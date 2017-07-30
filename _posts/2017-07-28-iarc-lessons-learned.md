---
layout:     post
title:      10 lessons learned from competing at IARC Mission 7
date:       2017-07-28 02:00:0
summary:    Figured, 10 was a nice round number
categories: robotics drones competition
---

I suppose throughout the years I've learned a few lessons as to what to do and what not to do when competing in these large collegiate engineering competitions. This list will hopefully not repeat the [lessons learned from the DJI challenge](/2017-06-25/dji-failure-analysis/).

# 1. At first, don't go off the beaten path

When first starting off and getting into a new field and a new competition, its safer to follow where previous competitors have hone. The problem here is that not only do you know nothing. You don't even know what you don't know. Take things by authority at first until you get a feel for things and improve your understanding of the field.

This is why in 2014, we built a quad using a Pixhawk flight controller, the px4 flight stack, the px4flow for optical flow, a Gumstix Overo board as our computing power, a Caspa FS as a camera and LairdTech RM024 radios for communication. The px4 ecosystem was selected after seeing the [video](https://www.youtube.com/watch?v=0Jpq6DU_HVg) from the pixhawk team showing position control with the old px4fmu and a px4flow. This meant it was the closest thing we could get to a plug and play system. As for the camera and the computing power, I believe it was selected because we had seen it being used in another Pixhawk project but also by Georgia Tech's aerial robotics group at [IARC 2011](http://www.aerialroboticscompetition.org/2011SymposiumPapers/GIT_2011.pdf).

Sure we knew things wouldn't be as simple as copying someone else's setup. But the risk mitigation was definitely worth it compared to going in blind with our gut feeling.

# 2. Be confident

I don't mean confident in a "I know everything way." rather, confident in a "Given enough time, I can figure out some of this." I see it pretty often when people start looking into something and simply give up as soon as they don't understand something or when they don't know what to look for. Even in my lab, some people think I know everything about implementing and developing robotics systems. To be entirely honest, I don't know that much, I'm just extremely stubborn, at times obsessive and I have a lot of free time. But beyond personality traits, I know that if I ask the right questions and who/where to ask them, I can get to where I need to be.

I'm not saying that you can figure out everything. Myself for the longest time I stayed away from attempting to understand Kalman filters. But there is definitely knowledge out there that seems slightly out of reach when in reality, it isn't.

So be confident.

# 3. Plan it out and set goals

I recently came across a video from psychology Professor Dr. Jordan B. Peterson talking about [goal setting](https://www.youtube.com/watch?v=OoA4017M7WU). Rough transcription here:

> Specify your damn goals because how are you going to hit something if you don't know what it is? That isn't going to happen and often people won't specify their goals too because they don't like to specify conditions for failure. So if you keep yourself all vague and foggy; which is real easy because that's just a matter of not doing as well. Then you don't know when you fail.

## 3.1 Resource Allocation

Peterson sums things up pretty well but only looks at the issue from a general and personal point of view. If you look at goal setting from a project management point of view, knowing your goals and your plan to get there leads to correct resource allocation. In other words, goal setting leads to an understanding of task priority which leads to you knowing what to work on and what *not* to work on.  If you want to do C and the dependency chain is A -> B -> C. Don't work on B if you don't even have A yet. This is why I had spent so much time on visual odometry and state estimation. I didn't see the point in working on obstacle avoidance if I couldn't get an accurate measurement of my position and velocity.

Moreover, resource allocation isn't just about putting the right amount of effort in the right places. It's also about knowing when to give up or drop some things when other tasks are of higher priority. In 2015 our goal was to follow a ground robot however we had many hardware problems which had to be addressed to be able to fly. I dropped my efforts on visual odometry to tackle these problems knowing that my team mates would be blocked on their robot tracking if they didn't even have a flyable vehicle.

## 3.2 Project Planning and Expectations

Once you have your goals, you can map our the road to them. The map should not only tell you what has to be done and how to do it, but also what kind of investment it should take. Don't lie to yourself about wanting to do obstacle avoidance if you only have 1 hour per week to give to your project over 3 months.

Setting goals allows you to estimate what kind of investment you're expecting from your team. Can't give that much time to the project? No problem, lower the bar! Can't reach your goal with how much work you're investing in it? Take it as a wake up call to start giving more.

# 4. Don't use planning as an excuse for procrastinating

Yes you need to plan ahead. But there comes a time when you just need to jump in, fall over, get up, trip and fall over again and get back up to really get to where you want to be. Keeping things theoretical all the time and having "design meetings" just leads to paralysis by analysis and, more often than not, work wasted on planning things that never would have worked in the first place.

I believe people spend so much time planning things without acting because they are afraid to be wrong. However, choosing a sub-optimal solution is better than not choosing. You need to get over paralysis by analysis and accept that you're going to make mistakes and that it's part of the learning process.

# 5. Don't underestimate the importance of sponsors and marketing and don't underestimate your ability to raise capital

I remember when first arriving at IARC 2014, a guy from University of Central Florida asked us "Yo guy! How do you have so many sponsors?" Having made a plan and having set our goals, I knew I needed about 20 000 CAD to set up my team. We were starting from scratch and needed even the most basic tools such as screwdrivers, power supplies, a flight cage for safety, a computer, etc... Basic parts such as motors, speed controllers, propellers, wiring, etc... We even had some administrative costs related to starting a non profit organization which would allow us to open a bank account for the team.

Of course, there was no way I would convince my school to give us 20k, they ended up giving us 4k for which we were already extremely grateful. That still left us with a significant amount to raise which we did by compulsively contacting all the companies related to robotics, engineering, hobby parts and more. This allowed us to get important sponsorships such as motors, ESCs and propellers from T-Motor or money from CanadaDrones or a rebate from RobotShop. Hell we even got motors from Scorpion Motors without realizing they were made for RC airplanes.

What I came to realize was that a lot of companies are eager to help out students. Sometimes they have pre-production units they don't mind unloading, the larger companies have an annual budget to allocate to sponsorship advertising and so on. What's clear is that you can't expect to start a team without putting in some financial and marketing work.

# 6. Budget for failure

One of the most tedious beginning of year activities is to plan out your budget for the next competition and for your grant requests. Early on I had the right intuition to budget for possible unexpected expenses and I had portioned 10% of my total budget as "unforseen expenses". But there's a smarter way of going about it.

As you budget for regular things, think about how they might have to be replaced. Need 20$ worth of propellers for one quad? Budget for 3 full crashes and boost that to 80$. Need a replacement onboard computer? Budget for two of them.

You know you're going to make mistakes. Adapt your budget (and your plan) to fit that narrative.

# 7. Logistics are just as important as technological advancement

One of team Elikos' core strengths was adaptability and responsiveness to change, call it "Agile Development" if you want. Sure we cut it close at times but we always made an effort to predict our future needs and possible failures.

Practically speaking this could mean buying a variety of nuts, bolts, spacers, various electronics, LiPo batteries, cameras, lenses, propellers, etc. beforehand so when the time comes where you will need these materials, you won't have to wait for buying and shipping delays. If you've planned your year right, you should be able to predict what kind of materials and equipment you need at the beginning of the year. It could also mean hurrying one project because it's a dependency to another one coming up.



# 8.

# 9. Don't reinvent the wheel

This lesson depends on your actual goals. If your ranking at your competition matters to you,

# 10. Chill out
