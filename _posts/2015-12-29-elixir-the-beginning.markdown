---
layout: post
title: "Elixir: the beginning"
date: 2015-12-29 22:00:00
categories: development
comments: true
---

Alright. After reading countless blog posts and a few books about it, I'm finally ready to produce something noteworthy in [Elixir][elixir].

However, I'm not really set on my opinion on the language this far. After finding my love earlier this year in [Clojure][clojure], there's a lot needed to top that. First of all, the syntax is way too verbose for my personal taste. I know [José][jose-valim] found a lot of inspiration in Ruby, which is a language I fell in love many years ago, but today I cannot feel any of that love to be honest. In comparision to Clojure (sorry, but everything about Elixir will be compared to Clojure), it feels like writing a novel to accomplish something. Also, after doing a lot of [Lodash][lodash] (JavaScript), Clojure felt intuitive and a natural way to get something done because of that.

Secondly, the macro functionality (which should be part of any language), felt pushed into the language. In Clojure, it feels like a way more natural part of the language, as in a LISP, *[code is data][code-is-data]*. But if I know myself at all, I know that I will rise the macro system up to the stars in just a few blog posts :)

There are a lot of things I love about the Elixir syntax as well, like the pattern matching and the pipeline operator. The winning point for me however is not the syntax, but the Erlang VM. Concurrency made right from the beginning... This is where I think functional programming will be the winner, concurrent programming where scalability is important.

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
