---
title: Feeding Boulders and Starting Up Engines
date: 2013-05-17 14:10 -06:00
tags: feed engine, boulder, startups
---

Well, it seems I haven't posted here in quite a while. Here are some updates and retrospectives.

Blair, Jorge and I have been working on Feed Engine, an app that consume the Github, Travis CI, and Pivotal Tracker APIs to create a project dashboard called HaxHub. I've really enjoyed working with these guys, and feel like we've made good progress so far. I've initially spent some good time working with the backend models and controller/model testing, and have recently moved into the CSS, jQuery/AJAX bits. The AJAX has been tricky, since I've never dealt with it on this scale before (I'd done a few cute tricks before, but haven't had to deal with continuous polling to the database for new dashboard items). While the latter part has been challenging, it's also incredibly rewarding to see the results. One problem I've been recently solving is how to display new Git Actions on the dashboard without refreshing the page. I'm getting so close, but keep finding new issue with our original code base. Here's one train of action:

* I'll use an ID > ? SQL call to collect all git actions with a higher id! That'll be ea-- oh wait. The IDs are in the opposite order that we need them in. Hm.
* I know! I'll just call a reverse on the initial array of actions, so they save to the DB in the opposite order! ... I can't make that call? But... but...
* Okay. I'll try using created_at instead! Wait... we don't overwrite the created_at on initial creation?
* I'll just overwrite it myself.

And it continues. Our project is due Thursday.

Plan for the next six days: Scale out the beginning AJAX code I have so it can handle multiple projects at once and multiple columns at once (for example, I want to follow rails/rails and blairand/alpha-feed-engine, and I want to have each one track travis and github, so want continuous updates on all 4 pieces of information). We need to set up background workers to handle hitting the API at a steady pace. We need to add Travis CI models. 

Oh, and probably put in on a production server.

Got our work cut out.

Brief aside: in other news, we went to a day of the Boulder Startup Week yesterday. Though it didn't quite clear up what I'd personally want to do after this program, it was informative to see real startups and dev shops in action. We had a lovely tour of the LivingSocial, GNIP, and QuickLeft offices. Learned quite a bit about the hiring process, what we should expect, and what we should really shoot for. It worried me a bit to hear that students of OTHER gSchooly programs had difficulty getting hired at legit companies, but also comforting to hear that most of the hiring questions and expectations had been thoroughly addressed by our teachings at school so far. For example, we were told we need to know the "where Rails ends and Ruby begins" -- and I think we certainly do.

More about the job-hunting business to come in next week's blog. Cheers.