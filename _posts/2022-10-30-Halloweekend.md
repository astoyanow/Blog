---
layout: post
title:  "Halloweekend"
date:   2022-10-30 18:35:38 -0500
categories: jekyll update
---

The parser is finally finished, at least for now. There will still probably be bugs that will mess things up but right now, there are no bugs and it can parse a CSV file accurately. The only issue may be keys that overwrite each other in the parser and the fact that cells with dollar signs are not accounted for, which may affect the table if it required integers instead of text or string. However, all that matters is that it works and has been able to parse a file that Arkansas Asset Builders sent to test with.

All that is need to be done now is integrate it with the database and the front-end portion. Currently I am working on integrating with the database which may be more tedious. Working with SQLite is always a pain because of how barebones it is and how badly the documentation is for libraries that adopt SQLite. I keep getting errors for an incorrect path to the database but it does not show me which method that is being raised in and I think it is somewhere in the Maven SQLite library but it must be so big that I will not be able to find where it is messing up. It may have to deal with how the files are set up in my directory but I am not sure.