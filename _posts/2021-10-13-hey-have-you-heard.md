---
layout: post
title:  "Hey, Have You Heard?"
date:   2021-10-13 18:35:38 -0500
categories: jekyll update
---

As Good Vibes continues to make progress on becoming an app used by many, the
costs of the upkeep for the server and database will also continue to rise,
as slow as it may be. Google has a neat little thing called AdMob, which
allows users to implement ads into their apps and gain money from people
using the app. Ads only give however many cents, but as the userbase increases
and more people use the app, the more the money will accumulate. This past
week I was tasked with implementing ads into Good Vibes so we could make a
little money and be able to help with the costs of maintaining the app.

Though it sounds easy, implementing it was a much harder task than anticipated.
The Google Ads SDK must be initialized before the app is run or else there would
be a RunTime error. Google Ads also has different types of ads, such as Banners
and Native ads, all of which have different properties and are initialized in
different ways. While following the tutorial, they used a Provider.value in the
runApp function (which runs the app) and used an instance of ad initialization.
Basically, the ad was instantialized and was able to be used anywhere in the app,
or so I thought. Since the app used a ChangeNotifierProvider, a subclass of
Provider that allowed listeners to be used so the app could change data in real
time, a MultiProvider needed to be used. After trying to use the Provider.value
and do a dependency check before initializing the banner ad, a
ProviderNotFoundException kept on popping up and I could not find a solution to
it no matter how hard I tried.

Eventually I was able to find a simpler implementation for the ads that did not
require another Provider. I was not able to implement it before our weekly
Wednesday meeting (since I found the solution during the meeting) but the fix
should be simple enough. This upcoming week will be about finishing the ad task
and potentially creating more analysis vectors for Firebase Analytics. A busy
week perfect for Fall Break...
