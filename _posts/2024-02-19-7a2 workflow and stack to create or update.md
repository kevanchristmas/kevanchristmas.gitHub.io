---
layout: post
title: Workflow and stack to create or update this site
tags: Living The_system
---

##  tl;dr

\[Writing Markdown] Obsidian -> VS Code \[version control via Git]\-> Github Pages \[Github Repository]\ -> Jekyll \[Jekyll Theme (Lanyon)]\ -> Browser

Framework/Philosophy:

1. Maximum Control/ Minimum Effort
2. Free and or Open Source with few local dependencies
3. Familiar tools
4. Version Control

![](https://kevanchristmas.github.io/public/assets/blog_stack.jpg)

(I am aware that I can, and have, use VS Code or Obsidian exclusively to write and edit markdown files - I'm sure that purists will be crying because I should edit them directly in Vim... - but the flow - whilst I'm improving the system - is to hack about in one Obsidian vault then copy to another (structured more like a zettelkasten as detailed [here](https://kevanchristmas.github.io/2024/02/12/standing-on-one-LEG-and-zettelkasten/)) from which I pick the notes to be published to the repo). 

Similarly I can/have run Jekyll/Ruby + DevKit locally for content creation/preview before publishing online but took this step out as it didn't add much to the edit-commit-push process or the end result, besides some nerdy satisfaction.

I ought to just be happy that I've escaped the rabbit-hole of markdown writing and notes apps (it might be worth detailing that journey at some point and I may share individual notes about using Jekyll etc). 

In short — I have customised/configured Obsidian and VS Code, using themes and plug-ins, to where I'm happy enough copy/pasting an entry out of between them - pretty much complete (minus zettel links) with final tweaks. I'm also using tags on the site which correspond to zettel categories and index. 


### 1. Simple: Maximum Control/ Minimum Effort

I tend to deep-dive into solutions to explore possibilities. I wanted maximum control over content and delivery and being less scared of technical details this led me to consider static websites. Static websites are  much faster and leaner particularly thinking of the type of content. I don't need webforms, lots of design, personalisation or content management.

More importantly I like being able to go in and edit not just the content and links but also some basic stuff in jekyll (and even a python script that generates/add tags) plus of course being able to roll back via Git if it breaks. It beats thrashing the black box of your CMS with a stick because you don't have a gears level understanding of what is going on inside it and your page looks funny.

Although this can get a bit 'tinkery' - I at least understand *most* of what's going on up and down the stack and once it was set up it's fairly easy to push from writing to publishing.

The cool thing is that GitHub Pages automatically detects changes to my repo’s master branch and using Jekyll integration auto-builds the site and publishes it live.

### 2. Free and or Open Source with few local dependencies

In addition to supporting Free and Open Source Software at least by participation, I also have zero hosting costs or software licensing fees. As stated I also have very few local dependencies.

### 3. Familiar tools

I have been using Markdown for over 10 years and I’m already using open source tools such as [Visual Studio Code](https://code.visualstudio.com/download) to further my Python exploration and [GitHub](https://github.com/) to store/share my code in the cloud and apply version control. 

As stated - Obsidian was also a daily driver and collectively this greatly helped to reduce the time needed to deploy and maintain this site.

### 4. Version Control

As mentioned, at Github I have a single repo and a master branch set up for this site. Obviously it can get a lot fancier but see point 1. above! As a 'non-technical' person I find the concept of Version Control one of the key building block concepts that are hard-wired into software development (thinking and *acting* like a programmer) but so poorly understood/implemented in many other business areas eg Documentation (Naming convention, Approvals, Revision history tables - 'track changes and comments' in Word anyone?....)

I see there's a bunch of stuff to expand upon/ share notes about from above so I'll aim to publish some re: understanding Jekyll and how I configure it as well as other topics.

Thanks for your time.