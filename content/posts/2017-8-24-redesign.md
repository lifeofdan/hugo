---
title: "Redesign"
date: 2017-08-24
---
![Ruby Gems](/assets/img/wrench.jpg)

**It is that time again**. I quite liked the old layout of the site. However, I had installed jekyll (the backend of this site) on a different computer and couldn't figure out how to update the thing and it was many versions behind. So, I reinstalled jekyll to my main rig, deleted the old repo and then loaded fresh. (I am a nuke and pave kind of a guy...I admit it.) I now am using my own jekyll host but I have locked the version to github and have the new gemfiles that should allow me to update easily in the future. That is the hope anyway.

For a little bit the site will be transitioning as I migrate the old content back to the new site. This has been a good learning experience, however. I am getting a better understanding of how jekyll is supposed to work. Previously I think I had really mismatched a lot of configs and kind of jerryrigged things to work. I am now working with the default theme and trying to see how it actually works and connects everything together so that I only override when necessary and keep the base theme files updated. We will see how that works. I feel a bit constrained, so I might end up reworking the theme file myself instead of relying on the gem file. We will see. 

**##Update##**

I have finished the migration. **Wow, was that fast!** It was much easier than I thought it might be once I finally got my head wrapped around collections and how to link the collections. The introduction of the [liquid template language](https://help.shopify.com/themes/liquid/basics) into the index pages for each of those collections will speed up my ability to produce content as well, as they will automatically generate the links based on the titles. I was previously linking this content manually. 

The more I have done in updating the site the more I realise how much I was doing wrong previously. Sometimes, just because it *works* doesn't mean it is *right*. 

# MS Visual Studio Code

On a different note, I have done this entire migration using *Microsoft's* [vscode](https://github.com/Microsoft/vscode). While it is made by *MS* is is a genuine pleasure to use. It is every bit as good as something like Sublime Text or Atom (which is what I have generally used in the past) but it also has all the git integration as well. Now I know that you can integrate both of the other programs to use git, I mean, Atom was created by Github after all. But, vscode just seems to *show* me the integration in a way that I actually just decided to have a go using it instead of the terminal, which is generally my preferred method. And you know what? It worked really well, and really crazy easily. The fact that I can also assign keyboard shortcuts to these functions means I could simply press something like CTRL+ALT+S (or something I haven't actually done this yet) and it was stage my changes, then CTRL+ALT+C to commit, then CTRL+ALT+P to push. (I might have to rethink those binds as I already use them for other things, but you get the idead.) This is the first code editor I have been genuinely excited about using in a long time. Weird.

  

