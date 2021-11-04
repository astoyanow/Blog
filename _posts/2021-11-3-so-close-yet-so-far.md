---
layout: post
title:  "So Close Yet So Far"
date:   2021-11-04 18:35:38 -0500
categories: jekyll update
---
Favoriting quotes is still a work in progress. The good news is that I am really
close to getting it done. All I need to do is create functions for writing and
querying data between the local database and the Firestore Firebase. I read
through the application state over and over again and looked at the files
in order to get a good understanding of the functionality of the databases within
the application. With favoriting quotes, the local database will be used more
often rather than just being the place that holds the good vibe and being
used by Firebase to get the quote. Now it will actually have to be checked
in case someone favorited the quote.

I also worked a little bit on the ad implementation. Instead of using test ads,
we are now moving to using real ads while registering our devices as test devices
so that we do not get in trouble for invalid advertisement use and get the
Disco Tray account suspended. AdMob does not let you use the Ad Units for your
application until you provide them with your payment information (I assume it is
just used for when they give you the payout based on the ads) so we are currently
in the process of getting the Ad Units to start working.

This next week will be a sprint to get this favoriting thing working. I do look
forward to getting everything to work nice and smooth and avoid breaking the
data in the app. It has been two weeks too long to have been working on this
task so I will be working diligently to get it done.
