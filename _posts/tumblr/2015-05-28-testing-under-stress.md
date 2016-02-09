---
layout: post
title: Testing Under Stress
date: '2015-05-28T09:37:34-03:00'
tags:
- testing
- planning
- tester role
- stress handling
tumblr_url: http://www.martialtesting.com/post/120103379259/testing-under-stress
author: "Ignacio Esmite"
redirect_from:
  - /post/120103379259/testing-under-stress/
  - /post/120103379259/
---

>CEO: Hey, how do you feel about the quality of the new model we shipped yesterday?
>
>Head of QA: Great! The new assistant integrated with the GPS will kill our competition.
>
>CEO: Awesome! You guys did an excellent job during the last weeks, I know we have a delay on our production but, you were >able to accomplish your job in a lesser amount of time. Well Done!
>
>Some minutes later ...
>
>CEO: Hey, we have a huge problem reported by our resellers
>
>Head of QA: What happened?
>
>CEO: The engine did not start!
>
Head of QA: ...
>
>CEO: I know that the addition was covered but I guess you guys verified that the engine started right?
>
>Head of QA: Give me 5 minutes, I have to take a walk and kill myself…

![Stress](/assets/stress.jpg)

How do you feel about that scenario? Do you think it would be possible that that could happened to you? The topic we want to cover in this post is **how stress can affect our clarity of mind** when it comes to designing and executing our plan.

Usually, most projects we take part of have strong requirements of deadlines: market reasons, sales promises, contracts, etc. Since Software Development is probably one of the most difficult disciplines to plan, the starting time is a scarce variable, so, can you imagine which is the area that takes the worst part regarding this? Yes, you are right: Testing.

Once the deadline is close, all stakeholders start to get nervous regarding the project, start asking questions, and probably, the testing guys(you) start to be the oracle of the project status. It’s a matter of time until the stress and pressure is over the testing team, and this could lead to making fatal mistakes while you are working.

There are some activities you should perform before that time, so you can have a set of tools to use in the **countdown** phase:

- Plan, plan, plan:
  * We aren’t talking about building an old fashioned test plan, take a look to this incredible useful [James Whittaker](https://twitter.com/docjamesw) [article](http://googletesting.blogspot.com.ar/2011/09/10-minute-test-plan.html).
  * You need at least to focus on:
    * What you will test;
    * What you won’t test: be honest, why not? Do an exercise to evaluate the risk, you don’t need a number, but at least, a strong reason to keep something out of scope.
  * Estimate how many times you’ll need to do this, don’t be scrimpy or you’ll regret it in the **countdown** phase ;)

- Gather all the information you need:
  * Do mind maps or any other thinking strategy to understand the new additions to your project. Share them with the team, ask questions to the stakeholders. Anything you can detect at this point, will help in reducing the time of the team to develop the product and you will also be reducing development<->testing iterations. If you don’t do this for the team, be selfish and do it for yourself; your **"future self"** will be thankful.
  * Do the exercise of building a bulleted list with potential risks, share it with the team. Don’t be afraid to share your thoughts, maybe others didn’t think about it.
  * Think as a product user: this is the time to do it, in the **countdown** phase you’ll start investing most of the time in the new additions, probably, you’ll be smarter at this stage than closer to the deadline. Think that most of the time, Users will not want to lose current product features and for that, plan accordingly. Do you have automated checking? Great! But think that maybe some new features could affect the product in a way that did not happen in the past, evaluate current automated coverage, study it, criticise it.

## The Final Countdown

At this point, it is the moment that you need to stay calmed and focused. You don’t have to soak up all the delays in the project. Are you part of the team? Yes, you are! but you don’t have to feel the responsibility to fix any planning fault. If you try to resolve the tasks in a lesser amount of time than you need, guess what? That error in production will be your fault. Some cases are unfair, but others… we just deserve them, we neither thought, nor acted with clarity.

Now is the time to start using as inputs, the work that was performed by your **"past self"**:

- If you planned X days,  by any circumstance don’t think that you are Batman or any other kind of superhero and now you are able to perform in X/2 days. Rise it, talk about the risks of the release, be clear that if you keep the dates you have risks and explain that with strong reasons. That’s why it is important to have a plan and gather information, you have strong arguments to give information to the stakeholders.
- Please don’t forget about the users at this point, do you remember our new model car users? We don’t want our users will not be able to start their engines.
- Never lose the big picture.
- Be transparent with the information you share. If you know something could go wrong in production, let other stakeholders and project members know about it, you are not Harry Potter, and that risk will not vanish into thin air with a spell.

What do you think about the times that you have the backpack? How do you handle that? Did you ever lose the big picture in those moments? Do you feel that at any point you want to have the time machine to go back and change the way you planned for? We want to hear about your thoughts :)
