---
title: Knackeries and Such
date: 2013-04-26 09:10 -06:00
tags: daughter of store engine, son of store engine
---

gSchool has been in store engine mode for 5 weeks now. I started by building Oregon Sale, a simple store platform. Next, we moved onto the multi-tenant Pink SoSE, which had the ability to add additional stores but was an otherwise failure from both an approach (waterfall over agile, code-first over test-first) and a design/UI stance (pretty bland, no focus on performance)

Now into our third consequetive Store-based platform (and why not?) we are working on the Daughter of Store Engine. Our project has been tentatively titled "Jeffsy" a simple portmanteau of our fearless leader and the knick-knack store Etsy (I was pulling for the title to be "Knackery", but apparently that could be misconstrued as either a place to hang butchered animals or a place for Irish hicks to congregate).

I've enjoyed working with our codebase, which was based on last week's Robofy. The code was already fairly well refactored and easy to understand. The biggest downside was the legacy CSS and HTML. Improper tags were used occasionally, but the bigger issue was discrepencies between when to use what bootstrap for scaffolding. As it often is with design, the actual site looks alright, but the code isn't very malleable. Chelsea and I decided to rip out the existing index page and start over to build the scaffolds/wireframes, and the result is already looking a bit tidier. I really hope we get to foray into some clean-looking JQuery, though admittedly I'm only halfway through our required reading (due Monday, yeeks).

Raphael and I had some struggles yesterday with Paperclip, and trying to implement multi-image products. We struggled with how to create the relationship between image and product, as well as how to tackle nested forms. 

As far as Rails goes, I feel like I have a better handle on the codebase and the helpers. Clearly, I'm still capable of running into 3 and 4 pomodoro break slumps (as with Paperclip yesterdya). I've developed a good sense of security after working with it in my previous two projects (and after the public torment of having our first codebase ripped apart by Hacker Monday at gSchool). Obviously, I'm still fairly reliant on gems for authentication, but have experience with authorization both with and without helper gems. 

I still don't think my toolkit is very big. I have a phew big tools, call em sledgehammers, that I can wield, but those hammers aren't the right tools to twist in a screw. I'm pretty excited to move into APIs and libraries. Our next project, FeedEngine, will teach us to use several at once. Our individual midway project will also be an exciting endeavor; though, admittedly, I don't have any super solid ideas.

More recap on the world of online Stores next Friday. 