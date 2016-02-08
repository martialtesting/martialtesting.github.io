---
layout: post
title: Pushing the limits with boundary testing - Part I
date: '2014-11-15T07:32:33-03:00'
tags:
- testing
- technique
- boundaries
tumblr_url: http://www.martialtesting.com/post/102686268074/pushing-the-limits-with-boundary-testing-part-i
---
As testers, we are often faced with a challenging task, and that is modeling our application under test through a critical thinking process.

This technique relies on the fact that boundaries must be tested because it’s where so many defects lurk. Particularly, in my own experience this situation has happened plenty of times.

The steps which have helped me use this technique effectively are very simple:

- **Step one**, identify the equivalence classes;
- **Step two**, Identify and recognize the boundaries which comprise each equivalence class;
- **Step three**, model and build your tests for each boundary value. One point “above” and one point just “below” the boundary.
Now, “above” and “below” are in bold because they depend on the unit you are working with, an example:

- Let’s say we are working with integers as a unit, and our boundary value is 100, then a point above is 101, and a point below is 99;
- However, if we were working with decimals as a unit, and our boundary is 100,00, then our boundaries change, and a point above is 100,01, and a point below is 99,99.

If we use this technique along with other ones, they help us build the mental model of our AUT in the context of our project, shape a suitable strategy for it, reduce the amount of tests to build and execute while maintaining a good coverage (just because you are not building 1000 tests does not mean your tests lack power), and last but not least, the aim of this technique relies on working passed, beneath and against the boundaries because it’s where bugs often hangout.
