---
title: "The Adventure Continues?"
date: 2025-09-30
draft: 
description: "Back to Linux from Windows, why?"
tags: ["linux adventures"]
---
# Coming back after two months of Windows 11

So, a few months back i switched my system back to Windows since I wanted to use some new Kontakt libraries I had bought, and was not really happy with how finicky using Native Access and Kontakt was through WINE + had still used Windows 10 before starting these linux adventures, so wanted to give Windows 11 a try to see how bad it could be.

From my 2 months of testing, Windows 11 is not that worse than 10, but there was some *jank* compared to 10 that I was not fond of, one of those being a weird bug I encountered, where applications started really slowly when booted from the task manager, but if I ran as administartor via UAC they booted as fast as they had in Windows 10, which was really annoying and weird behavior..

Music production wise things worked as they had in 10, but soon started experiencing weird system crashes which later turned out to be a weird issue with the windows usb midi drivers that sometimes got confused since I had so many midi devices connected via USB to my machine, which then led to windows deciding to instantly shutdown the system to protect it, and I only managed to get 1 actual BSOD where it made a dump file where I could get this info.

So because of that I just decided to go back to Linux land since I had already had my fun of playing around making orchestral music for a few jams and my EastWest hollywood orchestra samples worked well via WINE in their PLAY vst sampler anyway, only Kontakt had some issues but I can try to substitute those with other stuff and will try to overall stop being so reliant on non native plugins and sounds, hopefully🤞😂

## Old/New Setup

### On the distro choice
Last time I had started with a Fedora system, but quickly changed to EndevourOS, so this time I went straight to EndevourOS since it had been a good experience the last time.

I'm mostly using EndevourOS since its Arch based, has a GUI installer, some helpfull tools and all the good stuff that comes with it being Arch based, i.e the Arch Wiki, the AUR, large userbase and the forums.

### Low latency/Pro-Audio setup 

Setting the system up and running did not take time at all, since setting up all the low latency audio stuff is really fast because the **pro-audio** package and **realtime-priviledges** package, which do all the setup for getting the system ready for low latency audio work and also install a lot of instruments and effects, so you're ready to get started with audio work. For this setup the arch wiki [Professional Audio](https://wiki.archlinux.org/title/Professional_audio) article has all the info on setting things up, likewise the [PipeWire](https://wiki.archlinux.org/title/PipeWire) article and the links to the official PipeWire documentation it has, give all the info on configuring the PipeWire sample rate and buffer sizes.

### Reaper DAW stuff
I also did not realize it last time around, but the arch repositories also have packages for the **SWS Extensions** and **ReaPack** alongside **Reaper** (which is my Linux DAW of choice).
Since **Reaper** is already included in the **Pro-Audio** package group, both **SWS Extensions** and **ReaPack** could be included there too in my opinion, since pretty much every **Reaper** user uses those as well, but thats just a little thing that really does not matter that much.

At this point the Audio setup was done, and I only had to get all my steam games downloaded and setup all other misc apps I use.

## Going forward..

Like I intended on the earlier *adventure* on Linux, my goal is to transition to permanently using Linux, which worked well enough last time and my only gripe was with the sort of *sunk cost fallacy*  I had with all the sample packages for **Kontakt** that did not work without some issues via **WINE**...

Hopefully this time I will just accept that if some things wont work as well as they should to be usable, then I should just stop using those and hope that one day **Kontakt** comes out with a Linux native version.

So to aid that I'm trying to really find some Linux native alternatives, with the first one probably being a good piano sample library if I can find one I like, or if I cant find one, maybe it's time to think about buying **Pianoteq** 🤔  

Other than the piano, I have a good selection of native synths and other stuff, and for orchestral stuff the **Hollywood Orchestra** worked great last time around.  

I've also already got **Yabridge** setup with the **WINE** downgraded to 9.21, and all my samples are backed up in my backup server, so I can get running pretty quickly on all of those when I need to, but for starters I'm going to not install them yet. The reason I'm holding the **WINE** package to older version, because **Yabridge** does not work properly on the newer versions yet

I'll try to keep posting some update blogs of the linux stuff I'm trying out/learning from time to time, but I'm pretty sure these are going to be pretty infrequent 😅

Anyway, thats all for now folks.