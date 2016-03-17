---
layout: page
title: Carebot Metrics
permalink: /metrics/
---

* [Introduction](#introduction)
* [Measures and Indicators](#measures-and-indicators)
* [Carebot Measures](#carebot-measures)
* [Carebot Indicators](#carebot-indicators)

## Introduction

Seeking more meaningful ways to assess success in journalism has led us to explore different metrics and approaches to understanding how people come to care about stories they encounter. This document captures what these metrics are, why we chose them, and how we are using them.

## Measures and Indicators

First, let's be clear about what we mean by metrics. Metrics are a catch-all term used to represent the different methods we employ to understand change over time across a number of dimensions. They are made up of explicit measures and can be combined to produce indicators, which hint us to specific outcomes and trends.

### Measures

	1,234,567 Pageviews
	8,901,234 Sessions
	567,890 Facebook Likes

A **measure** is a number or a quantity that records a directly observable value or performance. All measures are composed of a value (a number) and a unit of measure. The number provides magnitude for the measure (how much), while the unit gives number meaning (what is measured).

Not all systems used to track measures share the same definition for units with the same name. A session on your site and a session on your competitor's site may be tracked differently. Ensure you are working with the same measure when using different tracking instruments. Examples:

* Pageview: An instance of a user visiting a particular page on a website. User commonly across many systems.
* Sessions: A group of interactions that take place on a site within a given time frame. In Google Analytics, a sessions is set to 30 minutes by default, but this can be changed.
* Facebook Likes: Number of times the Like link was cliked on in a Facebook post.

All measures are counts of a particular unit over a period of time. For a measure to be meaningful, it should always be contextualized with the period of time that it relates to. 

### Indicators
An **indicator** is a qualitative or quantitative factor or variable that provides a simple and reliable means to measure achievement; the attainment of a goal, changes resulting from a specific intervention, etc. It aggregates or combines multiple measures in an explicit formula.

For example, a *75% Completion Rate*. This indicator is defined differently based on the presentation of a story - in a video or audio piece it is the aggregation of total time played over video duration whereas for an interactive graphic it could be time spent viewing the graphic relative to an arbitrary ideal period of time.

All indicators are relative to a set of measures in a particular context. For an indicator to be meaningful, it should always be contextualized with the scope of stories being assesed and the measures used to calculate should be made explicit. 

It is very easy to get indicators wrong because they can obscure a lot of information and complexity with the deceivingly simple guise of a single value.

## Carebot Measures and Indicators

Here's what we have explored so far. Note: This part of the document changes frequently.

#### Measure: Graphic On-screen Visibility 
How much time a user views a graphic on their screen.

How it works
* time is counted in seconds
* time is captured in 10sec increments up to a minute, then 1min increments up to 5minutes then in 5min increments.
* views under 10 seconds are discarded (considered a bounce).
* screen is equivalent to the user's browser viewport.
* if the user leaves window innactive and returns, the count continues.
* if the user closes the window and opens again, the count re-starts.

Reporting
* Reported as a median value for all users of a graphic.
* Shown as a distribution to contextualize median.
* Used to calculate Graphic Linger Rate.

#### Measure: Scroll depth across a story
How far down the length of a story a user scrolled.

[coming soon]

#### Indicator: Graphic Linger Rate
The median visibility of a graphic across all users who viewed it.

[coming soon]

#### Indicator: Engaged Completion Rate
Percentage of people who start and complete the story.

[coming soon]

#### Indicator: Comparable Facebook Sharing
Number of Facebook shares per 1000 user sessions.

[coming soon]
