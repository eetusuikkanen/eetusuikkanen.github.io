+++
date = "2026-02-28T10:57:48+02:00"
draft = true
title = "Impressions Composing Jam: Imagination #4 "
categories = [ "Jam Journals" ]
tags = [ "impressions jam", "devlog", "jam" ]
description = "Jam devlog for the Impressions Composing Jam: Imagination #4"
slug = "impressions-composing-jam-imagination-4"
+++
# First jam of 2026!
## Foreword

I Haven't done much music stuff aside from 2 little sketches while tweaking my orchestral template, so I've been looking forward to an actual composing jam to hopefully get the old brain again..

From doing these jam devlogs for the past few years now, I've learned that trying to keep a proper journal for each day ends up with me forgetting to write down what I've done and any thoughts for a day and then having to try and remember what I did on that day while writing it down the day after... 😅

So because that, I've decided to change the format of my jam journals a bit and ditch the "Day 1, Day 2, Day 3" daily notes style, and just write about things as I go without mentioning any actual *timestamps* for things. That should be a bit better to manage for me.

## The Theme

For this year's Impressions Composing Jam, there has been some new additions and changes to the different jam *flavours*, with theme of the **Imagination** jam being to score a scene from a text/narration read by the jam's host **Alex** over some mood setting SFX.

Haven't really written music for anything like this before, so will have to see if I get anything done that actually fits the mood 😁

The theme has 2 different scenes to choose from, or you can write for both, if you so wish and have the drive to, with the different scene's being:  
**​Scene 1: The Factory in the Mountain** and **Scene 2: The Storm Colossus**

**Scene 1** has the protagonist traversing through a large factory inside a mountain, reaching a large door that opens to reveal a landspace. **Scene 2** follows after **Scene 1** where the protagonist surveys the landscape, where they see a large mountain in the distance where they see, on the mountain, a colossal machine sending out bursts of lightning.

Actually, why am I even describing the scenes when I can just put the theme video with the narration here 😅

### Scenes 1 & 2
{{< youtubeLite id="LVwgo5coli4" label="Theme!" >}}

## Initial ideas and feelings

From the narration and sound effects, the setting for these scenes felt really *Steampunky* to me to going to write stuff with that sort of thing in mind.

Because of the steampunk/industrial feel of the setting, using a piano to sketch stuff somehow felt *wrong* to me, so instead i loaded up a Rhodes electric piano sound instead, which I also doubled with a synth keys/pluck sound after a bit.

Listening to the first scene on loop and just noodling around on the keys, I got an idea for a little very repetitive figure around moving minorsus2 chords with a top line that had a semitonal movement between the minor3 and 2 notes as a sort of a motif-ish thing, which I felt fit the steampunk/factory vibe nicely with it's repeating qualities.

For the sketch of the first idea, I used my rhodes+synth sound as the base skeleton and added layers on top of it, hopeing to spark some ideas for other parts along the way.

After an hour or so, I had managed to form up some sort of a mess of sounds and decided to take a break and come back to it later with fresh ears, to see what parts work and what don't.

**Initial idea:**

<iframe src="https://drive.google.com/file/d/1HJljOK5Qc7A6ZvP0QOV7yVd4-2wv3VBl/preview" title="Google Drive Audio Player" width="550" height="60" frameborder="0" style="border:none;overflow:hidden;" allow="autoplay"></iframe>

## Not that good great after all?

On the day after, I listened back to the sketch and felt it felt pretty meh to me after the break.
So because of that I decided to try the idea out with just a  orchestra palette to see if it feels any better, which will take some time to get a arrangement done, but the jam lasts 2 weeks so there is time to experiment different ideas out like I usually like to do.

I initially started out with the assumption that the music was meant to underscore the theme narration and not be too in the foreground, but now I felt I'd mistaken this jam for the Ambience flavor one, where being ambient/mood setting was the main focus and for this one its mostly just writing music for the setting/scenery the narration and sfx give you, without minding how in your face the music is 😅

So for the new orchestral try I'll just write how I feel from the theme instead of trying *hold back* the energy 😁

After changing the sounds to orchestral ones and adding a new section for the **Scene 2** I think it's better this way, the orchestration is pretty crude but will work on forward from this, first things I probably need to make the orchestration change at parts to help highlight the different hitpoints in the scenes (getting to and opening the doors outside, and then seeing the landscape and the Storm Colossus), since as it is before the last section for the storm colossus it's pretty boring and samey feeling throughout.

**Orchestal version:**

<iframe src="https://drive.google.com/file/d/1oI-uUxM7ccJFhysVipdtyQZRRcqOOJYs/preview" title="Google Drive Audio Player" width="550" height="60" frameborder="0" style="border:none;overflow:hidden;" allow="autoplay"></iframe>

## Procrastination time!

The day after as I was going to start working on the track again, I was thinking what kind of metallic sounds I have and could use to amplify the feeling of being inside the factory in the mountain, and was reminded of this wonky sounding bell thing I had made by sampling a holesaw drillbit since it produced a clear pitch when hitting it.

Since I've been thinking about trying to learn and make a sample library for DecentSampler, this time I finally took the plunge and went through the work of making a simple instrument by sampling the 3 different size holesaw bits I had.

Luckily the [documentation wiki for DecentSampler](https://decentsampler-developers-guide.readthedocs.io/en/latest/index.html) has a simple [boilerplate xml code](https://decentsampler-developers-guide.readthedocs.io/en/latest/appendix-c-boilerplate-dspreset-file.html) to start from, so I just took that and added some other GUI elements that I needed for my instrument, with adding other UI elements being at first a bit confusing, but the documentation has all the info needed to get things working, with definitions and example code for all the elements.

I made it so that the 3 different holesaw bits each had their own volume slider to be able to easily change the sound and I also added a convolution effect with some different Impulse Responses, which should be Creative Commons licensed but will have to double check and remove/replace any that aren't, since I'm intending to try to make more sample instruments and just share those for others to use if they want.

One thing I still need to look into, is how the round robins and dynamic layers are made in the xml code, since as it is now the instrument is just using single samples for each holesaw.

**How it looks and sounds:**

{{< youtubeLite id="0nm3bm4qJCM" label="How it looks and sounds" >}}

I decided to make a git repository on Codeberg for my DecentSampler instruments, since from what I understand Codeberg is meant for hosting Open Source and Free Software projects, and this is meant to be exactly that + if I ever get around to sampling my voice for anything, I don't want to put that straight into github, for probably obvious reasons.. 😉

It's still rough around the edges first creation, but I'll try to use it somehow on the jam track and if you want to give it a try, the Codeberg repo is here:

{{< codeberg repo="eetusuikkanen/ES_DecentSampler_Instruments" >}}

Writing this the day after , the repo name is pretty awful with the underscores so might have to change it at a later point, but for now that's what it'll be 😅

## Same old roadblocks..

Been procrastinating with the jam track for a few days now, mostly just messing around with making DecentSampler instruments.

Only thing I've done to the track after the first few days of the jam was trying out my sample sounds in it, with having made 2 new sounds after the first one, with one made from some samples of whistling and another with some hits on a couple random metallic objects.

I've only recorded a single dynamic for all of them, but the metallic hits got a bit of use in adding some texture to the big bombastic tutti hits for the Colossus.

At this point I'm not really getting any orchestration/arrangement ideas to improve the track, so perhaps might be time to put this one on ice for a bit and try to make a new take on the theme again, in case the issue is just that I'm not vibing with the current one, like the first bit more electronic take.

This seems to be a recurring issue for me on most jams that are longer than a few days in length, where having too much time ends up with me constantly second guessing every single thing about my submission and in turn constantly getting stuck and unable to proceed from however far I can manage to get on a track during my first "creative session" upong getting the idea/starting it.

Regarding this issue, I've been thinking about it before, and this year might finally be the time I just try out writing stuff how it comes to my head, and totally disregard if it's good or not, maybe then I can actually get more tracks done for jams and not spend a 2 week jam writing just 1 track and spend 80% the jam pretty much doing nothing 😅

It's going to be a pretty tough thing to do, but hopefully I can manage to adopt that sort of a "mind-set", since I don't think this issue is going to go away otherwise.

Maybe on the same time I'll fully move my music production to linux too, instead of the dualboot with windows solution I decided on at the end of last year, which was mostly because of no native support for plugins/platforms like NI Kontakt and EW Play etc, but they do *work* via WINE and Yabridge, albeit with the obvious slight performance hit. As a side note the Native Access software is a pain to try and use under WINE, so to avoid headaches it's sadly easier to use a cracked version of a software you own.. 🥲.

The installer/manager from EastWest did work pretty much without issues for me under WINE, only issues were graphical with the GUI and fonts, but for downloading and installing libraries worked OK enough. The ILOK licensing service also worked, but there is one VERY IMPORTANT thing to remember with ILOK if you need to use stuff that has those licenses, and that is to remember to UNAUTHORIZE all licenses from your machine before every time you update your WINE version or to be safe, anything wine related. This is because everytime wine updates, the machine ID for the wine prefix can change and that leads to ILOK thinking you are on a new machine and need to re active the licenses, but some bright idea person at ILOK decided that you to deactive licenses from a machine needs to be done on that machine, which can lead to those licenses be stuck on that old wine version machine ID and you need to send a "this machine is unavailable" request to all the different companies whose products you use from the ILOK manager app, and it can take quite a few days for all the companies to release the old licenses back, leading to you being unable to work with any of those plugins for that time. I've made this mistake a couple of time's, so do keep that in mind 😉 

If I'm still stuck like this on the next week, I might just go ahead with wiping my windows drive and switching to work in linux during this jam, but probably will do it after the jam.

Anyway, hope you enjoyed the unasked for mid jam vent/rant, made for thrilling reading I'm sure 😅

## Better sooner than later, i guess?

Few days after the previous text, I'm writing this now a linux system after backing up my windows files and then formatting the whole drive, after which I also formatted my existing EndevourOS (Linux) drive and decided to start from a completely fresh install.

Since I've done the *pro-audio* setup/tweaks to new linux installations a few times now, getting things up and running was pretty quick.  
The one thing that took me a bit was getting EastWest's installation center and Play working properly without crashes and other issues, since they need some additional stuff that you need to install to your wine setup using the *winetricks* tool

