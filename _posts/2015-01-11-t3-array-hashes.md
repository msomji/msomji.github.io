---
layout: blog-post
title: "Comparing Hashes to Arrays"
subtitle:
date: 2015-01-11
---

Arrays and Hashes have a lot of things in common but they also have a few fundamental differences that make both of them useful in their own manner. In short, arrays contain order lists that can be accessed using numberical values ranging from 0(first object) to -1 (last object in the array). Hashes on the other hand contain pairs of entries known as keys and values where one can access a value of a certain object by calling its unique key. It sounds confusing but the following examples will show you how truly easy it is to understand how each work.

Consider a shopping list, that contains a total of four items : milk, eggs, bread and oranges. An array names shopping_list would store these values as strings within it and would assign a number them according to the order they were entered into the array starting with 0.


        shopping_list = ["milk", "eggs", "bread", "oranges"]

        => ["milk", "eggs", "bread", "oranges"]


The assigned numbers allow you to call the different objects in the array as such:


        shopping_list[0]
        => "milk"
        shopping_list[1]
        => "eggs"
        shopping_list[2]
        => "bread"


There are two things to note about the picture above, notice that shopping_list has a total of 4 objects within it however since the positioning starts from 0, when we call the fourth position in the array it returns nill. This is because there is no fourth object currently in the array. In addition to this, we see that when we call the object in the “-1” position, it returns the last object in the array. This is because an array assigns objects within it two numbers, if you read the array from left to right the assigned numbers begin starting from 0 however when reading from right to left the assigned numbers start from -1.

Hashes allow us to give objects a specific value, if we use the same shopping list, however instead of just stating what we need to purchase a hash can allow us to state how many of each we need to purchase.


      shopping_list = {
        "milk" => 2,
        "eggs" => 4,
        "bread" => 1,
        "oranges" => 10,
      }
      => {"milk"=>2, "eggs"=>4, "bread"=>1, "oranges"=>10}


The objects on the left are knows as keys and the objects on the right are known as values. It is important to remember that keys have to be unique but values can be repeated. In the example below we see how different values are called using their keys and we also see that when you try to call the key using its value, the hash returns “nill”. The nill tells us two things: It tells us that there is no key that has the value you called (in this case 2) and it also tells us that the only way to call anything in a hash is using the key and not the value.


        shopping_list["milk"]
        => 2

        shopping_list[2]
        => nil


As we can see, with arrays the order in which the object was entered into the array matters however in terms of hashes, the order doesn’t matter as we can call any unique key at any time and it would return its value.

There we have it! As I said before, the differences are small but fundamental.