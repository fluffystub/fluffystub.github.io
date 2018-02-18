---
layout: post
title: "Vertical centering in css"
date: 2018-02-06
---

Vertical centering in CSS
=========================

Vertical centering in css was one challenge that required using of "hacky" css up until flexbox was introduced. This article covers methods that can be used to achieve vertical centering.  

1. Table cell
-------------

Verical centering in css2 was mostly achieved using this technique. This involves making the display property of the parent as table cell. 

Let us make two divs, one larger outer div and a smaller inner div as shown.

![html](/images/180206vcic_html.png)

This html element node is used for all the examples in this articles.

Making a divs display property as table cell allows its internal elements be aligned as we want. This is achieved using the vertical-align and the text-align properties. 

![table-cell](/images/180206vcic_tablecell.png)

The text align property requirres that the element is an inline element. The inner div in the example has its display property set to be inline-block as i wanted to set its width as well. 

[Preview](https://codepen.io/RakshithNM/full/YWaXRq)

2. Position: absolute;
----------------------

Relative postioning an element creates a new context for absolute positioning within it. The inner element can be center aligned by postioning it absolutely and then using the top and left properties with the value of 50%. 

![postion](/images/180206vcic_positon.png)

When an element is moved in css, the reference point is the top corner of the element. So when an element is made to be positioned 50% to the top and left the element is offset by half its width and height. You can check this by removing the trasform property from the inner div.

References
----------

A. [display property](https://developer.mozilla.org/en-US/docs/Web/CSS/display)  
B. [display: table-values](https://css-tricks.com/almanac/properties/d/display/#display-table)
C. [position]()
D. [transform: translate(x,y);]()
