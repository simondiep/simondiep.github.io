---
layout: post
title: "Showcase your code"
date: 2018-09-25 11:50:00 -0500
categories:
  - thoughts
  - tech
---

It's been difficult for me to remember and summarize all of my personal projects. Something that's helped a lot recently has been Github. By posting all of my projects onto Github and leveraging their free website hosting in Github Pages, I'm able to share my code and live demos.

Steps to enable a live demo of your Github Repo

- Click Options
- Scroll Down to the GitHub Pages section
- Change Source Dropdown from None to master
- Click Save

Goals accomplished:

- Be able to access my projects from any computer
- Allow anyone to learn from my code
- Allow anyone to leverage my code to solve their own problems
- Easily set up live demos of code

The next problem I wanted to solve was how to consolidate all of those projects into a single web-page, sort of like a showcase for those that didn't have time to click through all of my projects. I first looked around to see if anyone else has done this. To my surprise, no. That's when I created a [web app](https://github.com/simondiep/github-project-showcase) to showcase my Github projects. I started off with [create-react-app](https://github.com/facebook/create-react-app) knowing that I needed to make a request to the Github API to get repository information. It turned out well, and scales well, such that whenever I create a new repo, it will automatically show up in the showcase app. It is also very easy for anyone else to start using, as you can easily swap the Github username to your own.

In summary, Github Pages is a super-convenient way to provide live demos of Github projects. By leveraging Github Pages, I was able to create [Github Project Showcase](https://github.com/simondiep/github-project-showcase) for anyone to show off their Github projects in a concise and visually appealing manner.
