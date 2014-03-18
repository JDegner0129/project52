---
layout: post
assetpath: post
title: Chrome Macros
tagline: I'm starting to think I'm way too lazy.
navid: chrome-macros
---

Okay, full disclosure: I'd be *really* surprised if what I'm about to talk about doesn't already exist, but I don't really care. If it does, I've never seen it. I get annoyed when I have to do the same thing over and over - there's not much that encapsulates what software is all about better than eliminating annoying, repetetive tasks. With that said, there are plenty of times when I have to do the same, (fairly) routine thing over and over. Particularly within the realm of e-commerce, where I'm making certain orders multiple times. Websites like [Domino's](https://order.dominos.com/en/) do a good job of making it easier, but I still have to do a lot of the same click-through.

You already know what I'm going to say: wouldn't it be awesome if something could make that all go away? In my mind, it shouldn't be *fantastically* hard to write a Chrome extension (or a plugin for whatever inferior browser you may use) that could be triggered to watch your interaction with the DOM on certain pages, and later, imitate it. Essentially, I'm talking about writing something that could record and execute "macros" in your browser. Let's say I were using Domino's to place a pizza order. I could record a macro of me making a pizza order in the way I usually do, and from then on, I could just use that macro any time I wanted to get some pizza.

The most glaring downside to this is that it could easily bypass typical privacy of the user. The macro would have to know a **lot** about the user in many circumstances - sign in information, credit card information, etc. - although a lot of this information could be cached by the browser or your machine so that the macro itself doesn't get exposure to it. Macros would also have to change as frequently as the site(s) they monitor change. If I have a macro for ordering pizza, and Domino's re-designs their website, then I have to go through the trouble of re-capturing my macro. Of course, this doesn't incur any heavy overhead. I was going to have to learn how to use that new site anyway. Overall, I'd still be getting a huge gain out of using the macro (provided I order pizza pretty regularly).