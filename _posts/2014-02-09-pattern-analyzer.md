---
title: Pattern Analyzer
tagline: So your code will never look like (mom's) spaghetti again.
layout: post
navid: pattern-analyzer
assetpath: post
---

I like to think I'm pretty okay at coding. I've done my fair share of research into design and architecture patterns, and I do my best to implement them whenever I can. As the years have gone by - I'm still basically a kid, so not many of them have - I've improved my ability to assess a problem and decide what sorts of software patterns should be applied to make it easiest to solve (and to scale!). But nobody's perfect, and there are a lot of times when I have missed opportunities for the implementation of a kickass pattern in my software. It always sucks to maintain code you know could be written more elegantly.

If it's not obvious where this is going, I'll make it so: a static code analyzer that could take a piece of software and suggest, or even apply, design and architecture patterns that would be beneficial for the programmer or team involved. AND, this just came to me: what if it was also a thing that could scrape a problem definition and suggest preliminary architectures for you? Man. That would make life easier ... although a lot less fun since I like thinking about that stuff. So yay! Aww.

Anyway, both of these would be pretty tough to implement, obviously. Especially the former idea; taking existing code and interpreting in a useful enough way to be able to suggest a new design pattern or architecture pattern sounds downright disgusting from a development perspective. But then again, I'm not much of a PL guy, so maybe it just sounds harder than it is. On the other hand, scraping a problem definition sounds fairly doable. Look for the buzzwords: "scalable", "global", "fast", "secure", "big data", "cloud", you get the picture. There are plenty of concepts in software architecture that could be applied to those words alone.