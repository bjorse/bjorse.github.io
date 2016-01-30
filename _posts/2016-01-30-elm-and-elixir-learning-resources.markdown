---
layout: post
title: "Elm and Elixir learning resources"
date: 2016-01-30 14:00:00
categories: development
comments: true
---

I thought that I would share some resources I've used so far when learning Elm. I will share some links to resources on Elixir as well, because I think that you'll (like me) want to use Elm together with [Phoenix][phoenix].

## The official documentation of Elm
Of course, [the official documentation][official-doc] is a great place to start. After getting a bit into learning the language, I now mainly use it mainly as a resource when reading other tutorials or when coding, because it really covers everything you need to know to get started up to an advanced level.

## The Pragmatic Studio Elm course
If you prefer watching video tutorials, there's a really appreciated course over at [The Pragmatic Studio][pragmatic-studio]. You get to watch three chapters for free, and then you have to buy the rest of the course. It may be worth the money if you rather watch videos than reading tutorials. I haven't watched this myself though, so I cannot give any personal review.

## The Elm compiler
This may sound weird if you're not used to it (I wasn't), but a great learning tool is the Elm compiler. It is *really good* at telling you what's wrong with your code. [This blog post][compiler-blog] tells you more about it. Bottom line is, don't only rely on guides and documentation, sometimes it's good just to explore the language on your own and let the compiler help you when it goes wrong.

## Getting started with front end development
When you're ready to actually produce some code, I really liked [this post][live-signup-form]. It goes through setting upp a live validated signup form in Elm. It covers the basics then goes through tougher parts, like communicating with the outside world. This helped me quite a bit.

## Game programming in Elm
[This blog post][making-pong] goes through how to code Pong in Elm. It's really fun if you want immediate feedback and want a break from coding web pages. If you want a tougher example to work with, I found [this article][elm-breakout] pretty interesting, where a programmer used to imperative programming tries out Elm by coding Breakout.

## The official documentation of Elixir
If you're not familiar with Elixir yet, you'll find the official documentation [here][elixir-doc].

## Elixir (Phoenix) and Elm
When you're ready for the next step (you want to use a high performance backend at this point), you'll want to use Elm together with Elixir/Phoenix. First, I recommend watching [this video][elixir-should-take-over-the-world] for getting inspiration and a bigger picture on things. Next, watch [this video][phoenix-with-elm-youtube] from the same conference to get a quick introduction how to integrate Elm with Phoenix. You may read [this blog post][phoenix-with-elm-blog] (there are several parts) that goes through the same stuff as in the video (it's written by the same person who did the presentation).

## Microservices
Today, everyone wants to use microservices. [This article][elixir-microservices] goes through how you get it for free with Elixir, and how the term is not really relevant in Elixir (call it a distributed system instead). [This article][elixir-umbrella] and the previous mentioned one, goes through how simple it really is to write a distributed system in Elixir, which is separated and scalable, but still offer very simple ways to communicate between tiny processes that are easy to deploy on their own, or together with other processes.

## State of Elm
I recommend you to fill out [this survey][state-of-elm] on the current State of Elm, which will provide us with some data later on how Elm is doing out there.

I hope you really enjoy learning Elm and Elixir like I do. I'm still just a novice in using this language, so if you got any tips I'll be happy to hear from you!

{% include twitter.html %}

[phoenix]: http://www.phoenixframework.org/
[frp-wikipedia]: https://en.wikipedia.org/wiki/Functional_reactive_programming
[frp-elm]: http://elm-lang.org/guide/reactivity
[official-doc]: http://elm-lang.org/docs
[pragmatic-studio]: https://pragmaticstudio.com/elm
[compiler-blog]: http://elm-lang.org/blog/compiler-errors-for-humans
[live-signup-form]: http://tech.noredink.com/post/129641182738/building-a-live-validated-signup-form-in-elm
[making-pong]: http://elm-lang.org/blog/making-pong
[elm-breakout]: https://github.com/Dobiasd/articles/blob/master/switching_from_imperative_to_functional_programming_with_games_in_Elm.md
[elixir-doc]: http://elixir-lang.org/
[phoenix-with-elm-youtube]: https://www.youtube.com/watch?v=MgFDZx1LmOE
[phoenix-with-elm-blog]: http://www.cultivatehq.com/posts/phoenix-elm-1/
[elixir-microservices]: http://blog.plataformatec.com.br/2015/06/elixir-in-times-of-microservices/
[elixir-should-take-over-the-world]: https://www.youtube.com/watch?v=X25xOhntr6s
[elixir-umbrella]: http://elixir-lang.org/getting-started/mix-otp/dependencies-and-umbrella-apps.html
[state-of-elm]: https://elm.brianthicks.com/state-of-elm/2016/survey/