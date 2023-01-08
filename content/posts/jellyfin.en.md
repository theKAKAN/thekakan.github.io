+++
title = "Experience with Jellyfin"
date = "2022-10-15T14:09:08+05:30"
author = "KAKAN"
authorTwitter = "ThKAKAN" #do not include @
cover = "https://raw.githubusercontent.com/jellyfin/jellyfin-ux/master/branding/SVG/installer-header.svg"
tags = ["selfhost", "media"]
keywords = ["jellyfin", "self hosting", "media server"]
description = "My experience with self-hosting Jellyfin for some years"
showFullContent = false
readingTime = true
+++

Before we go further, I'd first like to say that I absolutely love using [Jellyfin](https://jellyfin.org/) 
and I'll continue using it after this, too.  

Let's start with the advantages!

---
# Advantages:
---

## 1. Media metadata
This is basically the reason why people would want Jellyfin over say, a file 
manager. It manages to grab most of my media automatically from different 
sites, and it's really accurate at it too!  

And if that wasn't enough, it also fetches actor information, networks etc and 
lets you browse according to that, too. 

## 2. Playback History/Statistics
Another reason I like it is because of [Playback reporting](https://github.com/jellyfin/jellyfin-plugin-playbackreporting/) 
which offers a nice view of how much I've watched, or how many. I love seeing 
data and this is really nice since it's a centralised place for all my users.

## 3. Sync with other services
Jellyfin has plugins to sync watch lists and library with services like [Trakt.](https://github.com/jellyfin/jellyfin-plugin-trakt)  

This is really nice, especially if you want to know if you already have 
something in your library, or if you need to download/rip it from somewhere.  

It also has your watch history, and Trakt itself provides a lot of statistics 
which adds to its feature set, in my opinion. 

## 4. Plugins
By default, only point 1 is possible OOTB. However, with the help of its plugin 
ecosystem, you can add various things to it, like the above mentioned features.  

This is something all of the competition has, but I still felt like I should 
atleast mention it.

## 5. Multiple Users
This is also something that sets Jellyfin apart from "local" media managers 
which let you store, view and update metadata and keep a playback history, 
but tie it to a single user. Often times, its annoying and also cannot be 
changed since its usually stored in NFO files.  

Oh, that reminds me, Jellyfin has an option to store metadata in NFO files 
at the location, which I always keep turned off because I like them 
directories kept clean! :yum:

---
# Disadvantages:
---

Time to move on to the not-so-good parts in my experience of self hosting Jellyfin...

## 1. Mixed Libraries don't work well
I don't think it's a surprise to anybody, but if you have a lot of mixed content 
i.e, TV shows and movies in one folder (_say you have one folder for all Anime_), 
then you should consider moving them to different folders.  

The problem arises since Jellyfin can no longer safely say "this is a movie", 
or that "this is a series", so in the end you'll end up with multiple movies 
marked as series and vice versa. It's mildly annoying at best, and unfixable 
at worst.  

**My solution**: I moved Anime movies into my main Movies library, and then created 
a collection of all the anime movies. That way, I can still browse them separately.

## 2. Lack of Plugins
This is mostly because Jellyfin is changing from Emby, so plugins made for Emby 
might not work anymore. And because Jellyfin itself is getting updated, older 
and unmaintained plugins might not work anymore either. While there are some 
really good plugins that do work, it'd be nice if there were even more maintained 
ones available to use...  

Unfortuneately, this is kind of a chicken egg problem and I've no idea how this 
might get solved. That said, there are some really good plugins out there, I even 
[made a list of ones I found interesting](https://github.com/stars/theKAKAN/lists/jellyfin-plugins)!

## 3. Metadata Search/Update is... slow
I'm not sure why this happens, but if you have multiple metadata providers, 
you'll likely experience major slowdowns if you enter broad enough terms for 
searching.  

Oh, and sometimes the images don't get updated. Maybe it's a cache issue, I'm not sure...

**My solution**: I grab the IMDb ID and search via that, in case the builtin 
metadata downloader gets/grabs the wrong metadata

## 4. TV Shows are kind of a mess...
Honestly, this is more of a standard/naming problem than it is with Jellyfin, 
but nonetheless, it's a problem that I experienced a lot.  

Basically, many series are listed differently under different providers.  
For example:
  - Kitsu has 6 different entries for "My Hero Academia", for each of its different seasons.
  - Trakt has one entry for "My Hero Academia", with 6 seasons inside it.

This same pattern continues for many different series — as well as some movies — 
which makes it annoying to efficiently categorise and manage a library.


---

I hope this post helped you in some way. To me, Jellyfin is not just a media 
server, it's also a playground for me to play with my collection of movies 
as well as find ways to efficiently organise them for future usage.  

I simply chose Jellyfin as its the FOSS option, which makes it likely that 
in the odd case that it gets abandoned, I might be able to keep tweaking it 
to make sure that it *just works™* and suits my needs.