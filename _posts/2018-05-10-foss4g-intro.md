---
layout: post
title: FOSS4G Starter Pack - Part 1
tldr: You use Esri GIS software on a Windows machine, but want more. This post aims to get you prepared to do all the fun FOSS4G things on a Windows machine that the Mac and Linux folks get to do without fuss
img: flow.jpg
thumbnail: flow_thumb.jpg
author: Christian Gass
---

> *I work with Esri GIS software on a Windows machine. I want to branch out into other GIS, but don't know where to start. Help?*

Yes!

At CivicMapper, we help our clients adopt geospatial tech solutions that are low cost, fit-to-purpose, and have the least strings attached. Sometimes we find that available commercial-off-the-shelf solutions, with the right implementation and negotiated price, fit the bill. Increasingly, however, we're finding that we can do better by our customers by implementing stacks built with/on available Free-and-Open-Source-For-Geo (FOSS4G) software.

With most of our team members having spent years working with Esri software in a Windows environment, the move to FOSS4G tech has been both liberating and challenging. The reality is that a lot of FOSS4G software built (particularly those built for the web) just runs with less fuss on Unix-based operating systems. However, we're not going to be ditching our PC hardware anytime soon.

 Getting a full-stack environment up and running *natively on a Windows machine* often requires a slew of work-arounds. These can be discerned by cobbling together bits and pieces of knowledge from all over the internet, which can be frustrating and a turn-off for those coming from "traditional" GIS environments. And while virtualization is always an option, that can be overkill for run-of-the-mill or exploratory GIS work (and it brings with it an entirely other set of new things to learn).

This post aims to provide a starting point and document some of the oddities that must be dealt with before doing all the fun FOSS4G things on Windows that the Mac and Linux folks get to do. This post assumes that you're:

* already somewhat comfortable with fundamental GIS concepts
* are coming from the Esri ArcGIS suite
* are working on a Windows machine
* aren't afraid to tinker a little bit

As with any software tutorial, check the date. If you're reading this a year after we've posted it, things may have changed!

With that, we're going to start at the bottom and work our way to the top:

# Command Line with [Cmder](http://cmder.net/)

## Why

The first thing I struggled with when moving to FOSS4G software was reading tutorials that required running any sort of command line operations. While I was used to writing Python to automate GIS operations (within the context of the ArcMap Python console using Esri's ArcPy library), running geoprocessing tools from command line was another animal entirely. 

Bash? Environment variables? Secure Shell? Git what? Why do the commands in these tutorials all start with a `$` or `#` sign? Where's the `C:\` prompt!? Why does that thing the tutorial says to run just give me the `* is not recognized as an internal or external command, operable program or batch file` error? And of course: "Why on earth would I run Python geoprocessing operations from the `cmd`, when I could just do from within ArcMap", so my thinking went.

What I quickly learned--other than that I had a lot to learn--was that the basic `cmd` interface for the regular Windows command console just doesn't cut it for any of this; and for all its improvements over the basic command console, PowerShell introduces its own set of complications that can be daunting for the beginner.

The reality is: there is a wide, wide world out there, GIS-button-clickers, and it's really quite exciting if you can use the command line.

## What

The day I discovered [Cmder](http://cmder.net/) was the day I stopped fearing the command line. Get it. It's a console emulator and it's wonderful.

You're going to want to get Cmder's "slightly bigger git-for-windows version", which gives you "all Unix commands ready in PATH". What does this mean? For one, it will be easier--much, much easier--for you to follow any FOSS4G tutorial written by/for Mac users.

As of the writing of this post, the *Windows Subsystem for Linux* provides another way to get that Unix experience on your Windows machine via a Windows Bash console. You're still going to want to run that console *from within Cmder*.


# Scripting with [Python](https://www.python.org/)

## Why

If you're running Esri ArcGIS Desktop or ArcGIS Pro, you already have Python 2 and/or 3 (respectively) installed. That software depends on those Python installs. Hopefully you're also using it to automate your geoprocessing--or at the very least recognize the power of doing so over point-clicking through ArcToolbox.

If you're one of the crazies running Esri CityEngine, you've also got another Python install (OK, well technically it's *Jython*) on your machine.

If you're also using ArcGIS API for Python, then (as of this writing) you've also installed Anaconda 3, a commercially-curated Python installation.

And, if you've installed QGIS (as we'll suggest in our next post), then guess what--it has its own Python installation!

## What

For everyday Python use with your new FOSS4G stack, however, it's nice to have a clean "global" install of Python on Windows that isn't going to be wiped when you upgrade any dependent desktop software. As of this writing, you should be using Python 3, and shouldn't really need Python 2 for this.

Since version 3.4.x (?) Python 3 installers for Windows handle making different versions of Python available through the command line relatively easy.

## What else

For your initial wade into this part of the pool, you'll likely be OK with just that one "global" Python install. But once you start building projects that rely on Python, you'll want to manage dependencies for those projects separately. To do that, you'll also then need to worry about virtual environments.

Those topics are probably better covered in-depth elsewhere, so I'll just leave it at this: Use [Pipenv](https://docs.pipenv.org/). It's a great tool that handles Python package installations in virtual environments for individual projects, without any fuss.

# Version Control with [Git](https://git-scm.com/)

## Why

If you're going to write scripts (and eventually, applications), absolutely do yourself a favor and use version control. It tracks changes to your code line-by-line. It lets you rollback your code, branch out different variations of it, merge those branches back in, and store everything in synchronized locations. It does a million other complicated things that you need not concern yourself with at first.

Using it will force you to start thinking about your small scripting tools as real projects in and of themselves, which, ultimately will make them more useful to you.

It also will give you a way to get many FOSS4G software projects onto your machine in a managed, repeatable way, without clicking through download pages on websites.

## What 

[Git](https://git-scm.com/) is a "free and open source distributed version control system" that you'll encounter in the wide world of FOSS, probably through [GitHub](https://github.com/). GitHub is a hosted version of Git: a remote location to which you can push your code, and others can see it (it also provides a bunch of project management tools related to your projects). [Bitbucket](https://bitbucket.org) and [Gitlab](https://about.gitlab.com/) provide similar hosted-Git solutions.

In the case of GitHub, they provide an excellent [GitHub Desktop](https://desktop.github.com/) client that lets you do most of the git things you'll ever need in a simple graphic UI (also works with the other hosted solutions). They also provide a nice [web tutorial](https://try.github.io), which is where I'd recommended starting if you're new to this.

If you've installed Cmder as recommended above, then you'll already have [Git-for-Windows](https://gitforwindows.org/) available at your fingertips from the command line.

## What else

When using Git, the folder which has version control on it is called a **repository**. It helps to start thinking about software projects as repositories with clearly defined scopes of functionality. So, say, that one geoprocessing script you have to automate that one thing you always do? Get it out of the folder of the last client project you used it in, and put it in it's own repository, with other repositories next door. Now it is its own living thing, with a complete history of its evolution.

When you're ready you can `git pull` FOSS4G projects onto your machine, open them up, tinker with them, learn, and contribute to the FOSS community yourself.

# To Be Continued

We've obviously left out some important things here: desktop GIS, databases, code editors, and notebooks. We'll tackle those in Part 2!


<br>
<hr>

*CivicMapper is a civic tech company that empowers civic organizations to utilize modern mapping technology for the greater good. Get in touch via [info@civicmapper.com](mailto:info@civicmapper.com).*
