---
layout: post
title: Whither Pageviews? ¯\_(ツ)_/¯ 
date: 2016-04-30 11:00:00 -0400
---

*Pageviews* are a pervasive newsroom metric inherited from advertising-based analytics. As we think of more appropriate metrics for journalism, what place do pageviews have in the newsroom seeking more meaningful analytics?

## The problem with pageviews

Pageviews are a simple [measure](https://thecarebot.github.io/metrics-measures-and-indicators/#measures). It counts each time a page for a corresponding URL was loaded on the user’s browser.

When a page loads, all content in it is rendered on the browser, including ads, which makes this measure helpful for advertisers to understand how many opportunities they had for their ad to be loaded for the user's benefit.

You can also measure how many times an ad was clicked on, but you can't measure whether or not an ad was read, and understood, or what subsequent impact it might have had on the user. So, pageviews are a proxy measure used by advertisers to approximate how many people might have possibly seen an ad and then make presumptions about its impact outside having clicking on it.

#### How does that translate to journalism? 

In journalism pageviews still only count URLs loaded. And here is the danger: how a user may or may not have interacted with and or responded to a story shown on that URL is in no way demonstrable by the pageview measure. The implied "view" in "pageview" is not true[*](#footnote).

In short, pageviews:
1. Express intent (desire for content), not goal attainment (evidence of using the content).
2. Encourage comparison between stories based on general interest not performance of the story itself.
3. Do not reveal anything about made a story successful or not.

Instead of trying to further scrutinize pageviews (they don't need scrutiny because they are simply not useful to understand behavior), we turned our focus to the newsroom behavior: if everyone across the newsroom is going to continue coming after pageview information, how can we satisfy this expectation without offering the "empty insight" that this weak metric brings? **How can we offer what they want but give them what they need?** 

## Unsucking Pageview Ideas

Quick ideas and notes on how pageviews can express more useful information about a story: 

### Compare the total pageview count on a story to all traffic to site within 24h/1w

Instead of showing the raw measure, create a relative indicator that notes how a story is doing compared to what's been published in the last 7 days. This should help express magnitude: is this story attracting different traffic than what has been typical this week? More of a *smoke test* ("is someting wrong?" indicator) than a performance assessment, but possibly useful. It would be best to break down stories that got promoted on Facebook and Twitter versus stories that were not).

Usefulness potential: medium/low (but still better than raw pageviews)

### Compare ranking of story completion rate to ranking of pageview count on a story.

This could reveal how a high pageview number may conceal a poor performing story with users. The idea is to pair pageviews with a more useful metric (available on [Carebot tracker](https://github.com/thecarebot/carebot-tracker)) so pageview is never seen in isolation and so that it's not ranked on volume but relative performance.

Usefulness potential: high

### Compare the total pageview count on a story to the mean of all stories to date.

An approach that forces comparison to corpus of stories rather than most recent stories (which are not a particularly useful reference because there is nothing inherently comparable). This would be most useful if it could be visualy represented showing the overall distribution histogram so one could quickly assess where a story stand among others and what is "normal". 

Usefulness potential: medium

### Compare the total pageview count on a story to quartiles of all stories to date.

Like the above idea, forces comparison to corpus of stories in context of normal distribution, developing a shared understanding of what high/low/average performance means for a team. This could help quick assessment (simple classification into these buckets), rather than giving attention to the exact number, which doesn't offer any additional insight. Additional benefit of training people out of looking at pageviews.

Usefulness potential: medium /high

### Compare the total pageview count on a story to ‘throw-away pageviews’.

A pageview



(aka, pageviews that lasted under 3 seconds and there was no user interaction on the page)

How it expresses more useful info about a story:
Provides evidence of how much of pageviews are not indicative of engagement

Usefulness potential: high

### Compare total pageview count on a story to like-stories only

(applicable for all the above - helps tighten the focus and make the other aspects more meaningful because the comparable universe becomes more uniform)

How it expresses more useful info about a story:
Doesn’t affect perception of pageviews and its use

Usefulness potential: neutral - thought I suppose it discourages apples-and-oranges comparisons


### Compare current pageview to projected pageviews for that story




#### \* Terminology Footnote

I was unable to find the precise articulation of how the term pageview came about, but aside from the implicit assumption that a user "viewed" the content of a page simply because the URL was loaded, it is possible the term has a technical history since the word view, possibly short for viewport, is used to discuss the conceptual place the browser is rendering pixels on the screen. This would make pageviews technicaly accurate and precise in its definition of counting how many times the URL rendered the page in the browser, but no more useful for our purposes.

---

— [Livia Labate](http://twitter.com/livlab)



