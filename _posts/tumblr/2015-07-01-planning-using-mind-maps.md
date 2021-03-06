---
layout: post
title: Planning using mind maps
date: '2015-07-01T00:42:50-03:00'
tags:
- mindmaps
- mind maps
- planning
- testing
- adapting
tumblr_url: http://www.martialtesting.com/post/122916189724/planning-using-mind-maps
author: "Ignacio Esmite"
redirect_from:
  - /post/122916189724/planning-using-mind-maps/
  - /post/122916189724/
---
Hello to everyone! Today we’ll continue with the series of post related to [Mind Maps in Testing]({% post_url 2015-06-15-mind-mapping-in-testing%}). Last time we did a kick off describing some areas where the mind maps can be useful. Today it’s time to go deeper in the area of planning using mind maps.

## Test Plan
Before we start, what is a test plan? There are tons of definitions on the subject, there are lots of template if you take the time to google it, but our thinking of what should be a test plan is close to [The 10 minutes test plan](http://googletesting.blogspot.com.ar/2011/09/10-minute-test-plan.html) than an ISTQB definition of what should be a test plan.

Some “features” I would like to have in a test plan:

- **Meaning to the team**: the test plan should be a living doc, the team should use it, questioning about the approaches we are doing and understand our main goals. If the plan will be stored and will never be used, what’s the purpose of having it in the first place? We don’t like documents or artefacts that we’ll never use; if that is the case, why did we invest time in it instead of learning or doing something more interesting?
- **Dynamic**: don’t be afraid to change the scope or approach of testing throughout time. It’s a fact that the product will evolve, the features will undoubtedly evolve, so if we don’t adapt our Test Plan to that reality, what is the objective of having it?
- **A source of understanding for our product goals & strategy**: I always tend to talk about the product and not only QA or Testing b/c what we are delivering is a product and the quality is a responsibility of the whole team.
- It would be nice if our test plan reflects the **performed activities** not only what we’ll be doing, this approach enforces the goal of “meaning to the team”

## How to use Mind Maps to Plan

Using mind maps tools give us some flexibility that are difficult to find using other approaches:

- **Simple to extend/Dynamic:** when we are doing any kind of testing activities is simple to add nodes and express that information in a simple way so everyone could easy understand
- **Tree structure:** as a mind map is just a tree is simply to map not only testing activities performed as a tester, is simple to convert automation results from XUnit results to a tree in the format of the tool we are using
- **State:** there are lots of mind maps tools that allow us to set a state to a node, the states we want to use depends of our context and the way we want to express it but you could for example use to mark activities as: in progress, completed, pass, fail, blocked, etc.
- **Measurements:** some tools allow us to attach some custom numbers to nodes, this is great to add information like complexity points to estimate time invested in some areas, number of bugs if we are interested in have a track of the amount of related issues or any other kind of information you want to attach to a node and later aggregate as a result of the testing activities. Remember that a mind map is usually stored as a tree so it’s pretty simple to build a script to get all of this information automatically for us.

We usually use [Mindmup](https://www.mindmup.com) for some cases when we need measurements and states. Open Source project is [here](https://github.com/mindmup/mindmup).

## Some simple examples

We want to give you some samples of mind map usage, we don’t like to express as methodology or "best practices" because this depends a lot from your context, goals, testing strategy, etc.

### Have a global mind map for the plan

We usually use a single mind map that link other mind maps. A good approach could be have all the related mind maps stored in github and have a script or application that load all the data and build a dashboard; following that approach there is no need to collect data manually ;) Also having all that information in github or any other repository is simple to build a snapshot of what we did in the past and analyse and learn from those experiences.

### Describe risks

Mind maps can be used to describe the risks, identify possible problems which must be discussed with the whole team. Having this kind of things expressed in a mind map could be a good approach to optimise your meetings with the team and help them understand potential problems from the beginning. Remember that if we can address this kind of issues from the beginning of the iteration, then it is prone to reduce the likelihood to have problems close to the release time ;)

### As a tool to work together with development

Mind maps are great to discuss with development, as soon as we can discuss our ideas and other stakeholders ideas with development the better. There is a high likelihood that the quality of the product is better if development knows what we’ll be looking before they finish the implementation. The cycles between dev & testing will be less if we all are in the same page.

### Describe features & bugs addressed

Do not use mind maps only to describe testing scenarios, mind maps is a great tool to describe our ideas regarding a product. Don’t think only about which are the title of the new features, improvements or bug addressed, we can do better than that and start learning and model the reality from day 1.

### Describe charters

It’s pretty simple describe charters and group them by feature, area, or whatever you think is best. Later is simple to have a big picture of which are our testing goals and discuss with the team. I found that meetings could be much more productive with a mindmap than a spreadsheet or a regular testing tool. In future posts we’ll share an approach to do exploratory testing using mind maps.

### Describe scripted testing

Is pretty straightforward to build suites of scripted testing using mind maps. Also is pretty simple to build plans, add tests to plans, etc. Is much flexible than use tools like testlink that you need to create the test, create a plan, add a plan, create builds, etc. If you need to repeat a plan modified is simple, just copy, paste and modify on the fly, pretty simple right?

### Describe automated checking

As we said before, it is simple to map an XUnit report to a mind map tree. If we add just one step to our automation we can have all our testing activities integrated in a single mind map. Building a dashboard with all of this information is incredible useful!

### Have separate nodes for different goals

Keep it simple! Build a single testing plan and group each activity in different mind maps linked to the main one. I usually have different nodes for: Risks, Product Analysis, Testing Ideas, Testing Sessions or Threads, Scripted Checks that we usually run before go to production, Automated Scripted Checks, grouping testing sessions per product version. All of those activities/nodes depends of your context! Please share your experiences!

### Learn from your practices in future iterations

Having all of this information stored in github give us the flexibility to build in a simple way a snapshot of the result from previous iteration. Using for learn! Analyze which problems did you have in the past, review testing ideas and sessions. Did you have some problem in production? try to detect a pattern of why did happen, keep learning from your practices and your product! The goal is improve our skills and practices as much as posible!

Do you think using mind maps for planning is a good approach? Have you used them before? Share you thoughts and stay tuned with our [mind maps in testing series]({% post_url 2015-06-15-mind-mapping-in-testing%})! Next topic to cover will be using mind maps to represent our testing scenarios!  Stay tuned!
