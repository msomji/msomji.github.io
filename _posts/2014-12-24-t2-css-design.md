---
layout: blog-post
title: "What are the Differences Between Relative, Absolute and Fixed Positioning?"
subtitle:
date: 2014-12-24
---

Web design and drawing have a lot in common. Both include creating shapes, manipulating said shapes and then ordering the shapes in patterns that create the end product. While drawing in the traditional manner, once drawn, shape remains in a fixed position until it is either covered by another shape or erased. On the other hand, web design tends to be a little more volatile as it allows the shape to move and interact with the user depending on their actions.

The creation and position of a shape in traditional drawing is fairly straightforward however communicating the same information in web design can become very confusing without the proper foundation. First thing is first, in web design you create the shape in an html document and then manipulate it or style it in a separate CSS document. Though there are a plethora of different styling properties that one can apply to any given object using CSS, we will mainly discuss the “position” property.

There are three commonly used characteristics for the position property (yes you guessed it): relative, absolute and fixed.

Fixed is the easiest to understand. A fixed element is positioned on the screen whose position is not affected even if the page is scrolled. This means that the element will always be visible to the user no matter where they are on the page.

The absolute property is fairly similar to the fixed property however this time the element is positioned on the page rather than the screen (key word: “page”) When setting an element to absolute, it is excluded from the normal flow of things and abides by any additional instructions you give it. i.e:

Div {

Position: absolute;

Top:0;

Right:0;

}

In the example above, the element will be positioned on the top right corner of the page. It is important to remember that unlike the fixed characteristic, when the page scrolled down, the absolute position disappears as it is positioned on the page rather than on the screen.

The relative characteristic accompanied by additional top, bottom, left and right information allows the element to move relative to where it would have been placed normally in the document. The relative position characteristic becomes a lot more interesting when it includes other elements within it. For example when an element(A) with an absolute position is placed within an element(B) with a relative position, "A" moves relative to "B" so this time if we applied the following code to "A":

A {

Position: absolute;

Top:0;

Right:0;

}

“A” would position it self in the top right corner of “B.” It’s a little confusing so read that last paragraph again, its pretty neat stuff!

There we have it! The differences are pretty significant but can become confusing if you over think it. Happy positioning!