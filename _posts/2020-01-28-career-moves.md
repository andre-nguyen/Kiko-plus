---
layout:     post
date:       2020-jan-28 00:00:00
title:      M.A.Sc. to now
summary:    Finished my master's degree and wondered where to go from there <figure><img src="/images/career_moves/applanix.jpg"/></figure>
---

## Looking back on that master's degree

On December 21st 2017 I defended my Master's thesis in front of a jury composed of
[Liam Paull](http://liampaull.ca/), newly arrived at University of Montreal at the time, 
[Richard Gourdeau](https://www.polymtl.ca/expertises/en/gourdeau-richard) and my thesis 
advisors [David Saussié](https://www.polymtl.ca/expertises/en/saussie-david) and 
[Jérôme Le Ny](http://www.professeurs.polymtl.ca/jerome.le-ny/index.html). I was
stressed out of my mind and had practiced the presentation every day during the two weeks leading up to it. 

<blockquote class="twitter-tweet tw-align-center"><p lang="en" dir="ltr">Great talk by Andre Phu-Van Nguyen today for his successful MS thesis defense. Congrats Andre and thanks for the great work in the lab these last two years! <a href="https://t.co/CMn48jLaLd">pic.twitter.com/CMn48jLaLd</a></p>&mdash; Jerome Le Ny (@jleny) <a href="https://twitter.com/jleny/status/944034567039660032?ref_src=twsrc%5Etfw">December 22, 2017</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

The entirety of my graduate studies, starting in 2015, had been a rocky road and I was close to quitting more than once. I was way out of my element, with almost all of my
classes requiring mathematical rigor I had not properly developed during my
undergraduate degree in Computer Engineering. To say that things weren't going well
both personally and academically would be an understatement. My girlfriend at the time
had broken up with me (explosively at that), I had failed a class, which automatically
disqualified me from my graduate program and I my real research project still hadn't
started which meant I was more than a year into the program without being paid.

I decided that it was best to just accept
that I'm a software engineer who doesn't have what it takes to become a roboticist.
I gathered what was left of my courage and went to see my thesis advisor to announce
my resignation; man of my word, I would quit only after finishing the implementation
of a [robot path planning project](https://doi.org/10.1109/TASE.2017.2762088) he had given me.

As I sat there trying to explain why I was quitting, he glances at his screen and gasps.
Our grant request was accepted, my research project would be starting and I would
be getting paid shortly. I was now contractually bound to this research project for
which half the cost had been paid by a drone company.

<figure style="">
  <img src="/images/career_moves/geralt.jpg" />
  <figcaption>If you haven't seen The Witcher on Netflix, at least watch
  this <a href="https://www.youtube.com/watch?v=2BSrsUR5ph4">supercut</a> of 
  Geralt of Rivia saying fuck to understand how I felt at the time.</figcaption>
</figure>


To be entirely honest, I had no idea what the legal consequences of quitting were, if any.
I just knew I was committed to something and it would be in bad taste to break those commitments. I was barely hanging on but with the help of friends and my advisors,
I kept pushing, put my name on those publications, passed the rest of my classes,
delivered on that research project and wrote my thesis in about 2 months, judging from
the commit logs.

<figure>
  <img src="/images/career_moves/thesis_commit.jpg" />
  <figcaption>True story</figcaption>
</figure>

Flashforward to December 22nd 2017, the jury awarded me my thesis with minor corrections,
a huge weight was lifted off my shoulders. *Never again*, I thought to myself.
I played video games all day for the first time in 9 years. I got bored. 


## A little break

I decided to
pull the trigger on an idea I had had for a while to go on an extended trip in Asia. With
about two weeks notice and a lot of googling, off I went.
What was supposed to last about a month and a half got extended to almost three months.
In that time I went through Thailand, Vietnam, Cambodia, Indonesia and a bit of Australia.
I was at a point where I was tired of the beach and I had topped out on how much more tan
I could get.

<div style="display: flex;">
  <figure style="width: 50%;">
    <img src="/images/career_moves/vacation_small.jpg" />
    <figcaption>Look at this guy having a grand ol' time</figcaption>
  </figure>
  <figure style="width: 50%">
    <img src="/images/career_moves/diploma_small.jpg" />
    <figcaption>Back in Canada, tan, diploma in hand and 
    ready to start my career</figcaption>
  </figure>
</div>

I came back to Canada but I was still mentally fatigued and not quite ready to get a job.
I must of spent the next two months doing nothing other than going to the gym or going out
with friends as well as "studying" for a potential interview which would require solving
programming questions. And by studying I mean I went through only two chapters of *Cracking
the Coding Interview*. 

## First Job First Mistake

I remember I sent out a total of three resumes one to DJI
for a senior roboticist position, one to Auterion and one to a local drone startup. I got through the three rounds of interviews with [Auterion](https://auterion.com) only to be told
that it would be very difficult for them to hire internationally (?!). Clearly, I hadn't
put that much effort into finding my dream job. I was extremely picky about my opportunities,
the drone world is rife with bullshit, people who don't understand drones nor robotics.

I ended up accepting the job at the local drone company. The leadership was composed of engineers who understood drones, at least, more so that some unnamed startups out there. I was upfront about that aspect of what I was looking for in a job. "I don't want to work for someone who doesn't understand what I'm doing". Clear as can be and it was clear to me that my interviewer did understand. I was then sold on the idea that I would
be building a SLAM system for GPS denied navigation of drones. *Right up my alley*, all these
engineering competitions and my thesis have prepared me for this. I start on my first day
and I see a Gazebo simulation (not based on RotorS) of a quadrotor which integrates the
autopilot firmware and some basic LIDAR sensors. *Amazing. All these academic tools but now
I'm paid to use them*. It was explained to me that one of my main tasks would be to bring to
life a SLAM system which was written in Matlab by a student doing a research project with the
company. While this student was finishing his degree, he would also start working at the
company to continue his research. *Neat, I'll be on the bleeding edge too*.

And it all went downhill from there.

Things quickly devolved into me spending all my time teaching basic programming skills
and C++ syntax someone could simply Google. When I suggested my colleague take a programming class
or at least follow some online tutorials, he refused saying he was better at learning hands on. *Fair enough*. But when asked to do something he would simply reply, "I don't know how to do that". That's kind of the point isn't it? You figure it out by getting hands on and you learn.

While I had joined the company as a "Robotics Perception and SLAM Expert", my role was
diminished to being the programming assistant of someone with less hands-on, robotics, drones
and software experience than I. Nonetheless, I stuck around thinking things would get better
but eventually I started being more vocal about my complaints. 

### Bad Agile Methodology

While I had to teach programming I was also in charge of project planning, goal setting,
building our sprints in Jira and to be entirely honest, I don't think I'm qualified
to be an Agile Coach. What little I know about Agile is the brief overview they give in
school and the various blog posts you find online. However, reading through some parts of
the Agile Manifesto, I couldn't help but think this had nothing to do with us. 

> "Our highest priority is to satisfy the customer through early and continuous delivery of valuable software."

We didn't even have a customer, market research, nor did we even know what customers we 
were targeting. I would spend enormous amounts of time planning things in Jira instead of
simply going ahead and writing software. More often than not, the time estimates I would enter
would almost be bogus, especially with anything related to pure research. *Should I really time box my
literature review and stop it after only two days?* How do you know there isn't four days
worth of literature out there for the system I am trying to build? It seemed like we had managed to
combine the worst of two worlds, a small company with low resources with the bureaucracy of a large company.

We would have a daily company wide scrum (around 10 people) where some employees would literally have full conversations trying to problem solve instead of sticking to the basics. After a while I
noticed that no one was actually listening when anyone from the SLAM team spoke. Sometimes
my colleague would say something surprising and no one would react. I came to the conclusion
that the entire company didn't even understand SLAM or anything related to robotics for that matter.

There came a time when I simply asked what the project requirements are and the CEO bounced the
question back at me. It was management's way of acting like they trusted you with the
technological decision but once you made the decision you would invariably be overridden.
So much for the "freedom" and "responsibility" that comes with working in a small company.
I replied with another question: *Who's the product owner and who's the product manager here?* I asked the question, not because I didn't want to set the requirements, but because
the previous times I had tried, I would either waste time arguing with my colleague about who
was right when he hadn't even bothered researching our competition or my decision would be 
overridden.

My question was met with silence on the Slack channel. It turns out management had an
emergency meeting to clarify what everyone's role was. 

>"Let's forget Agile methodology roles because not everyone is familiar with them." 

My blood was boiling. They created a new organizational chart showing everyone's role. Somehow a two person project had 7 stakeholders. The CEO would represent client interests, the COO would make sure we filled
our sprints and followed agile-ish methods. The CTO would make the final calls on the
technological decisions. The day to day scrums would be supervised by a "senior" software
developer who had no background in robotics. I would be both a SLAM developer and
a system integrator because I had a lot of hands on experience on robotics. My colleague
would be a SLAM developer, in essence bringing his master's thesis to real life.

Thus, the only management person who could understand what we were doing (the CTO) would
only have a distant role in the project. *Great.*

### Getting Your Ideas Shutdown

As mentioned previously, when I joined the company they had started building a drone
simulator in Gazebo with some lidars. The drone ran a stripped down version of the
autopilot firmware in a software-in-the-loop fashion. It wasn't quite complete as the model
wasn't actuated by the firmware, but the state estimation was running using the simulated
input which was good enough. Now one of the questions that came up was, what the end goal of
the project was. The decision was taken to use lidar to also create 3D models of the environment,
thus the product would then be both for GPS denied state estimation and surveying 
In fact, shortly thereafter, it was was decided that the product would be entirely separated from
the company's main product, a drone autopilot, but we were sill targetting a drone mounted payload.

Now something didn't quite add up for me. To be able to do proper lidar based SLAM with the method
being developped, it would require use to have the sensor placed horizontally. This would allow us to get the most scene coverage and thus, the best chance at proper point cloud alignment. The problem however is that
there would eventually be places in the map left unscanned (parts of the ceiling for example) because it
would be difficult given a quadrotor's dynamics to point the sensor every where you need to create complete
scene models. Traditional aerial scanners work in a pushbroom manner where a 2D lidar facing downwards is
flown over an area with possibly overlapping passes for surface coverage. In an indoor scenario, this wouldn't
be possible. 

As of writing, to the best of my knowledge there are two main companies focused on lidar based
GPS denied navigation for micro-aerial vehicles with model reconstruction: [Exyn](https://www.exyn.com/) founded by renown University of Pennsylvania professor
Vijay Kumar and [Emesent](https://www.emesent.io/), a spinoff of Australia's CSIRO, both of whom decided to
adress the problem by mounting the lidar on an actuator to make it spin continuously. Other players include
GeoSLAM, who's beginnings trace back to technology licensed from CSIRO, developping mainly handheld scanners
(also rotating) and [Inkonova](https://www.inkonova.se/) which also claims to be using a rotating 3D lidar but information is sparse on their product.

<div style="display: flex;">
  <figure style="width: 33%;">
    <img src="/images/career_moves/exyn.jpg" />
    <figcaption>Exyn's scanner mounted on a DJI m200</figcaption>
  </figure>
  <figure style="width: 33%">
    <img src="/images/career_moves/emesent.png" />
    <figcaption>Emesent's Hovermap payload, drone is optional</figcaption>
  </figure>
  <figure style="width: 33%">
    <img src="/images/career_moves/geoslam.png" />
    <figcaption>GeoSLAM's handheld ZEB HORIZON</figcaption>
  </figure>
</div>

At the time I was still pseudo-in charge of project planning and I decided that down the line we would start
working on a spinning lidar. I was immediately shut down by the CEO and told to replan the next 9 months.
Making the lidar spin was a stupid idea and we had never planned this.
I can't say exactly what I was told after but it wasn't pretty. A colleague of mine mentioned that our CEO only
acts that way when he's mad but really our CTO gets away with not planning things all the time, hence there
was no need for me to actually replan anything. *He was right.*

I was concerned that
no one had a better idea to tackle sensor coverage and if we ever decided to make our lidar spin, our algorithm
wouldn't be able to cope with the dynamics, making us waste another year redevelopping everything from scratch. 
I continued to voice my opinion and the responses were still mostly dismissal.
*"We'll cross that bridge when we get there."*,
*"Maybe we can make it spin later and create a new SLAM algorithm when we do."* or my favorite response
from my fellow SLAM teammate *"We can put two Velodyne pucks on a drone, one to do the state estimation and one to do scanning in a pushbroom fashion."* **Cue Geralt saying "fuck"**. The one guy who can do the 
SLAM math doesn't know anything about drones and wants to add 1.2kg of lasers to an indoor drone in addition
to the wiring, mounting hardware and onboard computer.

A few weeks later, the CTO would go to a mining conference in Montreal where he got to see both Exyn and
Emesent. He came back saying that making a 3D lidar spin made sense and we should look into it. At that point
I just felt insulted. Not only was it a lie that I could have a role to play in the decision making, my ideas
were only of value if they were the same as the ones from someone in management.

## Moving on

I could go on and on with the problems I faced but I'm already tired of writing this post. To summarize in point form:

* My teammate was using me as his personnal programming assistant making me do all his dirty work.
* My day to day supervisor would vigorously argue with me about some of the most inconsequential things such as code line length.
* My project supervisor (the COO) didn't understand robotics and would decide the direction of the project and I'll quote: *"Knowing the direction of gravity doesn't matter, we just want lidar scans."* Enter crooked maps and drifting lidar scans.
* My ideas would repeatedly be shutdown only to be brought back when someone in management decided it was a good idea after seeing a competitor with the same concept.
* My CEO wasn't developping a business case. All he had going was this one guy from a construction company saying he would be interested in such a product. I later realized we weren't actually there to develop a product but to fill a [series](https://buyandsell.gc.ca/procurement-data/award-notice/PW-SV-011-34025-001) of [contracts](https://buyandsell.gc.ca/procurement-data/award-notice/PW-SV1-005-37033-001) the company had with the Government of Canada. I don't think I can say what we did, but I do think I can say that I wasn't proud. Nothing illegal of course, but I do think my research advisors would have been very much dissapointed.
* The project was poorly managed, there was no clear vision on what we were building. There weren't even any specifications or requirements to meet.
* I was stuck doing a mix of embedded programming and hardware to synchronize sensors, continuous integration because apparently 2/3 of the software guys in the company couldn't be bothered to maintain our Jenkins server, teaching C++ to my teammate and writing some infrastructure code to accomodate his poorly written algorithms. Basically no robotics.

I was a bit over a year in and couldn't take it anymore. All that time had been wasted and I had nothing to show for it. My career was off to a terrible start and I had learned nothing in that span of time other than the fact that I didn't want to be surrounded by people who had less experience than I did. And thats saying quite a bit coming from someone fresh out of school. While others would relish at the chance I wanted to be somewhere where I'd be the dumbest one
there with everything to learn. I wanted to step on a springboard that could eventually launch me to a job at
[X](https://x.company/). 

I started looking for a job but this time I actually put some effort into it. After a few interviews with
various companies, I decided on join the [Applanix Autonomy team](https://www.applanix.com/products/autonomyplatform.htm). While very small team and not quite related to drones, it looked like a great opportunity for learning and career growth without moving to San Francisco with all the startups backed by VC money.

<figure>
  <img style="width: 75%" src="/images/career_moves/applanix.jpg"/>
  <figcaption>Smiling because I never saw so many lidars in person.</figcaption>
</figure>

Today, I am cautiously optimistic about the move I made. The guys are competent, the product directors
understand the technology and are serious about making a business out of it. The product is already being
deployed on customer premises with the team doing multiple field deployments a year. All new employees go through a sort of orientation on their first week which was my chance to ask some longstanding questions I had accumulated over the past year. I learned more in a two hour conversation with the guy
working on qualifying IMUs than I did in an entire year at my previous company.

During a meeting with the Director of Engineering, I was explained the engineering process within the company, which was a bit of a mix between more rigid almost aerospace-like processes but with some of the flexibility from more modern software development practices such as Agile. To my surprise, and great pleasure, I was told *"You have a right to ask what the specifications and requirements are."* 

The thing I used to have to fight for was now my God given right.

***Thank Fuck***