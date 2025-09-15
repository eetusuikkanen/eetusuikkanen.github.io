---
title: "Start of the Linux Adventures"
date: 2025-05-06
draft: false
description: "Setting up my system"
tags: ["linux adventures"]
---
## Initial setup
I’ve been playing around with making music on Linux every now and then with some jam projects, but after trying different distributions and learning about what I need to run some of my Windows software on Linux, I finally decided to take the plunge fully and try to swap fully over even if I had to give up some of the orchestral/acoustic sample libraries I couldn’t get running.

I’ve tried to get the EastWest download/manager software working before using WINE, but couldn’t get the ui working correctly to install the libraries and Play engine. So this time around I saved my sample libraries to a different drive and kept the installers for the VST plugins, and to my surprise Play installed without a problem and the ILOK drm software they utilize works without a problem, so I could just tell PLAY where to find the samples and everything worked without an issue. It’s really unbelievable that this can actually work, and really shows the hard work that the WINE team and the creator/maintainer of Yabridge has done for it to be possible!

I had gotten Native Access working before, but they’ve released a new version n3 that is not working with wine yet, but hopefully might work on a later WINE version.

But with Play working well I’m pretty much set for all the basic orchestral sounds but I still need to actually write a full piece using those to see how the performance is, since I don’t have any old projects to demo with since I used Cubase in windows for those and now use Reaper while in Linux since Cubase is not natively supported.
## Some resources/tools i used for setting things up:
- [Fedora low latency setup guide/documentation by Audiojunkie on the LinuxMusicians forums](https://linuxmusicians.com/viewtopic.php?t=27121) - This is a helpful documentation on setting up Fedora for low latency work, best to read all the posts in the thread before doing any of the mentioned steps.
- [Yabridge](https://github.com/robbert-vdh/yabridge) - This is the most important thing in the whole setup, it works together
 with Wine to be able to use most windows vst’s on linux. The github page has a guide on how to set it up depending on your distribution.

- [SeXan’s pipewire config script for reaper](https://github.com/GoranKovac/ReaScripts) - This is a handy reaper script that opens a little GUI window in reaper to change the samplerate and buffer size for pipewire. You need to have the ReaPack repo manager extension installed and then import the repository with link from their github to ReaPack and then you can download the script called PipeWireConfig from there. After installing it you can make a button on the toolbar for it, add a keybind, or just call it from the actions menu when you need it.

- [Audinux COPR repo](https://copr.fedorainfracloud.org/coprs/ycollet/audinux) - This is a user repository for Fedora maintained by Ycollette from the linuxmusicians forum with a lot of audio plugins/software in it so you can easily install them via your package manager