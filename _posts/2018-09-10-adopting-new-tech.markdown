---
layout: post
title:  "Adopting new technologies and tools"
date:   2018-09-10 12:59:00 -0500
categories:
 - thoughts
 - tech
---

As I have adopted more and more technologies into day-to-day life, I've realized a common trend.

1. I need a tool to solve a specific problem for me
2. Search around for top recommended tools
3. Try out tools
4. Give up or pick the tool

When trying out tools, I definitely value tools that I can get up and running quickly, as in a minute or two.  If I have to read and follow a 30min guide on how to set up your tool, I'm not going to use it.

# Unsponsored rant about webtask.io

A recent tool I've had the pleasure of using is webtask.io.  It allows you to create a **free** public hosted API in under a minute, which is unheard of!  When I first heard webtask at a MidwestJS conference talk, I went to the website, logged in, and immediately started coding without any documentation.  The template app provides all the info you need.  It is designed very similarly to a familiar tool I'm more accustomed to: AWS Lambda.

What astounded me the most about webtask is that they provide storage for your API.  This was exactly what I was looking for, for my [space-shooter game](https://github.com/simondiep/space-shooter), as I needed a way to keep track of high-scores.  **I kept deferring this feature, since I didn't want to invest the time to learn a bunch of tools by watching tutorial videos on Pluralsight, then have to pay for web hosting.**  Having implemented this similarly on the AWS tech stack (API Gateway, Lambda, DynamoDB) was really time-consuming with a lot of trial-and-error, and was not free to host.

Later after implementing high-scores into my game within a few hours using webtask, I stumbled across a related [Youtube video](https://www.youtube.com/watch?v=_OTUGVAEWCA) of two developers who try to build a random app within an hour, just for fun and learning.  Seeing them struggle and fail to get a new tool, Firebase, working within the hour was a bit frustrating.  If they had known about webtask, they could've built the app they wanted within the time limit.

# Takeaways

Remembering how I felt as I adopt new tools, I incorporate these learnings to make a more enjoyable tool to try out.

## My Guidelines for building a new tool 

1. Clearly **define the objective** of the tool and list some of the more common use cases.  List who is the intended primary audience.
2. Prefer **no prerequisites or dependencies** to using the tool, such as not caring if you are on Windows or have Java installed.
3. An interested person could get the tool **running extremely quickly**.
4. Minimal hand-holding.  The tool should be designed in a way that is **intuitive** and does not have very wordy docs for beginners.  More detailed docs are still great for those who want to perform more complex actions.

