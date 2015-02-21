---
layout: blog-post
title: "Looping Through Ruby and JavaScript"
subtitle: "A closer look at some of the similarities and differences"
date: 2015-02-08
---

This week we were introduced to JavaScript, totally new territory for me personally. Surprisingly I wasn’t as intimidated as I had thought I would have been. Over all it turns out that Ruby and JavaScript both have a fair amount of overlap but there are still a few fundamental differences that need to be pointed out. In this blog I will be comparing how looping differs in Ruby compared to in JavaScript.

Ruby allows for two different ways to loop through an object. The first way is to use a "for", "while" or "in" loop and the other method is to use an iteration and a block that iterates through that particular object a certain amount of times. The "for in" loop is shown below:

<script src="https://gist.github.com/msomji/0c1f31e796dcb919cdd1.js"></script>


Below is an example as to how you can iterate through a loop in Ruby.

<script src="https://gist.github.com/msomji/8bd28d9f4c241210abfd.js"></script>

Hopefully so far, that was all review. Now when it comes to looping n JavaScript, it too does allow for a for/in loop but it does not work quite as well with arrays without the help of JQuery that we will cover in a later blog. Below I illustrate how to loop through an array using pure JavaScript

<script src="https://gist.github.com/msomji/d52126f3afa62f898aea.js"></script>

As we can see from the codes above, in JavaScript we have to define when the iteration should start and when it should end however when it comes to Ruby it is understood and the method understands that it only needs to iterate through the array as many times as the number of objects within the array. in addition to this JavaScript also makes us define a new variable (len) in oder for it to determine how many objects there are in the array that we need to iterate through where as none of that is needed in Ruby.

From these examples it may come across that Javascript asks for more information about what it needs to do where as Ruby just takes what it is given and does more work in the background making it easier to use however this the reasoning behind this is that JavaScript allows its users a lot more freedom compared to Ruby and the cost of this freedom is that it needs more specific information in its methods to make sure that it is doing exactly what the user needs.