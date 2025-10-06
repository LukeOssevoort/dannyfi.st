---
title: In search of an Open-Source VTT
categories: [General, Opinion]
tags: software foss linux vtt
---

This isn't just a blog post. It is the closest I can get to begging a talented software developer to just make an open-source VTT.

The VTT landscape is pretty dire. They are almost universally storefronts to rebuy the games you already own, just formatted for their stupid system. Roll20 is the exemplar of this with every system getting its own paid module with preconfigured compendiums that are basically essential for playing them without constant fiddling. Even then often the compendium is a little broken, requiring finagling to act right.

Even the mostly excellent Foundry VTT is infected with this, and the whole point of the damn thing is to handle systems and tools using open-source modules. If I want my beloved DCC RPG spell tables at the ready, I need also be ready to fork over cash for something I already own. Sure there are plenty of work arounds, but the point is that the software itself is slowly but surely moving in this direction.

Then there is the additional problem that Foundry doesn't guarantee backwards compatibility with old modules. If your favourite system hasn't been updated to fit the latest version, the only solution is to run up an older version. Running multiple systems often means running multiple instances of Foundry. No VTT should drive me, a perfectly reasonable not-at-all insane man, to containerise 3 different versions of your software just to run multiple systems!

I just want an open-source VTT that does all the stuff I expect. The only open-source VTT projects I can find are Owlbear Rodeo clones or the equivalent of digital dry erase maps. They're nice pieces of code but I am not suddenly going to move all my games to something that would require a bunch of additional tools. I want my players to just login and start rolling without having to look for their character sheet or remember a Discord bots dice commands. So let's get specific about what I want...

## Maps

This is the easy bit. Just a jpeg with a grid overlay (both square and hex), some draggable tokens, and a fog of war. No need for a fancy lighting system! In my experience dynamic lighting is just a way to guarantee that your players don't see shit. A simple, unified fog of war makes it easier for a GM to know what players can and can't see. Leave the complex high tech presentation stuff to plugins.

## Character sheets

Character sheets are an area where the right programmer could really get us ahead of the game. Currently VTT character sheets require a fair bit of programming knowledge to knock together, they are basically tiny websites. What if instead you could just upload a PDF of a character sheet, and then map required interactive elements to the sheet? It seems like a no brainer. Coupled with an easy to understand scripting system (ideally tailor made to handle dice rolling) and you'd have an easy winner.

## System automation

On the crunchier end of RPGs, there is a *need* for automation. At a real table there are games that demand handouts and open rulebooks - on VTTs this is better done with scripting. My dream VTT would need to have visual scripting - similar to Node-Red with the end result looking like a flowchart. Then the casual user has access to the same tools as the advanced users of Foundry - enabling them to automate games themselves. Now you have a user base with far more people capable of creating modules for their game of choice.

## And finally, a little bit of ethics

Free and open source software is just better. No one can force you to pay a subscription model just to access something you already own, or take it away when it no longer suits them to provide it to you. If it is on your machine it is yours. This should be the norm for computing, but in a world of operating systems with subscription models, forced updates, kernel level anti-cheat and many other business driven horrors  unthinkable to mortal man, it isn't. All I can do is try as hard as I can to pry myself and others away from the taint of mainstream computing. So please, don't be a coward. Switch your OS to Linux and move everything you can to open source software. It'll be better for you in the long run.

Also, I use Arch BTW.