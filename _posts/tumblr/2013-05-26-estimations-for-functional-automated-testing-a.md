---
layout: post
title: 'Estimations for Functional Automated Testing: A Simple Approach'
date: '2013-05-26T00:49:00-03:00'
tags:
- testing
- automation
- effort
- planning
tumblr_url: http://www.martialtesting.com/post/98367139739/estimations-for-functional-automated-testing-a
---
Probably one of the most complicated problems to solve when planning a project for automation, it’s related to estimating the amount of time it will take us completing our backlog. In the event we are planning for a project then it might be a little less of a problem if we are working with Agile methodologies because we can adjust estimated times, however, provided we are not working with neither a methodology nor a framework, then improving our estimation process, and thus, our margin for error may prove a difficult task.

Besides, jumping to a conclusion of the type "I’ll develop 1 automated test in X given time" measured from an average is not really that useful, it would be the equivalent as saying something as the following: "my development team is capable of developing one feature per week".

![Estimations](/assets/estimations.jpg)


One of the most widely employed strategies is that of “Expert’s Judgement”, in which an experienced automation tester or group of them, determine through their understanding and experience how long it should take them to automate a set of tests. Clearly, either by the absence of another approach or framework, that one is better than not estimating at all, still, from my point of view the greatest weakness it has is that we are unable to improve it, whether we overestimated or underestimated, what should we do to improve the way in which we estimate if technical problems and the model of reality is different? Even if we were before similar scenarios, how should we improve that approach?

The intention of this post is describing a simple approach which will enable us to estimate a set of scenarios and, at the same time, gives us the tools to improve estimations for the following iterations and/or projects. The approach takes the following variables into consideration:

- Variables for estimating
- Initial constants, which are the parameters that can be adjusted iteration per iteration
- Formulas which allows us to calculate the necessary time to automate a set of scenarios

## Variables for Estimating

- **Step Complexity:** we have to be able to describe each scenario as a set of steps, once we have the steps then a complexity must be assigned such as Low **(LComplexity)**, Medium **(MComplexity)**, High **(HComplexity)**. At this point, we should try to standardise what we understand by each type of complexity, however, it may vary depending of the context of the project we are in. In order to give an example, we could say that either a simple click or filling a textbox as a low complexity step, querying a database to retrieve information as a medium complexity step, and performing the access to a component which is not a standard in the UI as a high complexity step. It’s worth stressing the fact that we can always have either a high or medium level complexity step as a set of steps whose complexity is set to “easy”, although, it is always better having a larger array of options in terms of complexity for it reduces times in estimation, but, it is prone to increase uncertainty levels.

- **Reusing Scenarios:** it is always convenient grouping similar scenarios, thus, identifying weight for reusing different scenarios. If we have a set of scenarios which work with a form, most likely we can reuse a certain percentage of the previously implemented scenario. It is convenient assigning a value between 0 and 1, so that we identify either reuse of the scenario, or no reuse of the scenario at all.

- **Auxiliar Components of the Scenario:** It is a good practice building auxiliary components which can be reused by several scenarios, under such circumstances, it is recommendable to estimate a value in units of time for the development of such components.

## Constants

Development Time by type of Complexity of a step in minutes **(LTime, MTime, HTime):** this constant indicates the time in minutes required to implement a step of this complexity. This one may be sharpened throughout the on-going iterations, for so long as we identify a set of appropriate variables and constants, we will be capable of improving our estimations in each iteration. If we want to have a greater degree of refinement, it would be desirable having a time for each type of complexity taking into consideration the seniority of the team members, the development time are bound to differ between a senior and a junior team member.

## Formulas

Given the variables and the constants defined, it turns out to be quite simple having a set of formulas which will allow us to quantify the necessary time for developing a set of scripts.

```
Development Time of an Scenario in Minutes (ScenarioTime) = (#LComplexity * LTime + #MComplexity*MTime+#HComplexity*HTime)*(1-Reuse) +AuxTime
```

Where **#** is equals to the total amount of occurrences of steps with the same type of complexity.

```
Development Time for a Set of Scenarios (TotalTime): it is the sum of all the times for all of the scenarios.
```

## Conclusions

Using those simple formulas, we start working on a base upon which it is possible to estimate and refine our estimation effort progressively throughout on-going iterations. Either adjusting development’s time given a certain degree of complexity, or refining our definition of what each complexity stands for, we can then improve our estimation from one iteration to the following, or even from a project to another one. Lastly, even though this strategy is very simple, it is always better having a strategy in place which will allow adjustments throughout time.

Other variables/constants to take into account could be:

- Time for the setup of an environment
- Time for the deployment of the scripts
- Time for debugging/testing the scripts
- Time for setting up an appropriate framework for automation
- If applicable, time for designing the scenarios
- Time for designing the auxiliary components for the test scripts

So, what do you think about the approach? Do you happen to find it useful having a framework for estimating? "Expert Judgment" rocks?

See you next time!
