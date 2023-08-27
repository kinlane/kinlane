---
title: Liquid To Filter Out The Future On My Blogs
date: 2017-05-17 15:00:00 Z
tags:
- Kin Lane
- Jekyll
- Blog
image: https://s3.amazonaws.com/kinlane-productions2/jekyll/jekyll-logo.png
---

<p><img style="padding: 15px;" src="https://s3.amazonaws.com/kinlane-productions2/jekyll/jekyll-logo.png" align="right" width="30%" /></p>
I created a little hack on my Jekyll-driven websites to allow me to publish a week's worth of posts (or more) ahead of time. I've been scheduling these publishing using my homebrew CMS, but [I recently ditched it for Siteleaf](https://apievangelist.com/2017/05/15/my-new-cms-for-manging-my-network-of-github-site/), and one of the things that were not possible with the CMS was scheduling--so I needed a hack.

I wanted to be able to just publish at least a weeks worth of blog posts, but then just trickle them out somehow using Jekyll, and avoid using the CMS layer. I got to work publishing a couple of "future" posts and tightening up any holes where the future might leak out into the present--specifically the blog and RSS/Atom listings.

First I set a variable to tell me what the date and time were for any given moment:

<script src="https://gist.github.com/kinlane/1b99291324e54b05e7ec5d3bcb621321.js"></script>

Then I translated the publish date for each post into the same format as my definition for now (seconds):

<script src="https://gist.github.com/kinlane/934de175203b5718c28954f3c5e7cf2e.js"></script>

Then you just check to make sure each blog post that is being displayed using Liquid is truly from the past:

<script src="https://gist.github.com/kinlane/2f446ff6a76ec355c0647bf13a282eb1.js"></script>

Voila, a filter for the future on my blog listing page, and the RSS or Atom feeds. After this, I published a schedule.xml feed which showed all my blog posts, even for the future. I use this to schedule Tweets, and other social media posts for my blogs throughout the week--allowing my social media management tooling to see into the future when it comes to my blogs.

It is a hack for achieving a blog schedule, but it works. It allows me to schedule my world days or weeks ahead, and stay focused on project work. One of the reasons I abandoned my homegrown CMS is I wanted to be forced to find solutions within the cracks of a variety of SaaS tooling, using feeds and APIs. I feel like these approaches are going to be more valuable to my readers, as I can't expect everyone to deploy a custom solution like I was doing.


