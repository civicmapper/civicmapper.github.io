---
layout: post
title: DIY FOSS-4-Geo Starter Pack
img: default.jpg
thumbnail: default-thumbnail.jpg
author: Christian Gass

---

*tl;dr: You use Esri software on a Windows machine, but want more. This post aims to get you prepared to do all the fun FOSS4G things on a Windows machine that the Mac and Linux folks get to do without fuss.*

---

> I work with Esri GIS software on a Windows machine. I want to branch out into other GIS, but don't know where to start. Help?

Yes!

At CivicMapper, we help our clients adopt fit-to-purpose geospatial tech solutions that are low cost and have the least strings attached. Sometimes we find that available COTS solutions, with the right implementation, fit the bill. Increasingly, however, we're finding that we can do better by our customers by implementing stacks built with/on available Free-and-Open-Source-For-Geo (FOSS4G) software.

With most of our team members having spent years working with Esri software in a Windows environment, the move to FOSS4G tech has been both liberating and challenging. The reality is that a lot of FOSS4G software built for the web just runs with less fuss on Unix-based operating systems...however, we're not going to be ditching our PC hardware anytime soon.

 Getting a full-stack environment up and running *natively on a Windows machine* often requires a slew of work-arounds. These can be discerned by cobbling together bits and pieces of knowledge from all over the internet, which can be frustrating and a turn-off for those coming from "traditional" GIS environments. While virtualization is always an option, that can be overkill for run-of-the-mill or exploratory GIS work (and it brings with it an entirely other set of new things to learn).

This post aims to provide a starting point and document some of the oddities that must be dealt with before doing all the fun FOSS4G things on Windows that the Mac and Linux folks get to do. This post assumes that you're:

* already somewhat comfortable with fundamental GIS concepts
* have come the Esri ArcGIS suite
* are working on Windows
* aren't afraid to tinker a little bit

As with any software tutorial, check the date. If you're reading this a year after we've posted it, things may have changed! 

# Desktop GIS

## Why

First up, your desktop GIS alternative: QGIS. 

QGIS 3 was just released this year. If you've used ArcMap within the last 10 years, you'll find far more than parity now.

## Why

...

# Scripting with [Python](https://www.python.org/)

## Why

If you're running Esri ArcGIS Desktop or ArcGIS Pro, you already have Python 2 and/or 3 (respectively) installed. That software depends on those Python installs. Hopefully you're also using it to automate your geoprocessing--or at the very least recognize the power of doing so over point-clicking through ArcToolbox.

If you're one of the crazies running Esri CityEngine, you've also got another Python install (OK, well technically it's *Jython*) on your machine.

If you're also using ArcGIS API for Python, then (as of this writing) you've also installed Anaconda 3, a commercially-curated Python installation.

And, if you've installed QGIS like we suggest above, guess what--it has its own Python installation!

## What

For everyday Python use with your new FOSS4G stack, however, it's nice to have a clean "global" install of Python on Windows that isn't going to be wiped when you upgrade any depdendent desktop software. As of this writing, you should be relying on Python 3, but have the flexibility to also use Python 2.

Since version 3.4.x (?) Python 3 installers for Windows handle making different versions of Python available through the command line relatively easy.

(We'll post some gists of windows configs and environment settings that make this all workable)

## What else

Always use Python virtual environments for individual projects. `pipenv` is a great tool to handle both python package installations in virtual environments for individual projects.

# Git for Windows & GitHub Windows Client

# Database

PostgreSQL w/ PostGIS

# Command Line

## Why

The first thing I struggled with when moving to FOSS4G software was reading tutorials that required running any sort of command line operations. While I was used to writing Python to automate GIS operations (within the context of the ArcMap Python console and through their powerful ArcPy library), running geoprocessing tools from command line was another animal entirely.

Bash? Environment variables? Secure Shell? Git what? Why do the commands in these tutorials all start with a $ sign? Where's the `C:\` prompt!?

What I quickly learned--other than that I had a lot to learn--was that fundamentally the interface for the regular Windows command console just doesn't cut it for any of this; for all its improvements over the basic command console, PowerShell introduces its own set of complications.

## What

The day I discovered [Cmder](http://cmder.net/) was the day I stopped fearing the command line. Get it.

You're going to want to get Cmder's "slightly bigger git-for-windows version", which gives you "all Unix commands ready in PATH". What does this mean? For one, it will be easier--much, much easier--for you to follow the FOSS4G tutorials written for Mac users.

As of the writing of this post, the recently out-of-beta *Windows Subsystem for Linux* provides another way to get that Unix experience on your Windows machine via a a Windows Bash console. You're still going to want to run that console *from Cmder*.

(We'll post some gists of Cmder configs that make running different shells and calling scripting languages easy)

# Connections

SSH, Tunnels, Magic


<br>
<hr>

*CivicMapper is a civic tech company that empowers civic organizations to utilize modern mapping technology for the greater good. Get in touch via [info@civicmapper.com](mailto:info@civicmapper.com).*
