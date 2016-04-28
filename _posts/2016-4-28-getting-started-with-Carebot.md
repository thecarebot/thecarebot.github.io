---
layout: post
title: Getting started with Carebot
date: 2016-04-28 11:00:00 -0400
---

You've looked into your newsrooms needs, identified a scope, captured objectives, and brainstormed what measures can help you address them. You are ready to [jump in](#setup).

## How it works

Carebot is made up of two parts: an event tracker and a notifications component. 

The tracker is added to the pages on your site and captures specific events (like the user scrolling down a page), which are sent to Google Analytics. Carebot can be extended to capture events elsewhere, but GA was a good simplifyng assumption for the purposes of our initial prototype (and a very commonly used analytics platforms across newsrooms). 

While you can use Google Analytics reports to access your tracked metrics, we added a notification method so that the relevant insights can come to you instead. This is where Carebot helps makes data more in sync with the workflow of journalists. 

Notifications could be broadcast by any method — a text message, an email, Twitter, etc. We chose Slack for this prototype as it has become more widely adopted and also offered us the opportunity to build in querying functions (more later).

Carebot identifies the source of stories (how it knows you published something new) and alerts you that it has started tracking. It then provides you an update every 4 hours and twice daily for the next 2 days with the latest data.

Carebot can also start tracking ad-hoc stories you request and give you on-demand updates as you need. See [Handy Commands](https://github.com/thecarebot/carebot/#handy-commands) for more.

### Carebot In Action

Here are some examples of Carebot in use with the [NPR Visuals](http://twitter.com/nprviz) Graphics team, who are interested in tracking linger rate on graphics and scroll depth within stories that contain graphics they produce.

Carebot notices a new story is published

![Carebot starts tracking](/images/getting-started-example-msg1.png "Carebot starts tracking")

Carebot fetches the latest on a story with two graphics, by request

![Carebot gets latests by request](/images/getting-started-example-msg2.png "Carebot gets latest by request")

Carebot fetches update on a specific graphic, by request

![Carebot gets latests on graphic by request](/images/getting-started-example-msg3.png "Carebot gets latest on graphic by request")

Carebot's final update on a story it has tracked for 3 days

![Carebot final update](/images/getting-started-example-msg4.png "Carebot final update!")

Carebot fetches update on what's happened over the last 7 days, by request

![Carebot gets latests on last 7 days by request](/images/getting-started-example-msg5.png "Carebot gets latest on last 7 days by request")



## Setup

Carebot can be up and running in less than an hour. This presumes you already have a Google Analytics and Slack accounts, and that you are simply adopting the defaults metrics "as-is". 

If you don't have this in place, the instructions below walk you through step-by-step.

To get Carebot up and running you will need to:

1. Add the [Carebot Tracker](https://github.com/thecarebot/carebot-tracker) to your content.

2. Set up the [Carebot Slackbot](https://github.com/thecarebot/carebot) to report data through notifications.

**That's it.**

You likelly have different systems you also want to integrate with and your own metrics to develop on top of Carebot. Instructions for these are also covered in the tracker documentation.

Note that you will be working on very granular and specific aspects of how the analytics are implemented; deeper technical expertise (comfort with JavaScript and the DOM, creating and using AWS S3 buckets, etc), and familiarity with the technologies used (Google Analytics custom events, Slack API, etc) are highly desirable/necessary.

## Detailed Instructions

These instructions you are starting from scratch and have little technical expertise.

1) Sign up for a free Google Analytics account

Once you have a working [Google Analytics](http://analytics.google.com) account, add the provided tracking code to your website (Google Analytics offers [step-by-step instructions](https://support.google.com/analytics/answer/1008015?hl=en&ref_topic=3544906) if you require more detail). 

2) Sign up for a cloud storage service

Any service which allows you to programmatically read and write files to is fine. If you don’t know which one to use, sign up for a free [Amazon Web Services](https://aws.amazon.com/s3) account. Once you have a working account, create an S3 bucket (Amazon Web Services offers [step-by-step instructions](https://docs.aws.amazon.com/AmazonS3/latest/gsg/SigningUpforS3.html) if you require more detail). 

3) Create a new [Slack](http://slack.com/create) team for your organization.  

Once you have an active team, [create a new channel](https://get.slack.help/hc/en-us/articles/201402297-Creating-a-channel). The value of a notification system that offers insights about story performance is largely due to how well it integrates with a team’s workflow. You can make a private channel and name it #carebot for testing purposes, to keep notifications separate, but you should implement carebot in whatever channel your team will be using over the course of their normal workday. 

4) Add the [Carebot Tracker](https://github.com/thecarebot/carebot-tracker) to your content.

From the command line, 

    git clone https://github.com/thecarebot/carebot-tracker

Node.js users can add Carebot tracker to their projects with npm

    npm install carebot-tracker

Follow the instructions in the [tracker documentation](https://github.com/thecarebot/carebot-tracker). Notice you will need to check the HTML of your content and identify CSS ID for the HTML element that contains the content of your story.

Note: It will usually take about 4 hours for traffic data to start showing on your dashboard in Google Analytics. Verify the events you are seeing on your dashboard look as expected.

5) Set up the [Carebot Slackbot](https://github.com/thecarebot/carebot/#bootstrap-the-project) to report data through notifications.

You will use information for prior steps to set this up. Follow the slackbot documentation to create a bot user in Slack and authorize the API use as well as Google Analytics API access. This will ensure that the data can flow from the tracker to GA and to your Slack channel via the Carebot bot user.

The directions will also help you set up how Carebot should become aware of your new stories. It can source a variety of formats (spreadsheets, RSS, etc) and you can easily extend it to include new ones.

Note: The screenshot tool is a handy add-on that will show you a thumbnail of your story next to the page depth measure when it is reported to you in Slack. 

6) Deploy Carebot and start using

Once you are all setup, Carebot will look for the source of stories you defined and alert you that is has started tracking them with a notificaiton in Slack. As time passes you will see periodic updates about all stories and some related graphics to give context to certain metrics.

**Enjoy!**
