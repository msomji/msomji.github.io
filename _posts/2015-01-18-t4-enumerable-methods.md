---
layout: blog-post
title: "A little introduction to Enumerables!"
subtitle:
date: 2015-01-18
---

There are obviously a list of different enumerables that we can discuss but for this particular post, we will stick to the “.map” enumerable.

Lets take an example: Imagine you have an array or numbers that you would like to multiply all the numbers within the array by 2. This is can be done using a very basic for loop as seen below:


            array = [1,2,3,4,5,6,7]

            for x in array
                puts x*2
            end

            => 2
            => 4
            => 6
            => 8
            => 10
            => 12
            => 14


But, the using an enumerable such as .map, it allows us to perform the same task with a lot less code.


            new_array = array.map {|x| x*2}
            new_array

             => [2, 4, 6, 8, 10, 12, 14]


The .map in the case above acts very similar to the .each method that am sure you have used in your previous exercises. The key difference is that with .map, it actually alters each element in the iteration and put it into the new array while .each leaves the original elements unchanged. In case you were wondering, you can use .map! to also just change the array as that you are iterating through.