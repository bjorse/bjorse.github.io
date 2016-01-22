---
layout: post
title: "Project update #2: project goals"
date: 2016-01-22 22:00:00
categories: development
comments: true
---

In this post, I will go through some of my thoughts and goals - what I really want to accomplish by running this (free time) project.

## Minimalism
As I've previously stated, I'm all about minimalism at the moment, and on several levels as well (not only syntax). In this project, these requirements has to be met:

* **server hardware requirements:** the application (web server) should be able to perform well on a Raspberry Pi 2. How to measure good performance and what's defined as good performance will be set later.
* **developer hardware requirements:** I should be able to use my 2GB RAM/32 GB flash drive laptop to write code and test the application. No large IDE (or something like that) should be required.
* **minimalistic syntax:** This is a tough one, but I would like to focus on the problem I'm facing, not battling syntax. Any functional language should do the trick. Elixir on the server side (initially) should be sufficient, the problem right now is front end language/techniques, which seems to come down to either ClojureScript or Elm at the moment.
* **minimal with time spent:** Due to not having *that* much time to spend on this project, I have to be productive and effective during coding sessions.

## Learning new technologies/languages
Of course, this is important. And it shouldn't be any technology/language, but something that's completely different to anything I've used before. Like, when learning Clojure, it was all new to me as I hadn't coded in any (real) functional language before, or even touched Java/JVM (I've *written code* in Java, but I've never developed any project from scratch). Learning F# doesn't feel worth it then, as my main language is (still) C#, and by learning Clojure I've already picked up a functional language, and due to this learning F# feels redundant (I would learn it if it was usable through work, which it's not at the moment).

Elixir is a functional language as well, but it feels new to me as its core feature is the Erlang platform, which probably will allow me to develop a high performing web server to run on a RPi2! That's *very* new to me. I've tried to develop a high performing web server before, but with node.js (on RPi1 though), and it did *not* perform well, even though it was well advertised throughout the web that it would!

## Features is secondary and should not limit development
Right now I'm thinking of developing some kind of social network. It's an idea generic enough to allow for many features to be pushed in - almost any cool feature fits in a social network! As this project will not become a product aimed for any end user, there's no requirement to add any real *valuable* feature, as the only user is me! If a feature would allow me to test out some new cool technology/language, I will then just do it by not being limited by the original project design/idea.

## Application lifetime - maintainability
However, some kind of maintainability should be required. I should be able to ditch a feature completely, but if a rewrite using any new technology is performed, the existing features should still work if they're still part of the application. That should be hard enough, right?

## Why are you doing this?
A legitimate question! If not all the statements I've gone through above is a sufficient answer to that question, then I may add that this is also a way to prove to myself that all this can be done as well, by choosing *new* technologies/languages, and doing things I haven't done before. I *really* believe in the technologies/languages I've chosen, and it will be fun to implement cool features using it. Considering the really limitied free time I have left over for this project, it will be awesome to see how far I'll come with the few hours that are available. Maybe it will become nothing of this? Who knows?

It's also thrilling to put my progress on public display through this blog, and later on, through a public repo on GitHub as well. And lastly, of course I'm totally enjoying myself doing this.

{% include twitter.html %}
