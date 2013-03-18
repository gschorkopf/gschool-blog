---
title: Retrospective and Work on Duckett's 'HTML and CSS' - Part 2
date: 2013-03-18 15:11 -06:00
tags: html, css, duckett
---

After delving into HTML and CSS and completing the first two thirds of the book, I've decided to play around a bit with navbars. Here are some simple instructions on how to create a user-friendly navbar with styled links and inline CSS.

First, we start with the basic HTML:

````
<ul>
  <li><a href="#">Home</a></li>
  <li><a href="#">About</a></li>
  <li><a href="#">News</a></li>
  <li><a href="#">Blog</a></li>
  <li><a href="#">Contact</a></li>
</ul>
````

<P>Nothing special here. The result should look something like this in your browser:<br />
<img src="/images/navbar1.png" ></P>

Let's add some CSS! We want to make the li inline, so let's start off by working with the 'display' property. I'll also add a bit of basic property info about padding so that our navbar pops off the top of the browser window, as well as a margin to the li so the links' boxes aren't right next to one another.

````
ul {
  text-align: center;
  padding: 25px;
}
li {
  display: inline;
  margin: 0px, 3px;
}
````

<p>Now we're gettin' fancy!<br />
  <img src="/images/navbar2.png"></p>

I want to play around with the color scheme. How about we change the font color, add hover properties, and change  the border of our navbar.

````
ul {
  width: 550px;
  padding: 20px;
  margin: 0px auto 0px auto;
  text-align: center;
  border-top: 5px solid #819FF7;
}
li {
  display: inline;
  margin: 0px 3px;
}
a {
  color: #642EFE;
  text-decoration: none;
  padding: 6px 18px 5px 18px;
  text-transform: uppercase;
  letter-spacing: 0.15em;
}
a:hover {
  color: black;
}
````
<br />
Looks a lil' something like this:<br />
<img src="/images/navbar3.png"><br />

This is where I'll leave it at today. I'd like to add a drop-down menu for, say, 'news' to highlight the different news items. More to come.