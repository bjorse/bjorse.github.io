---
layout: post
title: "Project update #1: the first doubts"
date: 2016-01-21 22:00:00
categories: development
comments: true
---

This is silly really as I've barely begun to code, but I'm already having doubts whether I'm on the right track given the technical choices so far in this project. The thing is, even though dwelling deeper into native JavaScript (using React and Redux, for example) would be great to do (for several reasons), I'm not sure it's the thing to do for me right now. Because in all honesty, it feels like taking one step back in my own development. It's *not* because I consider myself better than someone else (because I really don't), it's just because JavaScript is really a crappy language with an obvious identity crisis and without several *important* features built into the language.

Don't get me wrong though. If this would be a project laid upon me through my work I would consider using JavaScript and React/Redux, but now that I'm given a totally free choice as it's my own free time project, I'm having a hard time considering putting myself through it all that's required to do this successfully. It feels like reinventing the wheel all over again (not that I actually invented the wheel, but you know, whatever...).

I'm quickly going to go through the areas I'm having trouble with.

## Immutability
Although I've known about all the positive consequences by using immutable data for a while now, a really nice thing occurred to me today: immutability has become a major part of my development style, and something that I have come to rely on. It's weird to realise this, because I'm spending most of my days writing code in a language that's not really associated with immutable data (C#). The reason it occurred to me now, I think, is because I'm expecting React and its friends to use immutable data by default. However, JavaScript does not support immutability natively, and that's a problem for me. Sure, there are libraries that will let me do this, but should it really be that way?

Immutability has given me a strong sense of personal security in a way that I'm sure the code I'm writing is going to behave the way it's meant to do. Isolated, and not affecting something else it's not supposed to affect. It's the same kind of security that I felt when I began to use TDD a few years back.

Like I said - JavaScript may support immutability through libraries, but I rather use a language that's built around it and encourages me to use it.

## Verbosity
Let's face it: developing code in React and Redux involves writing a lot of boilerplate code, which produces verbose code. I'm not going to go any deeper into this right now, as it's already pretty well explain in [this article][react-boilerplate], but this is something that's really bothering me.

I want to write code *as close as possible* to what I'm producing. I agree with André on this one.

Note: it's not just about syntax, it's about productivity as well, and logical decisions while coding. I want to produce features, not think about something else I might be missing out in the code I'm writing.

## Conclusion
Well, it comes down to choosing between going down the current JS path (maybe by using [Cycle.js][cycle-js] instead?), or switching to Elm or ClojureScript/Reagent. A tough decision that have to wait for a while until I have read up on Elm, and their respective compatibility with Elixir (the Channels in particular).

Don't worry though, I'm enjoying myself through all this anyway. At least I'm learning something new :)

{% include twitter.html %}

[react-boilerplate]: http://staltz.com/why-react-redux-is-an-inferior-paradigm.html
[cycle-js]: http://cycle.js.org/