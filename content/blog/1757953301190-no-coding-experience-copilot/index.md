---
title: "No coding experience + Co-pilot (what could go wrong.."
date: 2025-06-24
draft: false
description: "No coding experience + Co-pilot (what could go wrong.. 😅"
tags: ["godot experiments"]
---
## What this is about

Since the basic version of Microsoft's Copilot for Visual Studio became free to use, I've been trying it out by making tweaks to this website I had already previously made.

Using Copilot as help, I made this new "blog" section to the site, and ported over my old blog posts from my wordpress site, just so everything was under one domain name. And for just basic html and css stuff, It's worked great, albeit It got a bit stuck in a loop trying to fix something and It needed the me to tell it what to fix by holding its hand.

Since making these blog pages was pretty smooth with it, I got the idea of trying out how Copilot would work with making games on Godot, since the dataset knows GDScript and how the engine works + I had made a little JRPG demo game in RPGMAKER for the Impressions Jam just a while back, and was still in the mood of making something.

## Starting up

As soon as I opened Godot, I had the classic moment of having 0 ideas on what kind of a game I would even try to start making. Of course the smaller/less complex game the better, if a novice like me actually wants to actually get something finished 😂

I've been playing the tabletop rpg game HERO QUEST every now and then with a friend group + after I played some of the old ZORK games god knows when, I've had the feeling that doing a text adventure type thing could be cool, so I got the idea to kinda combine the two and make a text adventure game where I just lazily use the setting, story, characters and mechanics of HERO QUEST in a text adventure game.

Suprisingly setting up the basic base game mechanics and UI was not too difficult by working together with Copilot, and I got the setup done pretty quickly. I even got the bot to understand the rules and other logic of HERO QUEST, and it took that into consideration for the damage dice rolls and other stuff.

After going a bit deeper in to adding a ascii art map and other stuff, it got a more problematic, where Copilot sometimes started doing the classic LLM hallucination about an issue that was not the issue it was told to look at. Sometimes the plugin also bugged out, where it would proudly declare "I have removed the thing that was an issue, that you told me to remove!" and then it actually didn't remove it, requiring me to ask it "DID YOU REMOVE IT?" or just manually remove the lines myself.

But those things happened with my earlier HTML + CSS tests too, and I'm pretty sure a lot of the issues stem from the fact that I have all the game logic and systems inside 1 script, so Copilot gets confused and sluggish with so many lines of code to parse each query.

But nevertheless, I spent a few hours yesterday (when I started this test) and today, and managed to get some kind of "proof of concept" for the Hero Quest Text Adventure Game I had in mind.

Still need to set up a proper turn based sort of system so enemies can strike back after you've successfully input a command, and try make the catacombs area bigger, with more rooms and enemies, but for starters its something at least.

## About gameplay

How the game is played/works, is by typing commands on the input box on the bottom, so if you've ever played ZORK or that type of games, its the same thing.

To list all the available commands, type help and all the available commands are listed for you. There is also a music command that i forgot to add to the help info, which lets you control the volume by typing music 0, music 50, music 100 etc. to change the volume, or just type music off or music on to toggle the music

After you finish the quest and defeat the gargoyle Verag, there appear some command to return to town etc. The return to town does not work atm since there is no town to go back to, but in future would work to return back from a succesfull quest and do the usual shopping etc that happens between quests in HERO QUEST

Also the quest is cleared when you defeat Verag, so when you find him, you need to use the attack command on him to attack him, this starts combat, where in the future there will be a turn based system in place, where after you attack him, he attacks back and so forth. Just keep attacking Verag untill you kill him and thats the Quest cleared! and the end of the demo 😄

## Give the rough version a try?

If you go [here](https://eetusuikkanen.github.io/zorkquest/cargoquest/Endevour.html), you can try out the first, kind of playable demo. 
	

    