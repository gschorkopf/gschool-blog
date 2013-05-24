---
title: Hax So Hard and Independent Programming
date: 2013-05-24 14:52 -06:00
tags: haxhub, feed engine, independent project
---

Another gSchool project is in the books, and perhaps the most successful of the lot so far. I worked with Jorge and Blair on this one, and both were an absolute delight. We had a good mix of pairing and independent work, and we never exclusively owned a section of the code. I think our regiment - pushing branches to master and then reading over the code (never pushing directly to master) - was followed 99% of the time. Plus, we actually tested using VCR from the beginning. Our process felt very agile for whatever reason - we started with the essential bits (logging with GitHub, building out projects), and then built out iterations. It felt good being able to deliver a product in 2 day intervals, rather than chugging along and not having something ready for a customer until the day before (or sometimes the day of) the project's due date. It was great to stay in the know on all our code, which, ironically, was also the problem our group solved with HaxHub.

With <a href="haxhub.herokuapp.com">HaxHub</a> we learned about Travis CI, Pivotal Tracker, and especially GitHub and their respective APIs. Of course the final product was not perfect, but I think the codebase and final design represented what we'd hoped. I really enjoyed working with the frontend, and making stories/commits/tests visually appealing. It was my first foray into jQuery and AJAX, and those tools really helped dissolve the staticness of the app. 

<img src="/images/haxhub.png" />

The most challenging aspect of the project was dealing with APIs for the first time. Not everything about the gems we used was intuitive, plus allocating for background workers, knowing when to hit the API, and finding a way to comply with single responsibility was certainly a challenge. Chris Kelly spoke with us today regarding servicing APIs, and changed my perspective on delivering APIs. As he said, APIs should really be conveying the essential bits of OO programming too - sending messages and using verbs for methods and what not. 

Next week, we begin our independent project (our first since week two of gSchool). I have a few ideas, which I hope to flesh out over the weekend and in my upcoming 1-on-1 with Jeff. My first idea is to create a fantasy sports trade simulator and evaluator. You'd basically have two pages - the first gives you two forms, one for the players you'd like to trade away, and one for the players you'd be receiving in the trade. The progam would analyze each player's (or set of players') statistics, fantasy value, and upside, and then tell you whether it would be a good trade. Perhaps there would be bits about degree of confidence or age or upcoming schedule. I'd also like to explore data visualization with jQuery plugins.

There are a few APIs out there to use - ESPN seems to be the most prominent, and perhaps the Yahoo Fantasy APIs. I feel like my limitations will regard the algorithms I use for comparison - would it be excessive to come up with my own comparison metrics? Do the APIs provide actual fantasy value, or would I have to calculate that? Is this actually a good idea, that will show up my coding chops, or is it a silly, niche idea?

More thoughts on that soon.