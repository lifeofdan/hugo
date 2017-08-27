---
title: "AMD, Linux, Thoughts on Distros"
date: 2017-04-24
tags: ["gaming"]
--- 
![Linux Gaming Problems](https://itsfoss.com/wp-content/uploads/2016/09/Linux-Gaming-Problems.jpg)

Image linked from [itsfoss.com](https://itsfoss.com/linux-gaming-problems/)

Okay, so my last post was a bit frustrated. I continue to exist in that state of being. :P

This Christmas I built a new computer. Nothing super fancy, but a very nice upgrade for me from a i5 2500k to now running a e3 1230 v5 Xeon processor. I am also running an AMD R9 Fury graphics card. The rationale for the new graphics card and CPU was to run a Windows VM for my gaming with GPU Passthrough. I considered writing up a tutorial on how I accomplished this under Neon but I think I would need to do it a couple more times before I was comfortable doing so. I digress... This computer did okay. I had 16gb ram (that is definitely the minimum you want if you are to attempt this) an NVIDIA GTX 970 and an AMD R9 Fury, the NVIDIA card was for Linux and the Fury was for the Windows VM. This worked rather well. Unfortunately I knocked a nice cold beverage into my computer...My desktop was on the floor beside my table, the liquid came down through the top fan vents. Anyway, it could have been much worse. The only thing that got ruined was my GTX 970! While that is a costly mistake, it wasn't the end of the machine. However, in this process my hard drives became corrupted and I couldn't boot. Bye, bye Neon install. 

The next couple of weeks had me distro hopping. One thing I knew for certain was that I wanted to go back to Gnome. I enjoyed my time with KDE Plasma, and there are DEFINITELY great things happening there, but there were little niggles that I really just didn't want to put up with anymore. You can see my previous post to see what those were. 

So, requirements:

1. Gnome
2. Be able to run the apps I need. 
	* Discord
	* WPS Office
	* Wire
	* Text Editor (I'm not picky.)
	4. Skype (For work)
	5. Keepassxc or something similar

Almost any distro could supply those needs, and the distros I tried would have had all of these things. Unfortunately, I play games. This is where all my troubles lie.

3. World of Warcraft
4. Guild Wars 2
5. Steam Games (No troubles here)

As you can see, two of the games I love to play require WINE. Because I have an AMD GPU I also need to use [**Gallium Nine**](https://wiki.ixit.cz/d3d9) in order to have any decent frames and playability. That means I also need to Gallium Nine patched version of wine. So...I tried:

## openSUSE Tumbleweed

I love openSUSE. It was the first distro that I ever used with any success. I enjoyed it a LOT. However, it has been a long time since I have used it and things did not go as smoothly as I had hoped. I installed the gallium patched stuff, but the maintainer seems to have gone afk and I there are new ones that have picked stuff up, but the install just didn't work well. The graphics were bad and I couldn't get the patched wine to work. I also had a lot of issues with the firewall in openSUSE. It was not UFW. Lawl.

## Fedora 25

I like the idea of running Fedora. While opensuse was the first distro I really had any success with, Fedora was the first distro I ever used, or more specifically Red Hat. I got a CD of Red Hat back in 2003. It was actually around the time that fedora became a thing. I installed Red Hat but quickly found out online that I should be running Fedora Core. I installed and played around, but I didn't really use it for long, it was more of to see if I could do it. It was cool. 

When trying to use it for this aspect, it failed. I tried installing gallium patched wine and the mesa from COPR repos, but I didn't have any success. I got things to run, but it was unplayable. I now think it was probably a MESA problem, but I decided it wasn't work my time and reformatted.

## Arch/Manjaro/Antergos

Everything I needed was here. But due to knowing several people recently that have had system issues due to graphics driver problems, I didn't really feel as comfortable with Arch as I have in the past. Don't get me wrong, I have actually been running Arch with little to no problems for the past three years. However, I am also a constant distro hopper, which I believe has mitigated many problems that I could have run into.

## Solus

Let me say, I LOVE Solus. The desktop just WORKS so well. I didn't go with Budgie, I used the info on the website to go with Gnome-Shell. Since doing this Solus has even released a Gnome-Shell .iso, which I really, really want to try. Solus was **blazing** fast. It booted insanely quick and everything was smooth as silk. The hype is real.

Also, Steam integration on that platform is amazing. Games played WAY better there than on Neon. I did have some issues with my Steam Controller, but that all came down to user error. 

Unfortunately, one of the things that makes Solus great, also makes it hard in my use case. Solus does not put things in the repos that is already there. For instance, Wine Stable is in the repo. But I don't need Wine Stable, I need a Gallium Nine Patched wine...yeah...good luck with that. The whole philosophy of Solus says to have one thing to do a task so that the desktop isn't riddled with package dependencies that then break when using a different program that uses a different dependency. It is a good philosophy...but it makes it impossible to play the games I play.

I did briefly try making the patches to my system myself. I go them "installed" but I could not select the check-box to get the gallium patch activated on wine. I believe I didn't have MESA patched properly, or I needed to install the mesa first, and then the wine patched version, but I had a raid the next day and didn't have time to fiddle with it anymore. I will probably find myself back on Solus if I can ever figure this out because I loved every second on it. (Their IRC is awesome.)


## Ubuntu-Gnome

This is where I find myself. Ubuntu Gnome. It technically has everything I need. The drivers I needed for the patched mesa & wine were a ppa away. All of my software was easy to install. Everything just works...but it is boring. 

Everything works, but there is nothing exciting about this install. It runs well, but it doesn't blow my mind with its speed. It boots pretty fast, but not as fast as Solus. Everything installed, but I did have to mess with dependencies. Everything works, but it isn't rolling. There are little crashes but nothing that really effects my work. (Plymouth crashes, there used to be Nautilus crashes but I fixed that.) Some other crashes to programs happen occasionally as well, but nothing system wide or anything. Basically, there are little bugs, but nothing terribly earth shattering...so why am I discontent?

## Where will I be down the road?

I don't know. For the present I am too busy to be reformatting my machine to mess with things. If I can get my hands on another SSD I might try throwing Solus on it and trying to fix my niggles on it. Solus is where I want to be. I like the team's vision of things just working. I like that I can actually just go talk to the lead developer in IRC. I like their software center. I like how fast everything is. I like how they have updated Steam integration, If I can get my games going, I will stay there. 
