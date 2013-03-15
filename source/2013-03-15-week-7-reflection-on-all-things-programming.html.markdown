---
title: Week 7 - Reflection on All Things Programming
date: 2013-03-15 09:10 -06:00
tags: gschool, sales engine
---

Various thoughts: I learned how to use inject correctly. Though a minor victory, it lead to a week of breakthroughs. After the inject success, I generally broke through on quite a few ennumerables. And then quite a few relationships in my Sales Engine. And then and overall epiphany on Ruby on Rails and the finder methods in ActiveRecord. And then a thoroughly stronger grasp on the program so far and my comfort level.

And that all started because code like this:

````
def scrabble_scorer
  sum = 0
  word.collect {|letter| score_hash[letter] }.each do |score|
    sum = sum + score
  end
  sum
end
````


Turned into this:

````
def scrabble_scorer
  word.inject(0) {|sum, letter| sum + score_hash[letter]}
end
````


What are the differences between the first and second segments of code? Well, the latter is half the size. The latter is easier to read and doesn't use nested loops. I started to write more and more terse and simple methods. One's that I could explain to someone easily. Concepts like "favorite_customer" that stretched across three methods of 14 lines each turned into one method that was one line. Instead of throwing code down on the editor and seeing what stuck, I moved into writing test-driven, consice code - and in smaller, simpler steps. I can't wait to get into some Rails. I'm sure that I'll shift back into uncomfortable excitement next week, but for now I'm feeling good, at least on a basic concepts at the Ruby level. Thanks, Eloquent Ruby.

I also got a little more comfortable with testing this week. Maybe it came from writing 135 passing tests. It definitely came from using RackTest. And I think above all else, it came from writing the tests first.

Testing had really felt like a chore until recently. Now it feels like THE process. Testing is just writing Ruby, after all. Why stress out about that? Instead of struggling for 4 pomodoro breaks looking for a missing end across 15 files, my test will just tell me where it's at.

Rails next week. More posts to come.