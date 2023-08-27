---
published: true
layout: post
title: I Deleted My MySQL Database
date: 2017-07-10T11:00:00.000Z
tags:
  - Kin Lane
image: >-
  https://s3.amazonaws.com/kinlane-productions2/101/amazon_aurora_thumb_person.png
---
<p><img src="https://s3.amazonaws.com/kinlane-productions2/101/amazon_aurora_thumb_person.png" align="right" width="40%" style="padding: 15px;" /></p>I just deleted my primary MySQL database. Of course, I backed up everything, but it is the first time since 2011 I've cleaned up my entire database backend to the point where I could delete the entire instance (with confidence). I was motivated to do this mostly because I couldn't downsize the AWS RDS instance to a smaller instance due to a variety of constraints. The situation gave me the opportunity to clean house, and rethink my next moves.

Instead of setting up a new MySQL instance, I went with [the new MySQL compatible Amazon Aurora](https://aws.amazon.com/rds/aurora/). I setup a smaller instance that was more affordable, and I was able to easily import the database backups I had made in my previous setup, but now I had a cleaner, more modern Amazon Aurora situation. Which as Amazon claims, "provides up to five times better performance than MySQL with the security, availability, and reliability of a commercial database at one tenth the cost". Time will tell...

I like cleaning up my database and migrating to a new solution, even if the solution is still with the same provider. It helps me think through things, shed unnecessary databases, tables, and hopefully costs. Everywhere I've worked, and within all the businesses I have owned the database is always the hardest thing to manage, and migrate. I want that to be a thing of the past. Now that I have things cleaned up, I'm going to keep my databases small, modular, and using standardized solutions that top tier providers support. This means I can migrate my data wherever I need to, and wherever it makes sense to my business.

Another thing that has also allowed me to migrate my data in this way is that I have offloaded a significant portion of the data I manage, which drives my public research to Google Sheets. This approach helps me simplify, and modularize my data, again using a common tool (spreadsheet / CSV), but in a way that I can easily collaborate with others, and publish to Jekyll and GIthub using YAML. This shift in my world is all about helping me reduce the bulk on the backend of my business, and making sure I spread out my business data, content, and algorithms across a variety of solutions. While making sure all the services I use have APIs that allow me to automate, orchestrate, and of course migrate my data whenever I need to.
