---
layout: post
title: "Elixir: the beginning"
date: 2015-12-29 22:00:00
categories: development
comments: true
---

Alright. After reading countless blog posts and looking through a few books about it, I'm finally ready to produce something noteworthy in [Elixir][elixir]. Usually, my way to get to know new stuff is just by using it, but in this case I actually wanted to get some basic knowledge before getting started, in an attempt to see if it gets me faster ahead.

Elixir is a functional programming language, which is the only type of languages I'm touching these days, at least when it's about learning something new for my own development (long story short: tired of OOP and excited about FP). However, I'm not really set on my opinion on the Elixir syntax so far. After finding my love earlier this year in [Clojure][clojure], there's *a lot* needed to top that. First of all, the syntax is way too verbose for my personal taste. I know [José][jose-valim] found a lot of inspiration in Ruby, which is a language I fell in love with many years ago, but today I cannot seem to find any of that love to be honest. In comparision to Clojure (sorry, but everything about Elixir will be compared to Clojure), it feels like writing a novel to accomplish something (not a fan of words in languages, like `do` and `end`). Also, after doing a lot of [Lodash][lodash] in JavaScript a few years back, Clojure felt intuitive and a natural way to get something done because of that.

Secondly, the macro functionality (which should be part of any language), feels pushed into the language. In Clojure, the macros is a way more natural part of the language, as in LISP, *[code is data][code-is-data]*. But if I know myself at all, I know that I will raise the macro system up to the stars in just a few blog posts, be sure about that :)

Finally, the last thing that bugs me so far is the possibility to omit parentheses in function calls. I can cope with `some_function()` being replaced with `some_function`, but being able to type `sum a,b` instead of `sum(a,b)` really bugs me. The reason is because it confuses me, and it will confuse others. It's also one of those things that developers in the same project will use differently (unless some code guidelines are in place early on), leaving the code base inconsistent. Perhaps it's Clojure that has made me parentheses-friendly, but I think the code gets better readability that way. Maybe it'll become clear for me along the way why it's made this way and I'll buy it, but right now I can't see why.

There are a lot of things I love about the Elixir syntax as well, like the pattern matching and the pipeline operator. The winning point for me however is not the syntax, but the Erlang VM. Concurrency made right from the beginning. This is where I think functional programming will be the winner, concurrent programming where scalability is important.

Just thought of something: of course I will be writing for the web, and perhaps I will find a way to use ClojureScript on the client side. If it's not already made, maybe I'll code a [Phoenix][phoenix] wrapper in ClojureScript, and use [Reagent][reagent] (a gorgeous [React][react] wrapper) to use functional programming on the client side as well. Yeah, that sounds good. Let's do that first :)

{% include twitter.html %}

[elixir]: http://elixir-lang.org
[clojure]: http://clojure.org
[jose-valim]: https://twitter.com/josevalim?lang=en
[lodash]: https://lodash.com
[code-is-data]: https://en.wikipedia.org/wiki/Homoiconicity
[reagent]: https://reagent-project.github.io/
[phoenix]: http://www.phoenixframework.org/
[react]: https://facebook.github.io/react/
