---
layout: post
title: Session Based Exploratory Testing - A first approach
date: '2015-05-31T23:12:02-03:00'
tags:
- exploration
- exploratory
- testing
- sbet
- session
tumblr_url: http://www.martialtesting.com/post/120409682044/session-based-exploratory-testing-a-first
author: "Andres Curcio"
---
Hello! In our previous posts, we began [talking about Exploratory Testing]({% post_url 2015-05-20-thoughts-on-exploratory-testing-the-white-belt %}), and afterwards, [defining it along with exploration]({% post_url 2015-05-24-thoughts-on-exploratory-testing-digging-a-little %}).

Today, we want to keep on sharing with you about this subject, but first, let me share a quick definition written by [James Bach](https://twitter.com/jamesmarcusbach):

>"Exploratory testing is simultaneous learning, test design, and test execution.""

Doing those activities simultaneously, having taken the context of the test item that we are testing into account is the objective after **Exploratory Testing**, and that’s also what differentiates it from only following a predefined script.

Nowadays, in my personal and professional experience, it’s kind of difficult talking and praising **Exploratory Testing (ET)** whilst not saying a word about the subject we will be talking about today, and that is, **Session Based Exploratory Testing**.

Let me give you a little background and history on **SBET**, it was originally developed by [Jonathan Bach](https://www.linkedin.com/in/bachjon) and James Bach in Y2K, and it was conceived and developed as an approach by testers, for testers, so testers could use it to:

- Document our work that will ultimately provide evidence of it to stakeholders; and also,
- To measure the work we do whilst engaged in our exploratory testing work on a test item.

> WHAT IS SESSION BASED EXPLORATORY TESTING?

As already mentioned in this post, it is an approach and as such, it gives us some pointers so we can focus our work at hand, either by prioritising it by risk, or by degree of importance to the project, or per functionality of the test item, among others. Having that said, and from my personal experience using it:

- SBET makes it easier to report and present the areas that were covered,
- It helps us while undergoing scrutiny with stakeholders, and also,
- **To improve the coverage of our future test sessions, by using the knowledge acquired from the results of our past test sessions.** Employing that acquired knowledge will have as a consequence on our tests, that they will grow stronger and smarter, and ultimately, the coverage of ours tests will also be improved.

![SBET](/assets/sbet1.png)

As you may have already noticed, the post began with the definition by Bach, now, to stress the last point, I’d like to share the following adaptation by [Elisabeth Hendrickson](https://www.linkedin.com/profile/in/testobsessed):

>"Exploratory Testing involves simultaneously learning about the software under test while designing and executing tests, using feedback from the last test to inform the next."

From my current experience, I can tell you that in order to draw out the latest pieces of information regarding a test item, we must employ the most suitable tool we have at our disposal for it. More often than not, the variety of conditions surrounding a test item are changing almost permanently, therefore, we have to use the best approach we have at our disposal to match those changes, and in my opinion, **Session Based Exploratory Testing** is an approach I have found to be highly valuable.

**WHY?**

Simple, because:

- We design;
- Log potential new test ideas;
- Change and adapt our tests based upon the results we’ve acquired, which also include the tests recently completed;
- We report results giving value to the project, thus providing instant, and reliable information about the test item we are working with;
- We are aligned with the context of the test item.

Moreover, with this approach, by no means are we forced to follow pre-established instructions, on the contrary, and in similar words to [Cem Kaner](http://kaner.com/)’s definition on **Exploratory Testing**, "our personal freedom is emphasized, as well as our responsibility to continually optimize the value of our work."

Don’t get me wrong, I am not discarding scripted tests, not at all, because I still happen to use them as tools to set a knowledge foundation, to widen attention, and also, to generate new testing ideas.

> WHAT DOES A SESSION LOOKS LIKE?

![SBET](/assets/sbet2.png)

The session’s report I am sharing here, it’s the same the Bach’s brothers have developed and shared with the community, and also, it’s the format I have used the most either in a piece of paper, a mind map, a plain text file, or a spreadsheet, but that… that is something we will dig into in other posts. In the meantime, let me share with you the components and what they are for:

**Charter**

- This is the mission of our test session, and it usually describes in a few sentences our objective as well as our focus;
- There are general and specific missions, which we will also dig into in future posts, do not despair;
- In addition to that, the charter may also contain information about the area of the test item we have to test, and if necessary, it could have some information as to how you should start testing it.

Do you remember that I previously mentioned we log **new test ideas**? Throughout our exploration work, and if we happen to find an area which is potentially risky and that it’s not a part of the current charter, then we can write a new one to address it.

**AREAS**

- This **sub-section**, belongs under the **Charter**, and it’s purpose is record, as well as listing information to provide evidence regarding the coverage of our testing.
- Therefore, it is prone to contain information related either on the areas, or functionalities of our test item that we will go through, also, operating systems, and/or browsers spectrum.

Let me show you an example of how this sub-section can help you, using a dummy example:

>\#AREAS
>
>OS | Windows 7 32x and 64x
>
>Test Item | uPrint 0.3.6
>
>Menu | File
>
>Menu | Actions –> Print to file
>
>Strategy | Function Testing

With that example, we are showing what our **os** will be, the **version** of our **test item**, the **areas** we will cover (**Menu**), and the **strategy** we will be using.


**Start**

- In this section we record the date and time the session began.

**Tester**

- Insert your name or, the name of the tester, or testers (if you are doing Paired Testing).

**TASK BREAKDOWN**

**Duration**

- In here we use a predefined amount of time that we will be spending for our session. The different values that I have personally used and have found to make me more productive are:

  * Short from 40 to 60 minutes,
  * Normal from 60 to 90 minutes, and,
  * Long going from 90 to 120 minutes, I will not extend sessions for longer periods.

One piece of advice on this particular point, **Duration** in the report doesn’t have to be precise, why? Because remember, we aim to spending the majority of our time **testing**, and a lesser amount of time on administration.

**Test design and execution**

- This section is completed with an integer, and it represents a percentage going from 0 to 100.
- Its usage evidences the amount of time we employed to test against our test item.

**Bug investigation and reporting.**

- Alike the previous section, this one is also filled with an integer which represents a percentage, which also goes from 0 to 100.
- And its purpose relies upon recording the time spent on either investigating and reporting problems.

**Session setup.**

- As its predecessors, this section is also completed with an integer representing a percentage going from 0 to 100.
- It is used to record time that was spent setting up “things” that support our testing activities, yet, that they are not testing itself.

For instance, a **session setup** could be:

- Configuring a DBMS to work with the DB  so you can run queries, also,
- It could relate to getting your test data ready (should that depend on you, of course), or even,
- Installing a piece of software you need to conduct your testing activities, and the list goes on and on.


```
Important notice:
The grand total of running a sum operation through the three previously mentioned percentages must add up to **100%**. That 100% is the equivalent of the total amount of time we used for our session.
```

So, if we ran a short session for 50 minutes, that is our **100%**, which, for the sake of explaining the distribution could look like this:

**Test Design and Execution**

#65

**Bug Investigation and Reporting**

#20

**Session Setup**

#15



Moving on to the following sections available in a Session report…

**Charter vs. opportunity**

- The syntax for this area is represented as a ratio of the session, and personally, the ratio I have used and spent the most is 80/20.
- That means, I have usually spent 80% of the time of a session (regardless its duration) focused on the charter (the mission), and, I have spent a 20% on the opportunity.
- The opportunity represents off-charter work, and that means it’s time I’ve used, for instance, to investigate areas which could be potentially risky, and by going off-charter new test ideas have been generated to address them.

From TASK BREAKDOWN and up to this point, the report is focused on providing and giving value, by presenting how time was spent on what we might call **"Qualitative Testing"**.

A piece of advice on this point also, in case you gave this a try and noticed that you spent more time on the **opportunity**, rather than the **mission**, then make sure to go over your **charter** to adapt it accordingly, or, to create a new one.

Also, bear in mind that it is (as it usually is) complicated to estimate the ratio of our work. So, as a recommended practice, it’s a good idea to focus on a fixed ratio at first, yet keep in mind that as your tests unfold and progress, it may, and it most likely will vary.

**Data files**

- This section if meant to keep records of any and every file we may have been using throughout our test session.
That proves to be very useful, for instance, in case you or any other tester happens to have to run a new session over the same area/functionality in a new iteration of the project, and having that piece of information easily available will provide her with a better idea, and starting point.
- Keep in mind that all file that is mentioned here, should be saved to a known location.

**Test notes**

- In my opinion, this section is essential and one of the most important ones.
- It is in here that the tester(s) will record anything they deemed important over the course of the test session.
- An example would be,
  * Showing how the tests were performed;
  * How the test ideas developed throughout the session;
  * Pieces of advice for the tester(s) who might need it;
  * What challenges were either solved, or recognised;
  * etc., etc.

**Bugs**

- The section, as the name describes it, is meant to list the bugs we find throughout our session.
- Nowadays, and because there are plenty of Defect Tracking Systems, what I commonly do here is list the name(s) of the defect(s) along with its corresponding **ID#** in the tracking system.


**Issues**

- Lastly, this section lists either **problems, issues** that came up throughout the testing session.
- Let's say for instance, that it was the test environment that caused problems and blocked our testing, we should log it here; or also, it could be used to record problems we noticed and found, which could ultimately be deemed as bugs, but we cannot tell for certain until we have it either contrasted against an oracle, or until we have investigated it some more.

An issue may be seen as:

- Anything that threatens the value of the testing, or of the project, or of the business. Moreover, those that affect our work making it slower and harder, give bugs the chance and time to run and hide, reason why fixing issues is sometimes more important than fixing bugs.

All in all, and though the post is longer than usual, we have just begun with the subject. Have you used **Session Based Exploratory Testing** before? If so, what experiences have you had with it? How are you using it? How did you manage to introduce it in your project/company?

As usual, we would like knowing your opinions, and having your feedback on the matter, so step right up and let us know about you :)
