---
layout: page
title: Carebot Metrics
permalink: /metrics/
---
 
## Introduction

Seeking more meaningful ways to assess success in journalism has led us to explore different metrics and approaches to understanding how people come to care about stories they encounter. 

This document captures what these metrics are and their definitions, used as references for all Carebot outputs. We would be remiss if we didn't make it explicitly clear the distinctions we are making between [Metrics, Measures and Indicators](https://thecarebot.github.io/metrics-measures-and-indicators/) and why---these assumptions drive our framing for the definitions below.

### Definitions

<!--

For each definition below we attempted to:

1. Articulate what each metric means so it can be understood independently.
2. Frame the definition for what the metric does for the user of analytics data.
3. Avoid explaining a metric by using other metrics (as much as possible).
4. Make the distinction between metrics clear in each definition.

-->

#### Measures

* *Attempted Graphic Interaction* is a measure used to count how many times a user tried to interact with a graphic by clicking, tapping or dragging.

* *Graphic On-screen Visibility* is a measure used to count how much time a graphic is displayed on their browser’s viewport while the page is visible to the user.

* *Pageview* is a measure used to count each time a page for a corresponding URL was loaded on the user’s browser.

* *Story Scroll Depth* is a measure used to track how far down a one-page story a user has scrolled before leaving.

* *Story Rebirth* is a measure used to track how many users returned to a story and completed reading it after having abandoned a tab open after loading the story.

#### Indicators

* *Graphic Linger Rate* is an indicator used to calculate the median visibility of a graphic across all users who viewed it.

* *Never Seen (Graphic)* is an indicator used to calculate the number of potential readers of a story who never saw the graphic in that story.

* *Veni, Vidi, Relīquī* (*I came, I saw, I abandoned*) is an indicator used to calculate the number of times users loaded the page for a corresponding URL then promptly abandoned it.

* *Engaged Completion Rate* is an indicator used to calculate the proportion of people who started and completed the story.

* *Relative Facebook Sharing* is an indicator used to calculate the relative impact of Facebook Shares for every 1000 user sessions a story receives.

#### Other

Neither measures nor indicators, but related considerations:

* [The Care Question](http://blog.apps.npr.org/2015/02/26/multivariate-testing.html) is a Y/N question presented to users at the end of a story to assess if it satisfied their needs. Live tests have shown that having this question present at the end of a story significantly increased users likellyhood to take a subsequent action (share, like, contribute, etc)


<!--

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

-->
