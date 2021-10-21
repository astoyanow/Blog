---
layout: post
title:  "My Favorite"
date:   2021-10-20 18:35:38 -0500
categories: jekyll update
---
This past week was a small but needed break from school. Fall break!! I finished
up the implementation of test ads into the app which was pushed. It is time to
use real ads for the app even in beta testing so that we can start to get some
income. I will have to include the app's actual application unit ID for the
units rather than the test ad unit IDs in order for actual ads to show up. I will
also have to make sure that ads will be shown and limit what kind of ads will
show up.

I also started on the process of favoriting quotes. We brainstormed new ideas on
how quotes should be interacted with and distributed and ended up coming up with
the system where quotes can be favorited or shared. With favoriting, the quote
gets taken out of Firebase and gets saved into the local database. The sharing
system will stay the same and eventually quotes that are neither shared nor
favorited will be automatically shared with another user and be taken out of
the quote list. So far, I was able to implement some UI stuff where a star
icon is displayed and the star gets colored in whether the quote is chosen
as a favorite or not. Now I just need to figure out how to integrate the
local database with the Good Vibes widget and make sure the quote gets
added and deleted from the remote database properly and is saved properly locally
so that favorited quotes do not disappear when the app closes.

This upcoming week will be a lot more busy with trying to figure out all of
this database stuff (I have minimal skills with SQLite) and making sure I do
not break anything. An issue came up with the Podfile not working when
implementing ads so the iOS version could not build properly which Andrew Eveld
eventually fixed (thanks man). I will do my best to not cause any more problems
and contribute to the app. We will also be meeting with Dr. Goadrich's TEC class
who are beta testers for our app in order to learn about what works best and
what needs to be fixed. Exciting!
