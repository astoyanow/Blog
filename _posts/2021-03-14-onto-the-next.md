---
layout: post
title:  "Final Changes to HDX Assessment and onto Different Responsibilities"
date:   2022-03-14 18:35:38 -0500
categories: jekyll update
---

This week was a tough week with little progress. I had forgotten to update my development branch with the new updates that came in from the main development branch. This meant a lot of merge conflicts with the branch that I was working on for the addition and changes to the hamburger menu as well as the format style changes to the survey tables as well as the admin links. There were a lot of parts that I had to redo since the code from development changed so I could not include the changes directly. The merge comparator that Visual Studio utilizes was not very helpful as I could not edit individual lines in the windows that it provided for me, so I decided to accept all of the changes from the development branch. Thankfully, the CSS changes that I had made that were applied to all of the surveys did not have any conflicts so that was saved. 

At first when dealing with the merge issue, I had thought that there was a way to use RenderSection to include the format of the surveys into the _Layout page (since the surveys need to be in the navbar for users on phones) but that brought an issue that the surveys would no longer load into the sidebar so I had to go back to the old way and hard code the surveys into the navbar. After fixing that, I fixed the changes to the tables for the surveys by making the tables scrollable if there was an overflow so that the entire page would not move.