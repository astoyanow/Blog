---
layout: post
title:  "Data, Data, Data"
date:   2022-10-09 18:35:38 -0500
categories: jekyll update
---

I have some experience with databases and connecting them to software as well as handling data input and output. For this reason, I have been doing some work on connecting our Firestore database for Good Vibes to the static web page that I developed last year so that people that visit the site can see different formatted data, such as the mood chart, which is kind of neat and fun to learn how to do. I am also working on a parser for CSV files so that files that come from Arkansas Asset Builders can be read into a database and formatted correctly.

It has been somewhat of a struggle trying to learn the documentation and implementation for Firebase onto a website. There are different ways to import packages from Firebase but the only way that worked for me was importing an API from another site and using the packages from there. There are also no hints as to what methods I can use and what properties some objects contain so it is a little difficult trying to figure out how to retrieve data with so little documentation. However, I have a connection set up that is able to retrieve a document from a collection from the Good Vibes database which is a success in my books. Now I can focus on retrieving specific data and creating a pie chart like the one from the app.

The CSV parser has also been giving me trouble. The issues are that each document is not the same, meaning the layout of the headers could be different and the titles of the files do not follow a certain format so I cannot use those to create different parsers, so the parser must have some level of abstraction. I am also trying to figure out how to separate the data into some data structure that can differentiate each row but also be able to be retrieved somehow. There are no ID numbers for the rows so I must come up with a way to create a map of some sort with a unique key that can be applied to each of the rows so that if a query were needed to be run, there would be no duplicate issues.