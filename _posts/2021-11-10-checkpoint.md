---
layout: post
title:  "Checkpoint"
date:   2021-11-10 18:35:38 -0500
categories: jekyll update
---

I was finally able to figure out the process of favoriting quotes. After around
4 weeks of re-learning SQL, understanding the connection to Firebase, and many
hours trying to understand how the application worked, I was able to connect the
local database and the Firebase database through favoriting. The process was
much more convoluted than what I had originally imagined it to be but it was an
adventure nonetheless. Figuring out the whole process of trying to create a new
system of how users interacted with quotes was tough. The new system was that
users were forced to make a decision when opening and reading a quote: share the
quote with a random user, keep the quote by favoriting it, or remove the quote
from the list of quotes. Though it seemed simple in retrospect, it was much more
difficult.

For favoriting quotes, at first I had thought that removing the document sent to
the user containing the data for the quote and saving the data locally would take
the document out of circulation so that no one would be able to get the quote.
However, taking the document out of circulation does nothing but make it harder,
maybe even impossible, for the user to share the quote. Removing the document also
removes the documents ID. If a user were to try and share a favorited quote, a
new document would have to had been made and the data from the favorited quote be
put into that document. However, the app would then have to find the most recent
document created in Firebase that had the users userID in Firebase (since there is
no way of finding a certain named document since the document names are randomized
by Firebase) and, not being sure that it is even the correct document, set the data
inside of it. It was much more simpler to not have to do anything with the document
since removing it when favoriting the quote is meaningless.

Removing the quote was also a challenge since there was a combination of quotes from
Firebase and local quotes, both of which were accessed differently. Quotes linked
to Firebase had to have their documents deleted since removing the quotes from the
list did not work. Even if Firebase quotes are removed from the list directly, since
the document still exists in Firebase, it gets put back from the snapshot of the
Firebase instance listener.

The finished version was a lot more simple. Favoriting merely saves the quote
data locally and makes the quote mostly a UI change. There may be more implementation
in the future, such as sharing the quote when favoriting while also keeping the
quote stored locally, but that is for later work. Removing simply removes the
document from Firebase so that it is no longer assigned to the user.

This upcoming week is the consolidation of everyone's work, with Andrew's work
on streaks and Thank You counters and Vi's work on a dark mode theme (very
exciting!). I will be pushing ad implementation foreal this time and the favoriting
of good vibes. I will just have to make sure the ad implementation does not get
Disco Studio's Apple account suspended!!!
