---
layout: post
title:  "The Fourth Modding Generation"
date:   2018-09-10 11:23:32
categories: modding
excerpt: The future of Hollow Knight Modding, and what it means for you.
---
The old guard, with the exception of Gradow, has long ago abandoned actively modding the game, and yet the Hollow Knight modding scene is brighter and better than ever before. The changes have come painfully slowly, so much that defining any end and beginning points for a modding generation is arbitrary. I'm mostly calling it the forth generation since it comes roughly alongside the forth major update of Hollow Knight. Along with a menagerie of new modders getting into the scene, including Ttacco, Papers, and Xhuis, the tools used by modders has expanded allowing some truly interesting and diverse projects. Here's a list of what modders are doing now. These are tools you should add to your toolbox if you want to make the next giant modern mod.

Custom in game sprites:

![Xhuis](https://radiance.host/images/4thgen1.png "Exaltation mod")
(Image from Xhuis' Exaltation mod)

These aren't new to this generation, but prior to it only existed rarely, or in hacky assembly mods which swapped out the sprites directly. Thanks to unity's sprite renderer component, modders are able to in just a few lines, replace any in game sprite or set of sprites with any other one. I bring this up because it is a vital part of almost every forth generation mod, including: Redwing CP2, Dead Hallownest, Exaltation, Lightbringer API, and Shitmodst Reborn, among others.

Embedded sound effects:

Although custom sound effects in general aren't new to this generation, the only prior use was the BoopMod. A simple meme/example mod which loaded one sound effect from a path using unity's www. Now, mods such as Redwing CP2, Exaltation, and Hollow Point can and do load these sound files directly from the assembly itself, using a simple unity waveform serialization library. These effects can then be played on any AudioSource, including the one on the HeroController.

Coroutines:

Coroutines are as old as time, or at least Unity. But their usage in mods was very limited if non-existent, with even mods made by pro unity developer KDT avoiding them. Until 56 brought them to the attention of the modding scene. Now, nearly every mod takes advantage of them. Including Infinite Grimm Modern, Redwing, Exaltation, and Hollow Point. Nobody knows how they work, at least internally, but they do work to make Update functions less complex.

Custom cutscenes/video files:

![Nuke Meme](https://radiance.host/images/4thgen2.jpg "Nuke Meme")
(Image from Fallout 3 Intro / Nuke Meme mod)

Although both easy in theory and practice, embedding custom video files into Hollow Knight was first introduced only recently, by Redwing CP1. Although videos cannot at this time be loaded from embedded resources, they still mark an impressive milestone for those wishing to make total overhauls. Custom video files are present in Redwing CP1 and Shitmodst Reborn.

Custom Gameobjects:

![Fennel Mod](https://radiance.host/images/4thgen3.png "Fennel Mod")
(Image from Fennel mod by KDT)

Custom gameobjects are a trick as old as the first Hollow Knight mods. Gameobjects have been used in many mods everywhere, mostly for drawing canvas objects. However, their true potential has only been realized recently. By creating a more complex custom gameobject, with its own set of monobehaviors, such as an enemy or player weapon, you can circumvent the hackery that is working with PlaymakerFSMs and instead implement everything yourself. The unreleased Fennel boss alpha and Redwing demonstrate the potential that using custom gameobjects has.

Custom Particle Systems:

Particle Systems exist in vanilla Hollow Knight. They are an easy way of making things look cool when you lack any artistic talent. Yet, up until Redwing CP1, they were never used in any Hollow Knight mods. Redwing CP1 changed this by adding napalm- A proof of concept for particles. The Combo mod uses them to much better effect, as a way of showing the player's current combo directly on the knight itself. Particle systems go a long way towards making ugly mods look alright and giving pretty mods the slight polish they need to become perfect.

If any of these tools interest you, I highly recommend you look at the source code for these mods. Many of which have yet to be released. Others have been. All of these mods are or will be available on [Gradow's Mod Installer](https://radiance.host/mods/ModInstaller.exe) though.
