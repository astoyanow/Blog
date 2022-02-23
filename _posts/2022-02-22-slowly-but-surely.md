---
layout: post
title:  "Back to Good Vibes"
date:   2022-02-22 18:35:38 -0500
categories: jekyll update
---

This week I was hellbent on getting the hamburger menu to work for Hendrix Assessment. Previously, I was working on redoing the sharing process on Good Vibes and I had done the process before, I just needed to find the push in GitHub where I had made those changes. With a couple of fixes, I had the new sharing system in place and merged into the main branch in no time. With that success came the success of the hamburger menu finally. I had to hard code some things in since they did not want to work otherwise (HTML with C# is kinda weird and I am still working on learning things but I am still learning regardless). There are still some design issues that I would like to work on but the main thing is that the hamburger menu is functional and everything works properly.

After working on the hamburger menu, I realized that the navbar and elements of the surveys in the Hendrix Assessment site are formatted quite poorly. The navbar does not extend to the edge of the screen when the screen is collapsed and the rows in the surveys get cut off with smaller screens. In order for users to be able to use the Hendrix Assessment site efficiently on all platforms, I will have to improve the formatting so that important parts that require user input won't be cut off or missing. Right now I am going to try and use Bootstrap to insert things into fluid containers but I will try to find a cleaner solution that does not require new elements, only changing of existing elements in the HTML and CSS files.