---
layout: post
title: "My new project"
date: 2016-01-20 22:00:00
categories: development
comments: true
---
So, the time has finally come to launch my new personal project. Its purpose is solely for my own development - a place where I may try out new (for me) technologies, but still have something to work on, and something to maintain. So, I'm thinking it would be fun to develop some features and then force myself to switch/add technologies at times, just to learn by doing. The project is going to develop locally on my machine at first, but when the time comes it will be a public repo on GitHub, available for anyone. We'll see, maybe I'll get to know other developers with the same thoughts as me, and even collaborate on the project with the as well? Time will tell.

These are some of the guidelines I'm going to follow during this project:
* separate code early and do not mix stuff by thinking it will be parted later during some refactoring session (it will probably not happen, since this is a free time project)
* prepare the system with features, but do not finish all the way until necessary. For example, the system should be built around some kind of authorization process, but the authentication method might not be implemented until some time later.
* use static/local data as far as possible. Wait until the very last to persist data in any kind of database to see where it fits - [polyglot][polyglot]?

The technologies I'm going to use is:
* [Elixir][elixir] with [Phoenix][phoenix]
* [React][react] and [Redux][redux]. I thought I would use plain JavaScript at first to learn it well, and then perhaps add some [ClojureScript][clojure] (by using [Reagent][reagent]) later to mix it up (or even replace some features?)

This feels good and I'm going to let it stay there at first, and then decide on where to take the project later when I'm getting somewhere. Let me know if you're interested in collaboration on this one - it would be fun to work with someone else! There will be blog posts like these to come in the future with project updates!

{% include twitter.html %}

[polyglot]: http://martinfowler.com/bliki/PolyglotPersistence.html
[clojure]: http://clojure.org/
[react]: https://facebook.github.io/react/
[elixir]: http://elixir-lang.org/
[phoenix]: http://www.phoenixframework.org/
[redux]: https://github.com/rackt/redux
[reagent]: https://reagent-project.github.io/
