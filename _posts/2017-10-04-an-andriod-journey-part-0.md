---
title: An Android Journey - Part 0: Introduction
updated: 2017-10-04 20:00
categories:
    - android
    - software-development
---
Learning how to develop an app for Android has been on my to-do-list for a long time now. I figured as part of the learning process, writing blog posts about it may be helpful to reflect on any progress I made towards specific goals. This project will also help me in gaining some more experience in software design and architecture.  
This project is Open Source, the repository can be found [here](https://github.com/qn0x/copypasta) and a minimalist project page can be found [here](https://qn0x.xyz/copypasta/).

# The App  
What I actually want to create is a more or less useful und certainly fun app that is a able to query arbitrary subs on Reddit and extract so called "copypasta" (text snippets that are copied from that subreddit and pasted elsewhere). Obviously these posts are text-only. A user then should be able to save (and categorize) these snippets and use them via a custom Android keyboard.

# What I Need To Learn
I've been planning ahead a little bit and wrote a short list with things that I need to learn (and the rough order in which to learn them) in order to create the app:
1. OAuth (in general and how to use it in Android apps)
2. Using the Reddit API
3. The Android lifecycle (as well a bit of UI/UX Design)
4. A way to run (regression) tests for Android apps (I've worked with JUnit and similar frameworks before)
5. Storing/retrieving user data on an Android device
6. Using a ReST API on Android (HTTP request handling)
7. Creating or customizing an Android keyboard

# What I may need or could come in handy at some point
* Gradle builds (if the stock build from Android Studio doesn't suffice anymore, worked with Maven and a little bit of ANT before)

# This Format
I plan to write a blog post whenever I reach any of my milestones, if I learn something I consider useful for others or something relevant to this project happens.

# Milestones
1. Design drafts of UI are complete
2. First draft of architecture is complete
2. Data from Reddit can be queried and is available to use in the app via some kind of DAO(Data Access Object) or DTO(Data Transfer Object)
3. UI is implemented
4. App logic including storage/retrieval of user data is implemented
5. Custom Android Keyboard is working
