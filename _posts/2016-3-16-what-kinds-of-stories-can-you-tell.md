---
layout: post
title: What kinds of stories can you tell?
---

> "Organizing is what you do before you do something, so that when you do it, it is not all mixed up."
—A. A. Milne

There is no wrong way to categorize stories. There are, however, many right ways. When comparing performance across stories, newsroom users want to compare like stories, apples to apples. 

Comparing measures to broad averages across story types dilutes the insight and often obscures what is distinct about a specific story and its performance, so the classification system has the potential to impact the quality of the analytics used.

After we narrowed it down to **story** as [Carebot's subject of analysis](https://thecarebot.github.io/What-are-we-measuring-when-we-measure-journalism/), we started the real hard work, which is to define what is comparable and what is not; how to classify a story. 

I had interviewed several people at NPR about their interest in story analytics so I went back to the transcripts and looked for questions that were specific to a kind of story or unique to a particular of the storytelling approach — "how many comments mentioned the graphic?" and "did anyone mute the audio-driven slideshow?" are two examples that come to mind. 

I also pulled a random sample of NPR stories from the last 6 months and went through them, exploring the ways in which they were similar, like [Life After Death](http://apps.npr.org/life-after-death/) and [The Bus Station](http://apps.npr.org/lookatthis/posts/bus-station), and the ways in which they were distinct, like [Can't Go Home](http://apps.npr.org/syria/)
 and [Drowned Out](http://apps.npr.org/lookatthis/posts/whales).

This is the approach I generally take when making a content inventory; take a sample of content and explore it to generate the facets I'll use to classify all the content I'll eventually cover. This proved to be a useful method to show that a simple hirarchy is a poor way to think about storytelling approaches because the commonalities and differences may be granular AND overarching.

A multi-faceted taxonomy allow us to compare relevant things among very different stories and still find meaningful insights. In short, this taxonomy creates **a set of simplifying assumptions so that story measures and indicators can be compared to those of stories most like them.**

**Note:** This taxonomy reflects the realities of the NPR Visuals teams and the nature of stories told by this team, grounded in interviews with team members. The set accommodates further expansion with a variety of types and expressions should the scope of comparisons increase.

---

### Facet 1: Dominant Media
What media is most central to the storytelling (not just what there is more of)

#### Values
* Text (default)
* Graphics (charts, data tables or maps)
* Photography or illustration
* Animation/loops
* Audio
* Video

---

### Facet 2: Pacing
Who drives the storytelling rhythm during viewing

#### Values
* Self-paced: the story progresses according to continuous user interaction. (default)
* Auto-advance: the story progresses on its own after user's first interaction.

---

### Facet 3: Project Type
The nature of the storytelling device, from the user's perspective.

#### Values
* Story: user is informed through exposition of facts and opinions. (default)
* Lookup tool: user retrieves information from a dataset by selecting/inputing filtering choices.
* Quiz: user selects/inputs answers to a series of questions that are computed for a resulting score or conclusion.
* Playlist: user receives an organized sequence of media 

---

### Facet 4: Interaction Model
The method by which the user navigates the story.

#### Values
* Scroll: scan down a page containing various media. (This is the most common case)
* Playback: Start an audio or video-driven narrative.
* Advance: Click or tap through a sequence of assets (slides, screens, photos in a gallery, etc).

---

We can add new facets until the cows go home. My main objective is to have the minimum amount of categories to make meaningful distinctions, so we don't add any more than we need. In fact, the design approach is "take it away until it breaks, then add it back". And to the extent that it made sense, I tried to frame each facet from the perspective of the user and how the user interacts with the story, in alignment with our scope of interest.

Before all this, the first iterations of Carebot had a tagging system intended for the same purpose but was really a [folksonomy](http://vanderwal.net/folksonomy.html), not so much categorizing as giving the item some meaning, like "books" because it was a project about books. 

![Vintage Carebot's tags](/images/carebot-vintage-tags.png "Vintage Carebot tags")

We didn't really take advantage of that for analysis, though there was a method to query certain metrics for stories that matched a particular tag (sadly, I have no sample data or screenshots of the results):

![Vintage Carebot's query](/images/carebot-vintage-query.png "Vintage Carebot query")

A common problem with tagging is conflating the technology and the concept. The ability to tag is wonderful. It is free form and generative (I might even use it to implement this taxonomy), but the goal and intentions of the classification system depend on what you are trying to do, with the boundaries of the content space you are working with. 

In our case, our boundaries are stories produced by NPR Visuals. However Carebot gets implemented, it would be important for those adopting it to determine if the taxonomy matches their own stories or if they need different classes and definitions.

We are currently building a Carebot implementation that is focused on graphics stories, so we haven't yet broadened the scope of stories broadly enough that we need this classification system yet, but when we get there, we have this frame of reference to explore and see if it offers a sufficient level of granularity to distinguish stories withouth becoming overlwhelming and/or creating additional work for newsrooms to classify stories.


— [Livia Labate](http://twitter.com/livlab)
