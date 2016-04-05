---
layout: page
title: Carebot Metrics
permalink: /metrics/
---
 
* [Introduction](#introduction)
* [Measures and Indicators](#measures-and-indicators)
* [Definitions](#definitions)

## Introduction

Seeking more meaningful ways to assess success in journalism has led us to explore different metrics and approaches to understanding how people come to care about stories they encounter. This document captures what these metrics are, why we chose them, and how we are using them.

## Metrics, Measures and Indicators

First, let's be clear about what we mean by the terms we use. 

**Metrics** represent the different methods we employ to understand change over time across a number of dimensions or criteria. It is often used as a catch-all term to describe the method used to measure something, the resulting values obtained from measuring, and often (misleadingly) a calculated or combined set of measures. 

For clarity, we use the term **measures** when we mean the value measured by whatever mechanism we employ and the term **indicator** for values we combine and use to hint to specific outcomes and trends.

Note: All measures and indicators reflect events that occured in a specific period of time. When representing these values (specially when aggregating them), indicate the period of time it relates to. 

### Measures

A **measure** is a number or a quantity that records a directly observable value or performance. All measures are composed of a value (a number) and a unit of measure. The number provides magnitude for the measure (how much), while the unit gives number meaning (what is measured).

  1,234,567 Pageviews
  8,901,234 Sessions
  567,890 Facebook Likes

#### Pitfalls

When comparing measures that are tracked by two different systems (for example, the number of daily sessions on your site versus the number of daily sessions on your competitor's site), ensure that the units are consistent between both. It is not uncommon for a measure of the same name to mean different things; consult the documentation that defines each measure for that system.

Even when the same system is used, there might still be differences. For example, a `session`
in Google Analytics is defined as "A group of interactions that take place on a site within a given time frame." It is set to 30 minutes by default, but this setting can be changed. 

If, for example, you are comparing session lenght for stories with long-form video, you will likelly adjust the defaul 30 minutes to a longer period to avoid timing out user sessions while they are still watching and possibly miscounting the total number of sessions. If you do so, comparing sessions-related behaviors with another site that uses the 30 minute default may be a misleading comparison.

### Indicators

An **indicator** is a qualitative or quantitative factor or variable that provides a simple and reliable means to measure achievement; the attainment of a goal, changes resulting from a specific intervention, etc. It aggregates or combines multiple measures in an explicit formula.

For example, a *75% Completion Rate*. This indicator is defined differently based on the presentation of a story - in a video or audio piece it is the aggregation of total time played over video duration whereas for an interactive graphic it could be time spent viewing the graphic relative to an arbitrary ideal period of time.

All indicators are relative to a set of measures in a particular context. For an indicator to be meaningful, it should always be contextualized with the scope of stories being assesed and the measures used to calculate should be made explicit. 

It is very easy to get indicators wrong because they can obscure a lot of information and complexity with the deceivingly simple guise of a single value.

### Definitions

Here's what we have explored so far. Note: This part of the document changes frequently.

#### Measure: Graphic On-screen Visibility 
How much time a user views a graphic on their screen.

##### Question it answers
How much time do people look at a graphic when reading a story?

##### How it works
  * time is counted in seconds
  * time is captured in 10sec increments up to a minute, then 1min increments up to 5minutes then in 5min increments.
  * views under 10 seconds are discarded (considered a bounce).
  * screen is equivalent to the user's browser viewport.
  * if the user leaves window innactive and returns, the count continues.
  * if the user closes the window and opens again, the count re-starts.

##### Reporting
  * Reported as a median value for all users of a graphic.
  * Shown as a distribution to contextualize median.
  * Used to calculate Graphic Linger Rate.

#### Measure: Scroll depth
How far down the length of a story a user scrolled.

[coming soon]

#### Indicator: Graphic Linger Rate
The median visibility of a graphic across all users who viewed it.

[coming soon]

#### Indicator: Engaged Completion Rate
Percentage of people who start and complete the story.

##### Question it answers
Of the people who started, how many finished? 

##### How it works
[Engaged User Completion Rate](http://blog.apps.npr.org/2015/11/19/sequential-visual-stories.html)

##### Reporting

[coming soon]

#### Indicator: Comparable Facebook Sharing
Number of Facebook shares per 1000 user sessions.

[coming soon]

***

old notes from wiki:

# What does the "care" in Carebot mean? 

- How much people care about a piece? 
- If we made people care? (a change in care level)

# Metrics that track care

## Linger Rate

"People looked at your graphic for an average of 5 minutes" 

## Total Linger Time

"People spent 50 hours looking at your graphics today!"

Probably not a good metric because it's a proxy for pageviews (1,000,000 10-second views is a lot more time than 

## Interaction Rate

"50% of people [played audio]

## Completion Rate

Did someone get all the way through the piece? 

## [Engaged User Completion Rate](http://blog.apps.npr.org/2015/11/19/sequential-visual-stories.html)

Of the people who started, how many finished? 

## [Read Time / Total Time Reading](https://medium.com/data-lab/mediums-metric-that-matters-total-time-reading-86c4970837d5#.otwa46ny7)

> Read time is based on the average reading speed of an adult (roughly 275 WPM). We take the total word count of a post and translate it into minutes. Then, we add 12 seconds for each inline image. Boom, read time.

## Social Media

### Shares, Retweets 

### Replies

Did people actually have a discussion about the piece, or was it only shared outbound? 

### Social Circles

Hard to measure. BUT what if we could know things like "This article resonated among young Russian chess players, who shared it more than any other social cluster"? 

### Sampling messages

Rather than _volume_ of messages, where there any exceptional shares or responses? Messages that got more shares, retweets, or replies? What does a sampling of responses look like? (Give people actual examples of the text people wrote in response) 

#### Other

##### Indicator: Never seen
Number of people who never even saw the graphic

unique sessions for story - (sum of all sessions with graphics on screen visibilty over 10 seconds)

Could also be Graphic On-screen visibility under n seconds (figuring out n seems very random).
