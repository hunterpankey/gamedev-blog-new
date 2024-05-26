---
# This is a full listing of available Frontmatter options, available for any content (.md) file.
title: GameDev Shenanigans
layout: page
excerpt: # used for page excerpts and META (will be overwritten if SEO used below)
author: hunter-pankey # only displayed on Post lists and detail views. Defaults to _data/meta.authorURL
eleventyNavigation: # Required if want to display in Main Nav Bar
  key: main # "main" is required
  title: Home # as it will appear in the nav
  order: 1 # order to display in the nav (index = 1)
seo: # SEO values are used for OG and will overwrite 'title' and 'excerpt' above
  title:
  description:
  image: # used for OG:image and Twitter:image. Overrides default set in _data/meta.siteImage
hero: carousel # options: carousel, graphic, video, split (text & image)
heroSettings:
  height:
    mobile: # options = h-1/1 (default = full screen), h-1/2, h-1/3, h-3/4, h-9/10, h-48 (12rem, 192px), h-56 (14rem, 224px), h-64 (16rem, 256px)
    desktop: # leave blank to inherit "mobile" height (default = full screen)
  bg:
    color: # default bg-black
    image: home/pexels-mikhail-peace-939247406-20236201.jpg # relative to /assets/images/
    imagePosition: # options = bg-center (default), bg-left, bg-right
    video: # local relative /assets/video/, or full https://... if remote?
    opacityMobile: opacity-50 # options opacity-n, 5, 10, 15, 20, 25, 50, 75, 100 (default)
    opacityDesktop: opacity-75 # Leave blank to inherit opacityMobile, use same options as opacityMobile
  headingText: Making sense of game dev, <br />one package at a time.
  headingTextColor:  # default = text-white (can use any TailwindCSS text-[color]-[xxx])
  headingTextCase: # default = as typed - options: uppercase, lowercase, capitalize
  subheadingText: You actually R'd the F'ing M this time, but that didn't really help clarify anything.
  subheadingTextColor: # Leave empty to inherit headingTextColor or default (text-white) or use any text-[color]-[xxx]
  buttonText: To the articles! # no button generated if left blank
  buttonURL: /blog/ # full url required. Example: https://thisdomain.com/somepage/
  buttonTextColor: # leave blank to inherit from /src/_data/colors.buttonCustom or buttonDefault
  buttonBgColor: # leave blank to inherit from /src/_data/colors.buttonCustom.bg or buttonDefault.bg
  buttonBgHover: # leave blank to inherit from /src/_data/colors.buttonCustom.bgHover or buttonDefault.bgHover
  buttonBorder: # leave blank to inherit from /src/_data/colors.buttonCustom.border or buttonDefault.border
  carousel:
    images:
    - home/OladimejiAjegbile-frustredmanatlaptop.jpg
    - home/AndreaPiacquadio-frustratedwomanatlaptop.jpg
    - home/TimGouw-angrydeveloper.jpg
    - home/AndreaPiacquadio-screamingwoman.jpg
    - home/PetrGanaj-roaringlion.jpg
---