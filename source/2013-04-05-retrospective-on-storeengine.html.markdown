---
title: Retrospective on StoreEngine
date: 2013-04-05 14:06 -06:00
tags: store engine, rails, pairing
---

RAILS. Woot.

<a href="http://www.oregonsale.herokuapp.com">First project in the books.</a>

I learned a lot about model/controller/view during this project, and also a little about the power of the Rails framework. Certain terminal commands could help build out intricate relationships, forms and partials could help loop through patterns in your controller and views, and Rails could really make translating your Ruby to the web fun. 

The transition from straight Ruby to Sinatra to Rails has been an interesting one indeed. I find the bugs get more and more interesting: from "well, we got this bug because we didn't follow Jeff's tutorial right" to the much more complex "we just pushed and merged three features and are having S3 / postgres disasters." The coding also becomes much more interesting. The user experience of our app made up around 90% of our project's results. Who gives a shit what's going on under the surface (besides us?) If our site isn't shiny and easy to use, all that work is for naught. I stayed up fairly late the night before the project was due pumping out tests... that no one would ever see. In some ways, this will change the way I approach code and approach issues in general. As Ben Orenstein (@r00k) mentioned when we first started this project, you should be able to, every two days or so, stop the work you've done and ship your product as is. Start with the features that matter most first. That doesn't mean grappling with what database to use or how best to migrate your tables. That meant to start with the user.

This theme seemed to resound later when we discussed view testing. Using Selenium and Cabybara to test forms really helped guide some of our code. If I were a user, what info would be necessary to log in? And to create a trip?

Though "Don't Make Me Think" felt a little bit like hashing out basic principles of UX, it really helped in the design side of our code. I caught myself thinking aloud: "this looks like a button, but you can't click it", "these tabs don't mesh well against the background," "why is does our slider/navbar look different on this page?" I'd really taken a lot of the basic design principles for granted on the user end. Now I find myself concious of positioning, color, style, and so much more. Typography has turned from a novelty into straight-up helvetica.

As for my teammates, I couldn't have asked for a more complementary pairing. Josh and John were both very relaxed and paced, even when it came to crunch time. Both were fairly self-motivated as well, which melded our team nicely. Josh's personality was very sincere and innocuous (I mean that in as good a way possible) - he was non-confrontational, but at the same time an implicit leader on the team. John was able to go off on his own, build a feature, and transition seamlessly back into the group. He too had strong opinions and really guided the project's growth. Overall, I think our project, though slightly gimmicky, was a successful first foray into Rails. I look forward to getting started on the next project.

Here's to the Oregon Sale! (John not pictured)

<img src="/images/oregonsale.jpg">