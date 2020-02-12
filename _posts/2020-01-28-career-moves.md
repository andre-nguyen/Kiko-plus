---
layout:     post
date:       2020-jan-28 00:00:00
title:      M.A.Sc. to now
summary:    Finished my master's degree and wondered where to go from there <figure><img src="/images/applanix.jpg"/></figure>
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
classes requirering mathematical rigor I had not properly developped during my
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
  <img src="/images/geralt.jpg" />
  <figcaption>If you haven't seen The Witcher on Netflix, at least watch
  this <a href="https://www.youtube.com/watch?v=2BSrsUR5ph4">supercut</a> of 
  Geralt of Rivia saying fuck to understand how I felt at the time.</figcaption>
</figure>


To be entirely honest, I had no idea what the legal consequences of quitting were, if any.
I just knew I was committed to something and it would be in bad taste to break those committments. I was barely hanging on but with the help of friends and my advisors,
I kept pushing, put my name on those publications, passed the rest of my classes,
delivered on that research project and wrote my thesis in about 2 months, judging from
the commit logs.

<figure>
  <img src="/images/thesis_commit.jpg" />
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
    <img src="/images/vacation_small.jpg" />
    <figcaption>Look at this guy having a grand ol' time</figcaption>
  </figure>
  <figure style="width: 50%">
    <img src="/images/diploma_small.jpg" />
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
were targeting. I would spend hours breaking down my tasks into Jira almost down to the half
hour with bogus time estimates that would get challenged. How am I supposed to estimate
how long something will take if I've never done it before? Should I really time box my
litterature review and stop it after only two days? How do you know there isn't four days
worth of literrature out there for the component I am building? It seemed like the worst of
two worlds, a small company with low ressources but with the bureaucracy of a large company.

We would have a daily company wide scrum where some employees would literally have full conversations trying to problem solve instead of sticking to the basics. After a while I
noticed that no one was actually listening when anyone from the SLAM team spoke. Sometimes
my colleague would say something surprising and no one would react. I came to the conclusion
that a good 3/4 of the scrum was actually a waste of my time.

There came a time when I simply asked what the project requirements are and the CEO bounced the
question back at me. It was management's way of acting like they trusted you with the
technological decision but once you made the decision you would invariably be overridden.
So much for the "freedom" and "responsibility" that comes with working in a small company.
I replied with another question: *Who's the product owner and who's the product manager here?* I asked the question, not because I didn't want to set the requirements, but because
the previous times I had tried, I would either waste time arguing with my colleague about who
was right when he hadn't even bothered researching our competition or my decision would be 
overridden.

My question was met with silence on the Slack channel. It turns out management had an
emergency meeting to clarify what everyone's role was. *"Let's forget Agile methodology
roles because not everyone is familiar with them."* My blood was boiling. They created a new
organizational chart showing everyone's role. Somehow a two person project had 7 stakeholders. The CEO would represent client interests, the COO would make sure we filled
our sprints and followed agile-ish methods. The CTO would make the final calls on the
technological decisions. The day to day scrums would be supervised by a "senior" software
developper who had no background in robotics. I would be both a SLAM developper and
a system integrator because I had a lot of hands on experience on robotics. My colleague
would be a SLAM developper, in essence bringing his master's thesis to real life.

Thus, the only management person who could understand what we were doing (the CTO) would
only have a distant role in the project. *Great.*

### Bad project requirements

As mentioned previously, when I joined the company they had started building a drone
simulator in Gazebo with some lidars. The drone ran a stripped down version of the
autopilot firmware in a software-in-the-loop fashion. It wasn't quite complete as the model
wasn't actuated by the firmware, but the state estimation was running using the simulated
input which was good enough. 


<!-- 
Sure GPS denied navigation is something interesting that you could want, but
how accurate does it need to be fore the customer to shell out money? How will the end system
be used? How much of the integration are we doing ourselves?




The reality was that we were an internal research project funded by a government grant. In fact,
we didn't really have any requirements, what little I had planned at the beginning was 
thrown out without my knowledge. While the project started off as a GPS denied navigation
system for drones, it had changed to a LIDAR scanning system. Whereas the former focuses
on accurate and timely odometry data, the latter is interested in pointcloud models. While
both are intimately related, they are fundamentally different in their objectives. 


Bad
requirements and objectives ultimately lead to me presenting a plan that got dismissed on the spot.  -->
