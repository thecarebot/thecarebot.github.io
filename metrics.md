---
layout: page
title: Carebot Metrics
permalink: /metrics/
---
 
* [Introduction](#introduction)
* [Metrics, Measures and Indicators](#metrics-measures-and-indicators)
* [Definitions](#definitions)

## Introduction

Seeking more meaningful ways to assess success in journalism has led us to explore different metrics and approaches to understanding how people come to care about stories they encounter. This document captures what these metrics are, why we chose them, and how we are using them.

## Metrics, Measures and Indicators

First, let's be clear about what we mean by the terms we use. 

**Metrics** represent the different methods we employ to understand change over time across a number of dimensions or criteria. It is often used as a catch-all term to describe the method used to measure something, the resulting values obtained from measuring, as well as a calculated or combined set of measures. 

We use the term **measures** when we mean the value measured by whatever mechanism we employ and the term **indicator** for values we combine and use to hint to specific outcomes and trends.

Note: All measures and indicators reflect events that occured in a specific period of time. When representing these values (specially when aggregating them), indicate the period of time it relates to. 

### Measures

A **measure** is a number or a quantity that records a directly observable value or performance. All measures are composed of a value (a number) and a unit of measure. The number provides magnitude for the measure (how much), while the unit gives number meaning (what is measured).

* 1,234,567 Pageviews
* 8,901,234 Sessions
* 567,890 Facebook Likes

#### Pitfalls

When comparing measures that are tracked by two different systems (for example, the number of daily sessions on your site versus the number of daily sessions on your competitor's site), ensure that the units are consistent between both. It is not uncommon for a measure of the same name to mean different things; consult the documentation that defines each measure for that system.

Even when the same system is used, there might still be differences. For example, a `session`
in Google Analytics is defined as "A group of interactions that take place on a site within a given time frame." It is set to 30 minutes by default, but this setting can be changed. 

If, for example, you are comparing session lenght for stories with long-form video, you will likelly adjust the defaul 30 minutes to a longer period to avoid timing out user sessions while they are still watching and possibly miscounting the total number of sessions. If you do so, comparing sessions-related behaviors with another site that uses the 30 minute default may be a misleading comparison.


### Indicators

An **indicator** is a qualitative or quantitative factor or variable that provides a simple and reliable mean to express achievement, the attainment of a goal, or the results stemming from a specific change. It often aggregates or combines multiple measures in an explicit formula.

* 1M weekly active users
* 1:3 users complete the story
* 23% homepage bounce rate

#### Pitfalls

All indicators are relative to a set of measures in a particular context. For an indicator to be meaningful, it should always be contextualized with the scope of stories being assesed and the measures used to calculate should be made explicit. 

It is very easy to get indicators wrong because they can obscure a lot of information and complexity with the deceivingly simple guise of a single value.

**1. Indicators are always relative to a context**

*1:3 users complete the story* sounds as concrete and tangible as any other measure but the unit is not self-evident. There is no tangible `read-story` unit that can be tracked and counted. This abstraction forces introspection and requires a definitional understanding of all its parts.

[What is a story?](https://thecarebot.github.io/what-kinds-of-stories-can-you-tell/) Is a text-based 2000-word page-scroll experience and an auto-advancing photo essay with an audio track both considered stories? Can they be compared? Should they be compared? Are they compared in this '1:3 users complete the story' indicator?

While the answers may be yes, due to their inherent technical format difference they can't actually be tracked in the same way. This is where the diversity of story forms in journalism makes analytics trickier than more simplistic ecommerce analytics, which are consistently transactional.

What measures are being used for each type? A video or audio piece may aggregate the total time played over media duration, whereas for an interactive graphic could take the total time the user spent viewing the graphic relative to an arbitrary ideal period of time. These are other examples of items that may be considered "stories" in a specific context.

**2. Indicators can be simplifying to a fault**

Indicators obfuscate in order to clarify. By reliably providing just one method to observe change of a particular aspect over time and thus understand its performance, even if it is fairly complex or complicated, indicators help make the complex clear. 

They accomplishe this by obfuscating the details, rationales and definitions — in our example, the different ways in which it obtains the same metrics for different story forms, tracked by different means, and calculates a single number.

Obfuscating too much renders the indicator less clear because it hides some of that necessary context, so important to give meaning to the insight. Finding the right balance of offering useful insights while not overwhelming the user is a big challenge for meaningful analytics.

**3. Indicators force value judgments**

Numbers are agnostic. People attribute positive or negative meaning to numbers depending on the context in which they are used. Additionally, were averages, medians or total values of aggregated measures used? Each may give you a significantly different read on your data. This is further emphasized when indicators are presented in comparative terms such as relative to a specific goal or relative to existing benchmarks.

*Bounce rate* is an indicator used to describe the [percentage of single-page sessions](https://support.google.com/analytics/answer/1009409?hl=en), meaning the sessions in which the person left the site from the same page they entered without interacting with the page. Is this good or bad? It can be bad if that page is the starting point of an interactive story and the expected next step was for the user to hit play and start navigating through the story. It is good if that was your contact page and people came to get your phone number or address.

Scrutinizing what the indicator means, what it attempts to represent, how it is calculated is a healthy way to uncover measurementment problems.


### Definitions

For each definition below we attempted to:

1. Articulate what each metric means so it can be understood independently.
2. Frame the definition for what the metric does for the user of analytics data.
3. Avoid explaining a metric by using other metrics (as much as possible).
4. Make the distinction between metrics clear in each definition.

*** 

#### Measures

**Attempted Graphic Interaction** is a measure used to count how many times a user tried to interact with a graphic by clicking, tapping or dragging.

**Graphic On-screen Visibility** is a measure used to count how much time a graphic is displayed on their browser’s viewport while the page is visible to the user.

**Pageview** is a measure used to count each time a page for a corresponding URL was loaded on the user’s browser.

**Story Scroll Depth** is a measure used to track how far down a one-page story a user has scrolled before leaving.

#### Indicators

**Graphic Linger Rate** is an indicator used to calculate the median visibility of a graphic across all users who viewed it.

**Never Seen (Graphic)** is an indicator used to calculate the number of potential readers of a story who never saw the graphic in that story.

**Veni, Vidi, Relīquī** is an indicator used to calculate the number of times users loaded the page for a corresponding URL then promptly abandoned it.

**Engaged Completion Rate** is an indicator used to calculate the proportion of people who started and completed the story.

**Comparable Facebook Sharing** is an indicator used to calculate the relative impact of Facebook Shares for every 1000 user sessions a story receives.


***

#OLD NOTES TO BE CLEANED UP:

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
