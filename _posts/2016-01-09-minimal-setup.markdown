---
layout: post
title: "Minimal setup"
date: 2016-01-09 21:00:00
categories: development
comments: true
---

For long, I've been aiming for minimalism when it's about my hardware/software development setup. Coming from the .NET world where Visual Studio is used for everything, I've just like many others grown tired of the idea of a *huge* IDE that has the facilities to do almost anything. Such an IDE becomes really clumpsy and slow real fast. Nowadays, I want my setup just like I want my code; small parts that does *one* thing really well.

I thought that for my next project (to learn/explore Elixir), I would see how far I could push the minimalism and still maintain productivity. I thought about just running a virtual machine on my Macbook Pro at first, but it would be funnier to try with really crappy hardware to be limited for real. So, finally my blue [HP Stream 11][hp-stream] comes to valid use. With a 32 GB flash drive and 2 GB RAM, it's for sure not made for local development, and is thus perfect for this experiment.

First, I had to decide which OS to run. Windows is out of the question (I simply don't like it and it consumes too much resources), so it comes down to choosing the right Linux distro (which is fine by me, because I *love* Linux). So I needed a distro which favors minimalism and is lightweight. I tried [Elementary OS][elementary-os] first, which is a personal favourite. However, after evaluating it for a while, it became obvious it was way too consuming. It needed around 1 GB RAM just when idling, and without a dedicated graphics card (or a better chip), the GUI was way too slow to be usable for long. This was a very sad moment, because the OS X feel of the GUI felt strongly appealling to me. Next, I tried my new (after this experiment) favourite lightweight Linux distro: [Crunchbang++][cbpp]. Consuming around 150-200 MB in RAM while in idle state, it leaves a lot of memory for other things that I may need. With a very sleek GUI as well with *just* the stuff I need to use, it's perfect. Seriously, I could use this professionally. The only problem is that it frankly hates my Broadcom wireless card, with it dropping the connection and just stops working sporadically. I had problems installing it at first as well as it took a good while to find the appropiate drivers. But it seems worth it!

Next up, I had to decide which text editor to use. I have two major requirements that just *has* to be met when it comes to editors: vim support and speed. For git support and other stuff like that, I'll just use the terminal, and ideally such support wouldn't be included in the editor at all (it may slow down the performance). The obvious choice here is [Sublime Text 3][sublime-text]. I wanted to go with [Light Table][light-table] at first as it served me really good while learning Clojure, but this time around I wanted to try something else. I considered [Atom][atom] for a while, but the last time I used it in Linux (been a while since now though), it was really slow at times, making it not even an viable option at this point. So, back to the roots and Sublime Text it is! Consuming only ~100-150 MB RAM, no matter how many files I may have opened it seems, its performance is high above my expectations. What an amazing editor! It's blazing fast as well.

Now, it comes down to me to not let this setup become bloated. For music (Spotify), email, Facebook, Twitter, Skype, and so on, I'll just use my phone. Why go through the pain of installing it all on this machine, when they're all already available on my phone? Email and social media is reached through the web as well.

What really amazes me though, is how little resources that are actually needed to get started writing some code for the web, without spending a huge amount of time looking at loading spinners. Barely nothing at all to be honest! Next up is to install all the dependencies and then get started with producing the code! I'll come back with some news when there's something interesting to report ;)

{% include twitter.html %}

[hp-stream]: http://store.hp.com/webapp/wcs/stores/servlet/ContentView?eSpotName=Stream11&storeId=10151
[elementary-os]: https://elementary.io/
[cbpp]: https://crunchbangplusplus.org/
[sublime-text]: http://www.sublimetext.com
[light-table]: http://lighttable.com/
[atom]: https://atom.io/