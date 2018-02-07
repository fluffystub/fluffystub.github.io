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

References
----------

A. [display property](https://developer.mozilla.org/en-US/docs/Web/CSS/display)  
B. [display: table-values](https://css-tricks.com/almanac/properties/d/display/#display-table)
