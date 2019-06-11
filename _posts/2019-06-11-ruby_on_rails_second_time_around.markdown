---
layout: post
title:      "Ruby on Rails...second time around."
date:       2019-06-11 20:18:51 +0000
permalink:  ruby_on_rails_second_time_around
---

I’m not sure what others experience, but reviewing a programming language I previously studied results in two realizations. 
The first is that I forgot the most basic syntax. I can’t say its like riding a bike, the initial peddling will lead to a definite wipe out. The rust eventually clears, but I need to put some time in to work out the kinks. The comical part is that a few months back I was flying through the code on autopilot, muscle memory would take over. In addition to know thing syntax like the back of my hand, debugging down the stack was second mature. Not sure whats being passed? Piece of cake, raise params.inspect does the trick. The second realization was that although the “how to” was rusty, the overall concepts made more sense. During the initial learning phase I was just trying to keep up and get things working. Reviewing the material for a second time had me thinking thoughts like “ahh, so THAT’s why you do XYX”.  The big picture became clearer. 

Initially, the syntax part bummed me out. So much so I actually googled it. Fortunately this is a pretty popular topic. Developers with lots of experience talked about this, saying that they forgot some pretty basic format, but nothing that a search, copy and paste couldn’t resolve. 
Anyway, I began my re-rails journey. Just for me this time. No agenda, nothing due, just going over the basics and to see how far I could get. 
I don’t get very far at all at first. The good part is that what took me hours to learn the first time was taking a fraction of that time now. I start with the very basics, but then I quickly move to generators. Generators. So much easier, so much easier. 

Now I start remembering things. Best part for me is that I know how to reverse something if its wrong. I know how to drop a DB table and start from scratch. Whole project is poorly thought out? Delete the folder.  If you are reading this you might be thinking ‘um, yeah, no kidding’, but for me it meant freedom, the ability to screw up and then re-learn something. 

Start with a simple user model:
rails g model user first_name last_name user_code

Ugh! You forgot, you wanted the user name to be an integer, not a string. Piece of cake. Delete!
rails d model user first_name last_name user_code

You realized you already created some users and their in the Database?
Rails DB:Drop

Freedom to make mistakes. Making mistakes allows you to re-learn. No pressure. 

Don’t get down on yourself for forgetting syntax. It seems pretty common, even for experienced developers. The important part is that you understand whats going on conceptually. Thats the part you don’t want to forget. That’s the part you can’t copy and paste (and then use effectively). 
