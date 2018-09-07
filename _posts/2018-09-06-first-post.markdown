---
layout: post
title:  "First Post!  Setting up your own blog."
date:   2018-09-06 11:43:00 -0500
categories:
 - how-to
 - jekyll
---

I decided to start a blog today.  I had seen a bunch of blogs hosted with Jekyll on Github pages, so I wanted to try it out.

# New Blog Setup

The [Jekyll Docs](https://jekyllrb.com/docs/) were extremely helpful and easy to follow.

- If you already have Ruby installed
  - `gem install jekyll bundler`
  - `jekyll new simon-blog`
  - `cd myblog`
  - `bundle exec jekyll serve`

This will create and host a template site locally.

I started the server with the command

`bundle exec jekyll serve`

and started adding and editing `.markdown` files to the `_posts` directory.

This will generate html files into `_site`.

# Hosting your blog

To host on github-pages, I followed this [Github guide](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#step-3-optional-generate-jekyll-site-files)

Do note that you will need to use your name.github.io repo for this to work.

# Stumblings

I looked into using a new theme for Jekyll but was unsuccuessful.  Google results showed a lot of nice previews, but it was unclear how to use a theme.

I tried following [this guide](https://github.com/pages-themes/midnight#usage) for a github-pages theme but it seems like the directory structure might be different per theme.

Sticking to the default theme for now.