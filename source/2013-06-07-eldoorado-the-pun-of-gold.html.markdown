---
title: Eldoorado, The Pun of Gold
date: 2013-06-07 09:19 -06:00
tags: independent project, eldoorado
---

With Eldoorado now in the books, I found myself pretty happy with the results. Though I would have liked to combine more (or, erm, any) external APIs into my project, I thought that building a service oriented design was a good challenge, as well as building my first gem and use D3. I broke the services into the following pieces:

- An <a href="http://www.github.com/gschorkopf/eldoorado">API</a> for the door scan data in Galvanize
- A <a href="http://www.github.com/gschorkopf/eldoorado_gem">Ruby wrapper/Gem</a> for the API
- A <a href="http://www.github.com/gschorkopf/eldoorado_data">data converter</a> to transform a raw txt feed into gem objects
- And a <a href="http://www.github.com/gschorkopf/eldoorado_dashboard">front-end dashboard</a> build with D3js.

The final product is available here: <a href="http://eldoorado.herokuapp.com">Eldoorado</a>. Type in the keyword "yesterday" for an added bonus!

I came in late today, so I'll have to continue this blog later. Cheers.