---
title: Retrospective on Duckett's 'HTML and CSS' - Part 1
date: 2013-03-11 15:29 -06:00
tags: html, css, duckett
---

Though the opening 7 chapters of 'HTML and CSS' were fairly straightforward, I suppose the most challenging piece so far was on forms. Collecting information from visitors is vital to an interactive website, and there were plenty of form controls that I'd never seen or used before. Some of these controls include the type='password', select boxes, and where to use labels.

We are learning about input forms so that we might get or post data based on the user's choices. Forms use name / value pairs to know what information is sent and what kind of information it is (and where it's sent!). So:

````
<form action="/photo" method="post">
  <p>Upload a new picture:</p>
  <input type="file" name="song" /><br />
  <input type="submit" name="submit" value="Upload" />
</form>
````
<br />
Should produce:
<br />
<form action="/photo" method="post">
  <p>Upload a new picture:</p>
  <input type="file" name="song" /><br />
  <input type="submit" name="submit" value="Upload" />
</form>
<br />

The following code could be used in the Sinatra that we've learned so far. The song parameter can be gathered and saved in a sinatra server file like this (I think!):

````
post '/photo' do
  new_photo = params['song']
  new_photo.save
end
````
<br />
What gets a little hazier is the finer points of the HTML. For example, when might we use type="hidden"? According to the book, you use hidden when an author wants to "add values to forms that users cannot see... [for example,] to indicate the page the user was on when they submitted a form." This sort of information can be accessed through a product like Google Analytics, yes? So what else might you want to do with a hidden form?

There are a few additional HTML tags that I'd never really used. Fieldset and legend are among them, so I'll take a stab at a payment legend (complete with labels so that a user might click on the label to access the input):

````
<fieldset>
  <legend>Billing information</legend>
  <label>Credit Card:<br />
    <input type="text" maxlength=16 required="required" name="cc" />
  </label><br />
  <label>Expiration Date:<br />
    <input type="date" name="exp" />
  </label><br />
  <label>Three digit security code:<br />
    <input type="password" maxlength=3 name="code" />
  </label><br />
  <input type="submit" value="Submit for payment" />
</fieldset>
````
<br />

Should look like this:
<fieldset>
  <legend>Billing information</legend>
  <label>Credit Card:<br />
    <input type="text" maxlength=16 required="required" name="cc" />
  </label><br />
  <label>Expiration Date:<br />
    <input type="date" name="exp" />
  </label><br />
  <label>Three digit security code:<br />
    <input type="password" maxlength=3 name="code" />
  </label><br />
  <input type="submit" value="Submit for payment" />
</fieldset>
<br />
There are some nice points to this form, and some one's I wish I knew more about. I used a max length on CC and three digit security codes to make sure the user does not write too many characters. Plus, I kept the code hidden in case someone was looking over your shoulder. However, I still have some issues with form validation. I tried to make CC a required field, to no avail. I used several new HTML5 components, like the type="date". However, I couldn't figure out how to make the date only month and year (as an expiry date often is represented). Will do some research and post during my next blog!
