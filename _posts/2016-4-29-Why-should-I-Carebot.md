---
layout: post
title: Why should I Carebot?
date: 2016-04-29 11:00:00 -0400
---

Because *what gets measured gets done* [*](#footnote).

The metrics you choose---and the ways you choose to communicate them---drive people to action. Analytics have the power to change behavior. To push your team to embrace different types of storytelling. To encourage reporters to think about some audiences more than others. To help managers make the hard choices of what to staff. 

And this can all go horribly wrong. If your metrics do not align with your goals, you’ll push your organization in the wrong directions, to make poor choices. What you celebrate must reinforce your goals.

You must be extremely intentional.

The analytics platforms we have, like Google Analytics, were created with the interests of online advertising in mind. A pageview is a good measure of success for display advertising, but it’s  a poor measure of whether you’ve served your audience.  

And they’re generally implemented company-wide. This top-down approach gives the whole newsroom the same set of metrics and reports, irrespective of story objectives, audience or storytelling approach. 

Once you understand that the available metrics aren’t really a good measure of your mission, maybe [you’d want to keep this kind of data out of the newsroom](https://medium.com/thoughts-on-journalism/metrics-and-the-media-we-can-measure-it-but-can-we-manage-it-3349cb9a9050). However, in an age where storytelling approaches (specially on the web), are rapidly changing in response to audience [expectations](https://medium.com/@chrismoranuk/the-shocking-truth-about-audience-data-it-will-surprise-you-44a90431671b), technological [innovation](https://live.fb.com/), and shaped by the story itself, we \***do**\* need ways to measure the success of our work! 

**It is unrealistic for a news organization to expect or demand newsroom alignment without giving teams the tools needed to make good decisions.**

We started the Carebot project to seek out alternative analytics for journalism. Our effort has been two-fold.  We’ve examined and invented 1) measures and indicators of story success, and 2) methods for communicating them in the newsroom. 

The relevance and effectiveness of any performance assessment is relative to the circumstances and needs of the newsroom and its journalists at a particular point in time. While there is no one metric capable of measuring journalism as a whole, it is possible to **offer meaningful and actionable insights to teams by aligning measurements to objectives and their scope of storytelling**.

## Empowering teams to affect change

We propose flipping the usual top-down approach to a story-driven one. Carebot is a bottom-up analytics system that serves the needs of the journalist and their immediate team. Instead of crunching numbers organization-wide, it’s built to focus on a subset of stories with [similar characteristics](https://thecarebot.github.io/what-kinds-of-stories-can-you-tell/#carebots-story-taxonomy), and deliver numbers to a small group, like a desk---a team with a shared purpose.

By articulating journalistic objectives, audience needs, and by capturing questions and hypotheses about how stories are used, we can identify what to track and offer answers and benchmarks for comparison.

Carebot [tracks](http://github.com/thecarebot/carebot-tracker) measures that existing analytics tools don’t, such as how much time users are spending with an interactive graphic. This project was built as a prototype, in just a few months, so it only tracks a few things. We’re currently working to make it modular, with the hope that it will be relatively easy to add your own metrics. 

Also, most existing analytics systems require the user to visit and manipulate a dashboard to understand story performance. This just doesn’t fit the daily, deadline-based workflow of teams in newsrooms. To effectively communicate success, you’ve got to meet people where they’re at.

So, Carebot takes a public, notification-based approach (currently implemented as a [Slackbot](http://github.com/thecarebot/carebot)). Instead of having to look for analytics, Carebot speaks about story performance in a space where the team gathers---the team’s chat room. Carebot also allows [querying](https://github.com/thecarebot/carebot#handy-commands) of latest updates and summaries of similar stories for comparison.

## A healthier news organization

Creating an open space for the team to collectively monitor story performance encourages conversations and appreciation of effort. Celebrating success in a team gathering space affects morale and broadens the team’s perception of how each member contributes to their shared goals.

The Carebot approach also gives teams the flexibility to iterate their metrics. Teams can adjust measures to fit their needs, and to answer new questions without having to change the entire system for the whole newsroom---and without giving-in to a lowest-common-denominator approach that doesn’t address each team’s unique circumstances.

We hope this will empower teams to [take ownership](https://medium.com/thoughts-on-journalism/metrics-and-the-media-we-can-measure-it-but-can-we-manage-it-3349cb9a9050) of their analytics. Teams can define their own measures of success, and act independently---on how they tell stories, set priorities, and serve their audience.

## Systemic change on a budget

Carebot is [free and open-source](https://github.com/thecarebot/carebot/blob/master/LICENSE.md), so anybody can take it for a spin and modify it to fit their needs. Defining your own metrics requires programming skills, but the current implementation can be  [set up in under an hour](https://thecarebot.github.io/getting-started-with-Carebot/) with existing Google Analytics and Slack accounts (both also free services at the basic level). 

The big investment is in upfront planning. We strongly recommend that teams interested in implementing Carebot start with an exercise. First, determine what to focus on --- a desk, a story type, a beat. And second, clearly articulate objectives, audience and needs. (This, of course, would be a valuable exercise no matter what analytics solution one might adopt!)

We hope you’ll [give Carebot a try](https://thecarebot.github.io/getting-started-with-Carebot/)! (And if you do, we really hope you’ll pitch in! An open-source project is only as healthy as it’s community. We’re just getting warmed up, and every little bit helps!)


---

#### Footnote

This popular proverb has been [attributed to a variety of authors](https://athinkingperson.com/2012/12/02/who-said-what-gets-measured-gets-managed/) with slight variations in different contexts and eras. It was widely popularized by Peter Drucker and his [Management by Objectives](https://en.wikipedia.org/wiki/Management_by_objectives) approach since the mid 1950s and reinforced by Tom Peters’ work in the 80s and 90s.

---

*** 
— [Livia Labate](http://twitter.com/livlab) & [Brian Boyer](http://twitter.com/brianboyer)

