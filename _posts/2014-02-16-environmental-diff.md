---
title: Environment Diff
tagline: Sometimes, diffing code just isn't good enough.
layout: post
navid: environment-diff
assetpath: post
---

I love diff tools. It's really handy to be able to compare a file to its past self, or to another file, and instantly clarify the differences. There have been numerous times when our Design Studio project has broken after the push of a new build, and without fail, my first instinct is "check out the diff." It can be incredibly easy to pinpoint your problems when you're looking at the differences between a working model and a, well, not-working model. But sometimes it's not quite as easy as that.

Sometimes you need to be able to "diff" more than just files. Sometimes you've got to be able to diff entire environments, platforms, or whatever else may stand in the way of your codebase and the actual piece of software you deliver. A number of different things can go wrong without your code being any different. Today, I worked for a few hours trying to figure out why the master branch of our code works fine on my Windows machine and on the Linux deployment server, but not on my MacBook Air. I even tried *multiple* branches of our codebase, and went so far as to delete my local working tree and re-clone the repository to make sure I wasn't crazy.

Well, I wasn't. Our project makes use of a Less precompiler to compile CSS files, and as it turns out, I was using the *Ruby* version of `lessc` instead of the *Node.js* version. For whatever reason, the compilers are different. Because of this, none of the Less was being precompiled by Django before serving the web app. Isn't that great? It made me think, "man, wouldn't it be awesome if Git or some other tool had taken a snapshot of my environment, too?", and I think an idea like that could be immensely useful to people working on teams. No more wondering why your code works on your machine, but not your teammates'. How awesome would that be? Obviously, it'd be ridiculous to diff *everything* on your machine - you'd probably want to have some sort of settings file to decide which things you diff. But if you could specify compilers and other dependencies in your diff tool, it could catch all sorts of things existing diff tools don't.