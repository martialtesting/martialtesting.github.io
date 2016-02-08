---
layout: post
title: 'Automation Kick Off: Beginning Automation with the right foot(I)'
date: '2013-04-18T00:43:00-03:00'
tags:
- testing
- automation
tumblr_url: http://www.martialtesting.com/post/98366634769/automation-kick-off-beginning-automation-with-the
author: "Ignacio Esmite"
---
Ok, we decided to introduce automation to our project, so, how do we start? In other words, which is the strategy that we should follow to introduce functional testing automation in our project or organization? The objective of this blog post is to start a series of posts that do not describe how to introduce automation because depends on the context, but instead, the purpose is to describe how to **not** start with automation. Any resemblance to errors in projects I’ve worked on is pure coincidence:)
<p align="center">
  <img src="/assets/automation-kick-off.jpg">
</p>


**Automation is development: Where is the architecture?**

Maybe the first natural step to do is to pick a tool(let’s take apart the strategy to compare tools) and start “playing” with it. Thereafter the second step is start to create tests to check how well is the tool on our application under test. At last we’ll show results to our partners, manager and others. So ok, let’s use that tool, in which date do you have X test cases automated? In this point is where the problems come, we estimate the X tests, we develop them and we run them in our environment. Works great,  doesn’t it?

From my point of view this approach could be the kick off for a failed project, take into account that:

- What happens if at some point the UI changes? or the behaviour of a component changes? Should I maintain all tests? This is unacceptable for the automation ROI
- What if some behaviours are repeated in some tests? Should I copy paste? This practice does not permit scalability
- Let’s assume we run the tests on our local machine. What If we go on vacation? Who run the tests? What if we have suites that takes 2 hour to execute? 8 hours? Please give me pop corn and a coke to watch the movie!
Usually an automation project has the same components as a development project:

- A plan
- Need to build a backlog:  Which test cases we want to automate? Is it worth your while?
- Architectural definition: if we do not define an architecture we’ll suffer in the short run.
- Code, anyone will test our “application”, so if we do not define a methodology, reusability practices and code standards we’ll inject bugs to our tests. From my point of view, once we lost the confidence on our tests, it is pretty difficult to trust them at anytime in the future.

An approach to start an automation project could be:

1. Pick a tool
2. “Play” with it
3. Design a framework that assist us to resolve some basic problems like: Data Driven Testing, Reporting, Reusability, testing focus instead of boilerplate code.
4. Design initial test cases that we think are needed for automation.
5. Develop a small initial test suite.
6. Deploy to Jenkins, TeamCity or any other continuous integration server that allow as to run test scripts from any machine .

Having that as a baseline, it is possible to scale from the kick off without short term risks related to neither scripts maintenance, nor re-designing all of the architecture in our tests.

What do you think about it? Would you add any other initial activity to an Automation Kick-off? If so, share it with us.

photo credit: [ElDave](https://www.flickr.com/photos/eldave/3092991138/) via [photopin](http://photopin.com/) [cc](http://creativecommons.org/licenses/by-nc-sa/2.0/)
