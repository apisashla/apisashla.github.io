---
layout: post
title: "Work in Progress!"
date: 2021-07-04 09:45:00 -0400
author: ash
categories: test
comments: true
---
Hi! I've come back to this blog after a long absence, and because of changes made on the backend of Jekyll, Ruby, github pages and so forth, I'm thinking the best way to tackle this may be to rebuild the site. Comments will be lost, but posts may not be (I say "may not" because I've copied them but may decide to simply archive them for my own use and remove them. We'll see what I decide is worth putting back up.)

The easiest thing would be to rebuild using github pages and Jekyll again (a straight upgrade won't work very well, because github doesn't yet support the newest versions of Jekyll, which causes things to break because Jekyll now relies on newer versions of Ruby.) I may, however, decide to go with a different hosting provider. Not sure yet. It'll still be deployed to the same domain name, so don't worry about that part.

Thanks for bearing with me, and see you on the flip side.  

\[edit 7/7/21: I realize now I should clarify, if you've tried to leave a comment and haven't been able to, that's because comments aren't working right now because somehow bringing Jekyll up to date broke Staticman. I've spent a while trying to fix it and this was one of the primary reasons I decided to blow the whole thing away and start over.

Also, just to give you an idea of what I'm thinking so far, I think I've decided I'm going to try building the site in another static site generator. Per my limited research, [Eleventy](https://www.11ty.dev/) would be the logical next step, and everyone raves about how easy it is to learn, but to be honest at first glance I hate how un-opinionated it is about everything - where to put things, what templating language to use, whether and when to use JavaScript, and so forth. I understand this provides flexibility for ~~monsters~~ people who actually need to use multiple templating languages for whatever godforsaken reason, but if I'm going to have to fiddle with it to make it work anyhow (i.e. changing over config markup formats from yaml to json, manually [adding back functionality to Liquid](https://24ways.org/2018/turn-jekyll-up-to-eleventy/) to get it to do the same stuff as it used to do in Jekyll) then I might as well just start over with something saner anyway. 

Consequently, I'm leaning toward [Zola](https://www.getzola.org/). Partly this is just bias toward Rust, as I'm one of those people who's infatuated with Rust conceptually without really having any expertise in it to speak of. (The [handbook](https://doc.rust-lang.org/book/)'s just really cool, okay? I like how they explain things.) But more importantly, it's because, like Jekyll, it is opinionated about how one does things and there is usually one correct way to get it done, but unlike Jekyll, it is not particularly complicated to install, use, or maintain. Hopefully. Maybe I'll try it and hate it and come around to something else, but I think this might be the best way to go for me.

I also plan on switching my hosting provider to [neocities](https://neocities.org/), honestly because they cater to individual users looking to build and customize static websites, rather than developers demonstrating their portfolios or web startups advertising their fancy new apps (although it is a well-maintained static hosting provider and therefore theoretically capable of both.) It's also, to be blunt, not owned by a gigantic conglomerate and has extremely reasonable [terms of service](https://neocities.org/terms) - not permissive enough to enable abuse or harrassment, but no more restrictive than it needs to be, and specifically permits non-work-safe content and affirms its commitment to freedom of expression.

There's one problem, though - I can generate my content locally and simply upload it directly to neocities, but Staticman and similar comment systems for static pages require a public Git repository to work, so I'm stuck in this awkward position where I'm moving away from Pages but am still obligated to host code on Github. I'm hoping to have a solution for this soon, as an Internet acquaintance of mine is in the early stages of spinning up a [Gitea](https://gitea.com/) server for members of the Mastodon instance I'm on. Staticman, of course, doesn't support Gitea, but there is another, somewhat similar system called [Vssue](https://vssue.js.org/) that does. We'll see how this develops. I may be able to get my SSG and web hosting changes sorted out before my Git hosting changes.

All this is to say - new and hopefully better things are in the works! Stay tuned and good night.\]
