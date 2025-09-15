---
title: "Reflections, a few months after switching..."
date: 2025-06-30
draft: false
description: "How things have felt after switching"
tags: ["linux adventures"]
---
## On my change of distro
So.. In my previous post I was using Fedora as my distribution, and that was because everytime I've demoed linux for a few months, I've always tried a new distribution each time and had already tried out **Ubuntu Studio**, **Manjaro**, and **EndevourOS**  previously, So I decided to try out **Fedora** for music production this time around.

I've been running **Fedora** on my laptop for a long time now and had used it previously for a server machine that I used to host a **Mumble** voip server.
So naturally that made me want to test how easy/hard setting it up for music prodction would be.

And like I mentioned on the first post in this series, it went pretty smoothly, mostly thanks to a lot of linux audio setup being the same across all distros.

But after getting my audio stuff up and running, I had updated my system and come across a really annoying issue that the new kernel update had brought with it, that issue being that I use my phone as a hotspot to get my internet connection since I'm still waiting for my ISP to install the fiber cables they've been promising to install for 2 years now... (should hopefully be installed by the and of the year ...) And some changes in the new kernel made it so that linux does not recognize usb devices as modems anymore, so no internet connection for me...

The issue can be circumvented by just rolling back to the previous kernel and **Fedora** has a great system where the OS always keeps the previous 3 kernel versions cached, probably for these kinds of situations, so I could just roll back to the previous kernel and everything works.

But after checking/waiting for the new kernel including the hotfix to come available, I found out the fun part of linux, where I would have to wait longer for the hotfix kernel since I was not on a rolling release/bleeding edge distro.. 😓

So after checking **bodhi** (fedora's update system) daily to see if the new fixed kernel was on testing, or better yet, going to the stable branch, I just said **Fuck it!** and decided to switch to the distro I had used for a good half a year + before.
And that distro was **EndevourOS**, which is a rolling release distro based on **Arch Linux** and would already have had the fixed kernel update for some time now.

During my previous linux audio testing I had used **EndevourOS** for 2 itch.io composing jams and 1 Global Game Jam game, and had found the system to work without issues and the setup for audio had been been quick and simple, thanks to the pro-audio metapackage and all of Arch Wiki's articles on [PipeWire](https://wiki.archlinux.org/title/PipeWire) and [Professional Audio](https://wiki.archlinux.org/title/Professional_audio), which contain a lot of useful info worth reading through when configuring the sample rate and Quantum in PipeWire.

>Having a basic working music production setup in an Arch based distro is pretty simple with the packages provided in the Arch repository's and the AUR user repos.
>
>>On my installation of **EndevourOS** I used the recommended quick setup from the [Arch Wiki](https://wiki.archlinux.org/title/Professional_audio) and just installed the **pro-audio** package group and the **realtime-generic-setup** AUR package, both of which which installed a big bundle of open-source instrument and fx plugins, some open-source DAWS and made a quick config setup for low latency audio respectively.

After that the only other thing I needed for music production was installing **Yabridge**, which is available in the official Arch repos, so just running `sudo pacman -S yabridge yabridgectl` installed yabrige and the cli tool for it 😁

Then I installed **Reaper** and got all my windows plugins installed via **WINE**, got those connected with **Yabridge**, and with that I was pretty much done with my setup.

## First "Real" test of my audio setup
Not long after I had done the switch to **EndevourOS**, I took part in the **Impressions Composing Jam: Mystery #1** composing jam event, which was the first proper test of my hopefully new long lasting music production system.

I started out with doing some orchestral music using EastWest's Hollywood Orchestra, and the PLAY sampler VST it uses worked great via Yabridge and WINE! Kontakt on the other hand worked too, but I have this feeling that it's performance is slightly worse compared to windows, but it's not SO bad that it's an issue to me.

I did end up changing to a **NES** sound palette for the final jam submission, but I still was able to test and confirm that **Kontakt** and **Play** work OK enough.

I did keep a little journal/devlog during that jam, which you can read [here](../1757949741177-imptressions-mystery-1) 

## After the first jam test
All in all the setup seemed to work smooth all throughout the jam, and I even made a little demo game for the music using **RPGMAKER VX ACE** via proton on **Steam**, so I could call it an all around success.

I already knew it would work well from all the previous few month tests I had done the years before, but I was still pleased to find everything to work the same now.

After the jam had ended, and I had managed to rate all of the other submissions in the jam, I got the idea to start messing about in the **Godot** game engine, using the integrated microsoft Copilot LLM bot in Visual studio since a free tier had become available.

I've done a couple of small games before during a game programming optional subject/course while in school, but it was after going through those classes I really realized that programming was not for me and felt really hard to grasp and wrap my head around it, so I never did any programming after that, and have 0 knowledge and skills about it 😂

But working with Copilot I managed to get a little *proof of concept* of a text adventure game done, which im intending to continue after the free tier usage refreshes next month, since I already spent all of my "tokens" on the poc demo and some tweaking to the website by making a blog section and importing my wordpress blogs to my homepage 😅

Which turned out to be a waste, since I then pretty soon after remade the whole website using a static site generator...

## Website overhaul
As I mentioned before, I have ported over my blog from wordpress to this github pages site I use as my website.

I initially had the page made with some html and css, and it worked great for just a little ABOUT ME page with links to all my profiles elsewhere.
But after making a blog section with sub pages for all the post and their categories, the upkeeping became a bit of a nightmare, since every time I changed the navbar I needed to make the change to all pages and posts, which got a bit ridiculous, and writing the blog posts was really tedious with having to use all the HTML tags to add paragraphs and everything else.

So I decided to just take the plunge and learn how to use a static site generator, which would be a lot easier to use and manage.

I had a friend recommend **Astro** before, but saw that a lot of people used and recommended **HUGO**, so decided to go with that, since with a large userbase there's always a better change of finding a post about an issue you might come across.

After watching a video about how it works and following the official quickstart tutorial, I got it setup without much issues, and started porting over all of my existing blog posts.

The good thing about static site generators is that there are a lot of premade themes available to choose from, and installing is as simple as just cloning the git repo to hugo's theme folder and setting that as the theme in the config files.

For my site I really liked the look of the [Poison](https://github.com/lukeorth/poison) theme by Luke Orth, and went with that.

I found an issue in the theme where the About page does not appear in the sidebar menu, but thats not too bad of an issue since the main site URL opens that page as default, and my name also works as a link there.

The way content is written in hugo and other static site generators, is using markdown, which I was not really familiar with, but after I learned how making headers, links, bold, italics etc worked, It felt great! Compared to how cumbersome writing blog posts was in HTML, this felt like absolute bliss 😩

I'm still learning the basic syntax and I just learned about Blockquotes while writing this post, but I hope all that stuff will turn to muscle memory at some point, so I dont need to read up on how it works every time I want to do a Blockquote or something else 😅

I got all my blog posts ported over to the new site, wrote a new post and overall got things looking pretty OK and published the site, replacing the old one, with the new **HUGO** site being the site you are reading this in RIGHT NOW.

I like how the site looks and functions overall as is now, but I feel like I need to look up if I can somehow get the about section to appear in the side menu, and then if I can also add a link to some form of **POST CATEGORIES** page, that would contain links to all of my different post categories for easy viewing (so for example, **Linux Adventures**, **Jam Journals**, **Godot Experiments**, etc.)

Hopefully thats possible with this theme without too much tweaking things needed, but at least for a start, I feel this page is pretty OK for now.

## In conclusion
With the audio setup working and the blog ported to my website, I'm feeling pretty happy with everything.

Seeing as how my motivation on working with music is usually pretty much 0 unless its for some sort of a project, jam or something else, any other music proction testing will probably happen on the next Impressions jam, which starts in bit over a week.

Since the Godot text adventure thing is on hold for now, untill i got the next free "tokens", I've started a little 2d hack and slash game.

On the 2d hack and slash game I've managed to get a moving character and a enemy that patrols around, that then chases to try and attack the player when they get too close, and can take damage from the players attacks and die.

I think its a good start for now, and probably need to do some level design to get a proper large area with platforming and more enemies to fight.

But that might be on hold too for a bit, since I've gotten the itch to continue my Final Fantasy playthrough, where I've been playing all the original FF games I've never completed.

I just finished FF 3, which was OK, but had some old school jank that could've used some QOL in the remasters, but I guess there would've been a bit of a backlash from the OG fans yelling "NO CHANGES!!" like vanilla wow had.

Next up is FF 4, which luckily won't have the job system from 3, which I had a bit of a love/hate relationship with 🙂

But anyway, thats all 👋

