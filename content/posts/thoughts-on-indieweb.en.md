+++
title = "Thoughts on Indieweb"
date = "2023-01-08T20:20:41+05:30"
author = "KAKAN"
authorTwitter = "ThKAKAN" #do not include @
cover = ""
tags = ["selfhost", "indieweb"]
keywords = ["self hosting", "indieweb", "federation", "Mastodon"]
description = "My thoughts about the IndieWeb and why it might be a privacy risk"
showFullContent = false
readingTime = false
hideComments = false
Toc = true
color = "" #color from the theme settings
+++


Before we start, I'd like to point out that I'm not very well-versed on the topic, and this post is written on how/what I understand about "IndieWeb". Do correct me if something's wrong!

# Some concepts related to the post:
---

## Webmention
Think of how you can mention someone on Twitter. When you do, they get a notification for it, right? 
Currently, there's no way to do that _across_ self hosted websites ( _except Mastodon, maybe?_ ).
IndieWeb and its collection of different standards tries to fix it( _the one we are talking about right now is called Webmention_ ). Basically, when someone links to your website from their blog, their blog( _or some external service_ ) posts it as a comment in your blog/wherever you want. Or when some comments on your tweet about a blog post, it'll be cross-posted to your blog
All of that is due to **Webmention**.


## Microsub/Micropub

Then they have **Microsub/Micropub**, Microsub is basically RSS but with much more features and a standard for most of them. Micropub is a standard, but for publishing instead.
The advantage here is that, you can use one app, to post to as many blogs/comment on any other blog. You don't have to install an app( _like Medium_ ) to read/post/comment on their specific website. You would be able to install one app to manage everything

## IndieAuth

But, how will you prove your identity across them? That's fixed by **IndieAuth** using which you can define your own way of authentication, all the other websites will simply be using OAuth to connect you. This is rather neat, since you'll be resposible for your accounts over the web.

-----

Basically, Mastodon, right?  
Well, yes. [Mastdon is part of the IndieWeb](https://indieweb.org/Mastodon), but it only implements some of the features, not all of it.

## So, why do I think it's a privacy nightmare?

The most probable reason is due to Webmention, because of which, you've no control where *your* post/comment ends up using their _backfeed_. Their wiki does discuss this: [backfeed discussion](https://indieweb.org/backfeed#Discussion).  

While I think this is nice for data preservation, it's not so nice privacy-wise or legally. It's an action that's much more public than people think about...

For more information, there's [this excellent article](https://sebastiangreger.net/2018/05/indieweb-privacy-challenge-webmentions-backfeeds-gdpr/) written by [Sebastian Greger](https://sebastiangreger.net/) that goes to great lengths to explain this and also provides some probable solution and his thoughts on the matter.

---

**This article was originally written a long time ago( _somewhere around 2019ish?_ ) and might not be accurate anymore. Things have changed, and my understanding back then might have been wrong as well. I'll update it sometime to reflect more of my thoughts and correct whatever mistakes there might be. Thank you.**