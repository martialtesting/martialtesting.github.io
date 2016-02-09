---
layout: post
title: Mind Mapping in Testing
date: '2015-06-15T23:41:08-03:00'
tags:
- testing
- toob
- mindmaps
tumblr_url: http://www.martialtesting.com/post/121644552329/mind-mapping-in-testing
author: "Ignacio Esmite"
redirect_from:
  - /post/121644552329/mind-mapping-in-testing/
  - /post/121644552329/
---
Hello everyone! Today as a sequel to our last article, we want to kick off a series of blog posts related to the usage of mind maps for testing. The aim of the articles are a compendium of ideas and experiences we have collected over the course of time while using mind maps. Please share your thoughts, let’s keep an open discussion about it to keep on learning and improving our day to day work :)

![Mindmaps in testing](/assets/media/mmtesting.png)

>This mind map will be extended in each new blog post from this series.

## Which are my initial thoughts on how I could use mind maps in testing?

- **Describe plan of testing**: if we take into account that a mind map is just a tree structure, we could start adding childs to set forth:
  * Charters of exploratory testing, organised in a root level of the plan or breakdown in Stories/Features, ticket numbers, tester’s names or whatever is the organisation you feel comfortable, there is no silver bullet for this, it always depends of your context;
  * Scripted checking? Of course! You may consolidate your scripting testing with exploratory testing and have all of them hanging in the same tree and all you information is consolidated;
  * Automation? If you have the skills to automate tests I’m pretty sure you know how to build a tree of execution of your tests! and of course, you may also link one mind map to another (the mind map of the plan of testing!);
  * Express other types pf ideas and activities in the mind map containing your plan.
- **Describe your scenarios of test**
  * Do you execute scripted tests? Use mind maps to express them, is just a tree like any other testing tool and you could add the script as node information;
  * Do you use exploratory testing? Use mindmaps to define charters and handle sessions. Regardless you are using SBET or not, mind maps are a great tool to express units of execution of exploratory testing, and also come back later at them to understand which parts of your plan were covered;
  * Any other scenario of test could be represented in a mind map, and having it stored in some place could be very useful;
  * Execution log, there are several mind mapping tools that allows you to set up states in nodes, so you could use the leafs of the mind map as “units of execution”. You could define whatever framework fits to you, the aim of this post series is not just define “a way” of working with mind maps. We want to hear from you on how you use it!
- **Add information as needed**. Some mind maps tools allows you to add information to nodes and add custom measurements.   Sometimes we used to attach bugs found, issues found, complexity points, and any other information needed.
- **Getting Information**. Once you have all of this information in a mind map or linked mind maps is pretty simple to build a script to aggregate information and build reports to express testing coverage, bugs found, lists of issues reported, complexity points of testing areas, etc.
- **Log of our knowledge learning curve and execution**. We want also share one approach of how to organize your mindmaps. Storing them in a filesystem is ok, but in our opinion there can be better approaches to store the data and afterwards, compare our outcomes throughout time.

To organise this series of posts, below you will find the agenda with the topics we’ll be covering in the upcoming weeks:

   1. [Planning using mind maps]({% post_url 2015-07-01-planning-using-mind-maps %})

   2. Designing and execution using mind maps

       * Exploratory (Coming Soon)

       * Scripted (Coming Soon)

   3. Getting Information from mind maps (Coming Soon)

   4. Don’t miss your history or how to use mind maps with Github (Coming Soon)


Have you worked with mind maps to manage your testing? How do you feel about this approach? We want to hear you thoughts about this!

Stay tuned with this series of posts!
