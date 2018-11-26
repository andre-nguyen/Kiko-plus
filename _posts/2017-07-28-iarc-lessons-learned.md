---
layout:     post
title:      10 lessons learned from competing at IARC Mission 7
date:       2017-07-28 02:00:0
summary:    Figured, 10 was a nice round number
categories: robotics drones competition
---

I suppose throughout my two years as project director I've learned a few lessons as to what to do and what not to do when competing in these large collegiate engineering competitions. This list will hopefully not repeat the [lessons learned from the DJI challenge](/2017-06-25/dji-failure-analysis/).

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

Once you have your goals, you can map out the road to them. The map should not only tell you what has to be done and how to do it, but also what kind of investment it should take. Don't lie to yourself about wanting to do obstacle avoidance if you only have 1 hour per week to give to your project over 3 months.

Setting goals allows you to estimate what kind of investment you're expecting from your team. Can't give that much time to the project? No problem, lower the bar! Can't reach your goal with how much work you're investing in it? Take it as a wake up call to start giving more.

## 3.3 Fail fast

A while ago, I came across a [Ted talk from Astro Teller](https://www.ted.com/talks/astro_teller_the_unexpected_benefit_of_celebrating_failure), head of [X](x.company) (formerly Google \[X\]) where he talks about how his team works on the most difficult challenges of new projets to see as soon as possible if the said project is viable. In other words, and I'm paraphrasing here, when working on something its almost as if you're looking for a reason to kill off your project. And if you can't find a reason to, then it's a good project.

The ideas Teller expresses in his talk are maybe a bit extreme in the case of student competitions. Instead of all or nothing, you can still half ass your way to winning a competition on points. But the importance of knowing your limits and knowing when to kill a project so you can take back those ressources and allocate them somewhere else is crucial. Killing a project early could free up a person to help another person on a more essential task. Its definitely not an easy task to identify a point where something needs to stop and it's even harder to do it even when you know it has to be done. But the best way to know when to kill a project is to always keep an eye on the big picture and how you can adapt to new situations to get as close to your goals as possible.

# 4. Don't use planning as an excuse for procrastinating

Yes you need to plan ahead. But there comes a time when you just need to jump in, fall over, get up, trip and fall over again and get back up to really get to where you want to be. Keeping things theoretical all the time and having "design meetings" just leads to paralysis by analysis and, more often than not, work wasted on planning things that never would have worked in the first place.

I believe people spend so much time planning things without acting because they are afraid to be wrong. However, choosing a sub-optimal solution is better than not choosing. You need to get over paralysis by analysis and accept that you're going to make mistakes and that it's part of the learning process.

I highly recommend this TED talk by Tom Wujec titled [*Build a Tower, Build a Team*](https://www.ted.com/talks/tom_wujec_build_a_tower). He talks about the marshmellow challenge where small teams have about 20 minutes to build the tallest structure to hold a marshmellow using dry spaghetti and tape. The surprising result is that kindergarteners performe much better than recent business school graduates. He explains that

> the reason is that business students are trained to find the single right plan, right? And then they execute on it. And then what happens is, when they put the marshmallow on the top, they run out of time and what happens? It's a crisis. Sound familiar? Right. What kindergarteners do differently is that they start with the marshmallow, and they build prototypes, successive prototypes, always keeping the marshmallow on top, so they have multiple times to fix when they build prototypes along the way. Designers recognize this type of collaboration as the essence of the iterative process. And with each version, kids get instant feedback about what works and what doesn't work.

Measure twice; cut once? Fuck that. It only works when you know what to measure and how to measure it. Plan for an iterative process, bring out your inner kindergartener and fiddle with things to understand them.

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

In other cases it could mean planning a full scale test day, planning a full systems integration day, planning a touch point, making sure you arrive to the competition a day early to get acclimated to the city, making sure you rent a spot to do your tests if you need it, getting in contact with campus security to clear your flights, getting in contact with competition organizers, etc. There is a lot of support structure you need to provide to your team. In larger student projects logistics lead can be a full job in of itself. 

# 8. Remember that the iterative process includes failure

I've touched on this in the other lessons but it's definitely a lesson in of itself. If you're starting from scratch you'll break things, you'll crash things, you'll work on useless things, you'll work on things that are too hard, you'll work on things when the other things it depends on don't even work, you'll fail.

It's normal. It's only a waste if you don't learn from it. Fail fast, figure out what you've learned and try again.

# 9. Don't reinvent the wheel

This lesson depends on your actual goals. If you're in it more for the learning experience, your ranking doesn't matter to you and you have a love for reimplementing existing things to fully understand all their intricacies, then by all means, build your own autopilot, your own air frame and so on. To my understanding, this is what University of Michigan has been doing since 2014. On the other hand, if you're in the competition to actually compete, then don't reinvent the wheel. People far smarter than you and I have been working on MAVs and their related algorithms for far longer than us and with access to much bette ressources.

Is there a point to reimplementing your own position controller like UofM? Is there a point to writing your own optical flow algorithm like Embry-Riddle? Is there a point to making a new kind of aerial vehicle like Pima Community College? Not reinventing the wheel gives you time to work on things that truly matter. 

The lesson here is obvious and mostly common sense. However it often gets lost in enthusiasm for the technology. Yes making your own attitude controller or your own state estimator would be an amazing advancement to your learning and it would certainly be an outstanding achievement. But you have to be honest here, are you doing it because you love the idea of doing things yourself or are you doing it because you truly have something to gain to get to your goals? Both answers can be correct. But they are only so if they align with your team's goals.

# 10. Test test test

Don't stay stuck in simulations and theory all the time. Simulating your quad and your algorithms on datasets can only get you so far. It will never be the same as the experience you acquire by having two or three team members actually flying your vehicle around. All the hardware issues and parameter tuning can take ages and if you don't budget at least a good 1-2 months of flight tests before your competition, you're at high risk of showing up and not even flying.

# 11. Bonus lesson: Chill Out

This is a lesson I wish I had truly understood while I was director of Elikos. People are going to be dishonest with you to save face. It's tough to admit that you've failed or that you didn't end up doing what you said you were going to do. More often than not, it's simply a question of them not putting the same importance to the project as you do. At the time, I found it pretty infuriating that some of the core aspects of the project were not moving forward, putting the entire thing in jeopardy. In the first year it was not even having an air frame 3 months before the competition. The second year it was how all the electrical systems were non functional and were actually destroying equipment. But deep down it stemmed a lot from having honesty as a core value and a deep disdain for people blowing smoke. I *hated* when people would come up to me, act like the thing I was asking for was super easy or worse suggest we do things completely out of our reach and then ended up never delivering anything at all.

*Side note* : I specifically remember at IARC 2015 that one of the organizers talked about how on flight day you'd be able to distinguish between who can really fly and who's just blowing smoke. I guess the organizers were also tired of people saying they were fully autonomous in their presentation and then showing up with nothing the next day.

The lesson here is that sometimes you might just have to accept failure and that it might not be your fault. Its tough as project lead because you'll be the one who's going to have some explaining to do. But this kind of thing happens all the time, especially in student projects.

Maybe I should have chilled out while I was director. Then again, my non-acceptance of failure brought us to two wins and multiple honors.

***Lesson update 26-11-2018*** : A year after writing this post, it has come to my attention now that team Elikos went way downhill ever since I left. In 2016 though they finished first in North America, they had technologically regressed to Elikos 2014 and were only capable of performing autonomous take off. By 2017 they weren't even able to take off on competition day and by 2018 they didn't bother showing up to the competition. It is truly a sad sight to see and goes to show how I was never in tune with the rest of my team. None of the lessons I learned above have been passed down, no one valued the same things I did and now what's left is but a shadow of its former self.
