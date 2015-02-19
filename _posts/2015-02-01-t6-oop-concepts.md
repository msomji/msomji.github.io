---
layout: blog-post
title: "A Scoop of Ruby Variables"
subtitle: "It's not at bad as it seems!"
date: 2015-02-01
---

When thinking of variables, one can consider them as objects in which you can hold information in while running a particular program. Depending on the program and your needs, you can set limitations to the variable (scope) that determines where it can be accessed from and whether it can be alters later on in the program or not.

There are only five different types of variables that are supported by ruby. There are Constant variables, Global variables, class variables, instance variables and local variables. I have listed these in that order intentionally with the variable with the largest scope at the start and the variable with the smallest scope at the end.

The constant variable is usually depicted by being defined in all caps as such:

INTEGER = 5
In this example, the integer 5 is a constant variable named integer. Having the largest scope, this variable can be accessed from any where in the program. The global variable is depicted by a “$” preceding the variable name as such:

$integer = 5
These two are very similar as both can be accessed from anywhere in the program however, the constant variable will not let you change its contents and will return a warning if you try to do so.

The class variable has the next largest scope. it is usually depicted by “@@“ preceding the variable name as such:

@@result = “true”
These variables must be initialized before they can be used in the method definitions. Class variables have a scope that expands through the entire class and therefore if the variable is ever changed in one method it results in a permanent change of the variable in ever future occurrence. The instance variables that is depicted with an “@“ before the variable name is very similar but only differs that when it is changed, the variable is only altered for that particular instance, once a new method is initiated, the variable returns to its original value.

Local variables that are not preceded by anything before the variable name, they either start with an “_” or a lowercase letter and have the smallest scope of all variables. it is only accessible within the method it is introduced in.

This is obviously a short introduction to the different ruby variables, but I hope it sheds light on what they are and how they can be used across and within different classes and their methods.