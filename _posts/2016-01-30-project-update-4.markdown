---
layout: post
title: "Project update #4: learning Elm"
date: 2016-01-30 12:00:00
categories: development
comments: true
---

I haven't really worked on the project for several days, as the little free time I've got is spent on reading up on and learning Elm. For every new concept/feature I get to know and understand, the more I adore and appreciate the language. The only thing that bugs me so far is the necessary evil to interop with JavaScript code (when using [Phoenix][phoenix] at least). It's made possible through ports, which generates some boilerplate code, but hey, you can't get everything right? At least the code I'm writing in Elm is easy to read and refactor.

My [sucky computer][hp-stream] (that's entirely set up for web development) is still comfortable with what I'm doing and is able to keep up with me, which is a good review for Sublime Text 3, Elixir, and Elm (and [Linux][cbpp])! I can write code and do stuff without the system getting into any of those endless loading loops that's associated with some other operating systems and/or IDEs. Chrome is however, as you all know, really demanding on resources and takes up about 1 GB of RAM alone just when newly launched in idle state, and its memory usage only goes up from there. That may become a problem, because when learning new technologies/languages, you have *a lot* of tabs on various subjects open at the same time, and that seems to be the only possible limitation of this computer so far. *However*, I haven't reached the end on resources yet, because I still got around 1 GB of RAM to use (if you include the swap). The worst case scenario is that I've to switch to another less demanding browser, but I don't see that need to happen anytime soon. The cool thing is that the stuff I'm using for development (Sublime Text, Elixir, Elm, brunch) claims almost no resources at all.

I'm having trouble with the [Elm integration with brunch][elm-brunch]. For a while, I didn't get the hot reloading to work at all, but the 0.4.2 patch of elm-brunch fixed that. Now, I got the ["Unexpected end of input"][elm-brunch-bug] problem instead. It happens pretty often, and I usually re-save my file until the compilation process succeeds. When reading about it on the web, it seems that brunch tries to read the compiled Elm file (as JavaScript) before it's done, which results in the given error. If any one got a tip to get around this, please advice me on it. It may be limited on Linux setups though, as its functionality to notify on file changes seems to implemented differently than on OS X (the web says so, at least, I know nothing on that subject). Hopefully a fix will arrive to get this out of my way for good soon.

{% include twitter.html %}

[phoenix]: http://www.phoenixframework.org/
[hp-stream]: http://store.hp.com/webapp/wcs/stores/servlet/ContentView?eSpotName=Stream11&storeId=10151
[cbpp]: https://crunchbangplusplus.org/
[elm-brunch]: https://github.com/madsflensted/elm-brunch
[elm-brunch-bug]: https://github.com/madsflensted/elm-brunch