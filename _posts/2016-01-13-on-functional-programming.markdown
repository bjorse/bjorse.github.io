---
layout: post
title: "On functional programming"
date: 2016-01-16 13:00:00
categories: development
comments: true
---

This post is like the title suggests, about functional programming. In the world of today where concurrenct systems is what we are developing, or at least heading towards, maybe object oriented programming (OOP from now on) is not the answer nor the solution, despite what we're grown up to believe. Concurrent programming in OOP is flawed with problems like race conditions, deadlocks, complex thread handling, and so on, due to mutable state. As [Jessica Kerr][jessitron] nicely put it in a [tweet][jk-tweet] almost 3 years ago: *GOTO was evil because we asked, "how did I get to this point of execution?" Mutability leaves us with, "how did I get to this state?"* (end quote). Immutability leaves us with a more simple code base, with fewer sources of errors. The only *real* reason we do prefer OOP, is because that's what we're used to, and we *believe* us to be more productive and less error prone in it, because we know it so well. From my point of view, we've already given OOP enough time to prove itself in this area, and it's obvious it doesn't fit well in the concurrent world of today.

## Prologue

Before we proceed, and if you're not yet a friend of functional programming, I just want to warn you. Because in the moment as you understand and appreciate the superiority of functional programming, there's no turning back. No seriously, I'm not kidding. You will never again gaze upon your current favourite object oriented language and utter the words: "wow, that's just wonderful. What a beautful piece of code, and what a nice solution to the problem". If any OOP language seems vital to your existence, I've now warned you about the consequences if you keep on reading.

If you're new to functional programming, or just want to refresh your knowledge about it, read [this excellent article][fp-article], and then come back here, because from now on I'll consider you knowing what functional programming is all about. However, I will of course use facts from that article to get my points across throughout this post.

## Productivity

I just want to talk about myself for a moment. First, I'm not *that* smart, I don't even got a college degree (or something equal) in anything. I don't fully understand most of the important (according to some) concepts of functional programming, like monads or gonads. I haven't even touched or looked at Haskell yet (not in an attempt to learn it anyway)! If I should get in an argument or discussion about functional programming with someone who knows most of the deeper details, I would probably fail to understand their arguments and lose badly. But *still*, I'm finding myself extremely more productive in [Clojure][clojure] than [C#][c-sharp], even though I've been writing code in C# for 5+ years, and in Clojure just a few months (and just sporadically on top of that). Why is that? I'm still writing unit tests and keep code separated in small sections, not losing any "signs" of quality, so there must be something else that I'm doing different.

For me, the answer is: even though you're following all the best practices in object oriented programming, you're just adding another layer of complexity upon the other while doing it. It's not just about the mutual state stuff, it's about how we write our code. Take C# for example, the language where I'm producing most of my code during the day. I find myself being several steps ahead (in my head) of what I'm actually writing code for in the moment. You know, "I'm going to implement feature X, but to do that I have to write these abstractions to hide data first so I can test it in isolation". Or, is it really in isolation? No, it's not. Due to following the best practices in C#, I'm using dependency injection (through constructors) and some kind of mocking framework to simulate the world around my implementation to get my unit tests to pass. That doesn't sound like isolation to me.

I know, I'm repeating some of the things mentioned in the article I linked to earlier, but this is a big part of my point here. If we're honest about what our functions need and what they produce, the code gets a lot more simple and is easier to reason about. Nothing strange about that at all. But, it has a huge impact on productivity, because if you can just focus on what your code is supposed to do, without encapsulations and abstractions, you'll gain productivity while doing it. *Getting shit done!*

## The web (front end)

Let's go on and talk about the web. Where in the front end do functional programming fit in? The obvious answer is: [React][react]. However, even though I'm a big fan of the idea behind React, I'm not really fond of its JavaScript implementation, even though it's still the *best* JavaScript library for rendering/controlling state in views at the moment (note: I *do not* dislike JavaScript, I just think there are other languages that are a better fit). A lot of people are talking about [Elm][elm] these days, which I unfortunatly haven't got around to try yet, but it looks promising (it's on my todo list after learning [Elixir][elixir]). For me though, the most clean solution where I'm still insanely productive, is the React wrapper written in [ClojureScript][clojure], [Reagent][reagent] (which uses [Hiccup][hiccup] to represent html). By using Clojure, yet another layer of abstraction has been removed for me when writing my code, reducing the amount of boilerplate code I'm forced to write as well, letting me to *only* focus on solving the problem without getting distracted. And in the front end on top of that! Observe that Reagent still maintains the speed of React, even claiming itself to *improve* the speed. Just plain amazing!

*Thanks to ClojureScript, we could use the same language on both the back end and the front end as well, if that's important to your cause.*

## Where to keep client side state?

Reagent has its own implementation of the Clojure `atom`, where it keeps track of its changes, and notifies when it's been changed (like the store in [Flux][flux]). So, a component who's using a `atom` gets re-rendered when its value changes. But it's still important to follow the functional principles. An component should never use a value from a store directly as its reusability would then be equal to none (and hides data/dependency on top of that). They should be pure functions: return what they should render based only on the provided value. If we provide a function as well which should be called when we're intending to *change* the value, our components gets extremely reusable (pure), and easy to reason about. The function we provide should be part of the action (dispatcher) that'll update the store for us in the end. A view should get states from the store on top of the hierarchy, and pass the data down to the components. For a simple Flux implementation using Reagent, [this article][reagent-flux] handles the topic well through code. If you want to take another step right away and start using components, [this article][reagent-components] will save you some time.

## Conclusion

Functional programming is the future, both in the back end and in the front end. I *really* believe it's a good thing with wrappers around JavaScript libraries (if the performance is kept or even improved) on the client side. The result is no bigger changes for the browser implementations, but with a *huge* impact on development through the ability to use a wider range of languages. Clojure is already a functional programming language while JavaScript is not, reducing complexity and the amount of boilerplate code. Reagent is a great example of that. The main problem with JavaScript, as I see it, is that while you *may* gain immutability through a [library](immutable-js), it's still a language with *way too many* ways of doing things, which may result in a diversified code base (concerning paradigms). Clojure has an appearant identity without multiple ways of doing things. Which is good, yes?

{% include twitter.html %}

[jessitron]: http://jessitron.com/
[jk-tweet]: https://twitter.com/jessitron/status/333228687208112128
[fp-article]: http://blog.jenkster.com/2015/12/what-is-functional-programming.html
[c-sharp]: https://en.wikipedia.org/wiki/C_Sharp_(programming_language)
[react]: https://facebook.github.io/react/
[elm]: http://elm-lang.org/
[elixir]: http://elixir-lang.org/
[clojure]: http://clojure.org/
[reagent]: https://reagent-project.github.io/
[hiccup]: https://github.com/weavejester/hiccup
[flux]: https://facebook.github.io/flux/docs/overview.html#content
[reagent-flux]: http://blog.cryptoguru.com/2015/12/react-flux-architecture-with.html
[reagent-components]: https://github.com/Day8/re-frame/wiki/Creating-Reagent-Components
[immutable-js]: https://facebook.github.io/immutable-js/docs/#/