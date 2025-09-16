---
layout: post
title:  "Stellar Scrapm'n, a game for the Playdate console"
excerpt: "I made a space salvage game with Marty on the Playdate. Come see!"
author: hunter-pankey
date: 2025-09-15T23:00:00-04:00
draft: false
tags: 
  - playdate
  - dev
  - gamedev
  - game-announcement
  - playjam
seo:
  title:
  description:
  image: 2025/09/playjam-8/stellar-scrapmn-title.png
images: # relative to /src/assets/images/
  feature: 2025/09/playjam-8/playdate-angles.jpg
  thumb: 2025/09/playjam-8/stellar-scrapmn-title.png
  align: object-center #(default) - other options at https://tailwindcss.com/docs/object-position
  height: # optional. Default = h-48 md:h-1/3
---

![Stellar Scrapm'n](/assets/images/2025/09/playjam-8/stellar-scrapmn-title.png)

Last weekend, my friend [Marty](https://martymcgui.re/) and I built [Stellar Scrapm'n](https://schmarty.itch.io/stellar-scrapmn) in a [weekend game jam](https://itch.io/jam/playjam-8/entries) for the Playdate. Stellar Scrapm'n is a flyin' around space, pickin' up treasures game. It was a lot of fun and a decent amount of frustration building this thing!

72 hours is not a lot of time to make a game, it turns out! The theme of the jam is "ascension", which, of course, can mean a lot of things if you're willing to accept metaphorical meanings. We ended up making a space salvage game where you navigate the game world using thrust and rotation controls using the Playdate's crank, avoiding enemy turret fire, shooting back, and collecting scrap parts to turn in for cash.

![Stellar Scrapm'n](/assets/images/2025/09/playjam-8/stellar-scrapmn-1.png)
![Stellar Scrapm'n](/assets/images/2025/09/playjam-8/stellar-scrapmn-2.png)

Our version of ascension is of the "[Hardspace: Shipbreaker](https://hardspace-shipbreaker.com/)" variety. Having had few options to make your way in this world, you sign an onerous contract to work for peanuts, going into horrendous debt to unlock the possibility of wealth in the space salvage game. Or at least a modicum of comfort in the modern space age.

The game is developed for the [Playdate](https://play.date) ([Wiki](https://en.wikipedia.org/wiki/Playdate_(console))), a small handheld console with some interesting and intentional limitations. It's as if an original Gameboy had a great processor (168 MHz!) and a relative ton of memory (16 MB!). The display is 1-bit monochrome, so it doesn't even draw some grays. It's 400x240 pixels and a small display at 2.7", so it's actually a pretty nice pixel density, but it does mean that you have to think hard about your sprite size vs. the overall screen size.

Anyway, [Marty wrote up his experiences](https://martymcgui.re/2025/09/16/stellar-scrapmn-is-hauling-on-the-playdate/), and he and I would love [a view and a rating](https://itch.io/jam/playjam-8/rate/3886395) if any of you are up for it. If you have a Playdate, you can sideload it by downloading the zip from itch and uploading it in the [sideload page](https://play.date/account/sideload/). If you don't have one, you can [download the SDK](https://play.date/dev/) and run it in the simulator.