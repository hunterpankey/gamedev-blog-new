---
title: OK, What's Going On? # will be overwritten by SEO.title below
date: 2024-05-25
layout: page
eleventyNavigation:
  key: main
  title: About # as it will appear in the nav
  order: 2 # order to display in the nav
seo:
  title: OK, What's Going On? # overrides 'title' above on both Page and META
  description:
  image:
hero: graphic # options: carousel, graphic, video, split (text & image)
heroSettings:
  height:
    mobile: h-1/4# options = h-1/1 (default = full screen), h-1/2, h-1/3, h-3/4, h-9/10, h-48 (12rem, 192px), h-56 (14rem, 224px), h-64 (16rem, 256px)
    desktop: # leave blank to inherit "mobile" height (default = full screen)
  bg:
    color: # default bg-black
    image: home/pexels-mikhail-peace-939247406-20236201.jpg # relative to /assets/images/
    imagePosition: # options = bg-center (default), bg-left, bg-right
    video: # local relative /assets/video/, or full https://... if remote?
    opacityMobile: opacity-50 # options opacity-n, 5, 10, 15, 20, 25, 50, 75, 100 (default)
    opacityDesktop: opacity-75 # Leave blank to inherit opacityMobile, use same options as opacityMobile
  headingText: About GameDev Shenanigans
  headingTextColor:  # default = text-white (can use any TailwindCSS text-[color]-[xxx])
  headingTextCase: # default = as typed - options: uppercase, lowercase, capitalize
  # subheadingText: So what are we actually doing here?
  subheadingTextColor: # Leave empty to inherit headingTextColor or default (text-white) or use any text-[color]-[xxx]
---

- [GameDev is Great!](#gamedev-is-great)
- [The Complaint](#the-complaint)
- [The Solution](#the-solution)

## GameDev is Great!

Right? It really is a lot of fun to play with these components, put stuff together, and make some games! There's really nothing like putting in the hard work and making something cool looking and fun! That said, integration is really quite complex, sometimes, and there's a lot more to making a good or fun game than just throwing some models in a scene and clicking "Play". 

Say you're working with a character controller asset, trying to get a little bloop moving around on the screen or whatever. You might be getting some nice results from that character controller, initially, but at some point, you're gonna want to implement a cool, new game feature, like a speedup or a slow-mo condition, or a better jump (or a jetpack!), and you might have to do some work on programmatically setting some values in the controller. What's the best way to do that? Is that a feature in the asset, or do you have to write that code on your own? How do you do that in a way that won't make life hard in the future? Who can say?!

Well, the author of the character controller, for one. It would be very nice if the asset's documentation had some discussion on how to programmatically access critical values like move speed, jump power, or turning speed. And it would be great if it had some quality of life features, like grouping up those value changes into named conditions, and being able to switch between those conditions by using the name, rather than manually setting them.

## The Complaint
###### (Strap In, Folks! Bitterness ahead.) <!-- omit from toc -->

If you're lucky, the asset has those features, and if you're very very lucky, the developer of the asset has even written down some information on how that works. But only if you're exceedingly lucky has that written information actually made it into the documentation. Hopefully, at minimum, there's a PDF file sitting in your assets folder, probably converted directly from a Microsoft Word document, complete with default Calibri fonts, and so much spacing that you can barely see a sentence and a screen shot on the screen at once. 

Ideally, there would be a modern, categorized web site with documentation presented in a user-friendly way. If you're lucky, when the documentation leaves something to be desired, there'll be a Discord where you can lob out some questions and either get answers from the developer or exasperated guesses from others in the community. Lots of times, you're left with a PDF and an email address, which, good luck getting that issue solved!

## The Solution 
##### (Hahaha, no, it isn't.) <!-- omit from toc -->

Basically, as I go through things and work with an asset, if there's something weird about it that people ought to know that isn't covered in the documentation, then maybe I'll write it up, and maybe some people will even see it! Hopefully someone will get some mileage out of this, and if I can learn some new stuff along the way, then that's even better.

So go [check out the posts](/blog)!