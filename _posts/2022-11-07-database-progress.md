---
layout: post
title:  "Database Progress"
date:   2022-11-07 18:35:38 -0500
categories: jekyll update
---

I have finally gotten database insertion to work. I can successfully insert a client into the client table based on information parsed from the FileParser. All I need to do now is to utilize it in the user interface so that whenever a user uploads a file it can insert into the database. The only issue that I am running into right now is the testing of the insertions into the database.

The problem is the way that the database is set up in conjunction with the functions of the database. The database connects to a named database that all of the functions use. These functions are also present in the function that I made to insert into the database. The issue is testing the function so that it does not insert into the actual database and instead, inserts into the test database. I am not sure how to tackle the issue. Perhaps I could create an entire separate class with identical functions but for the sole purpose of testing.