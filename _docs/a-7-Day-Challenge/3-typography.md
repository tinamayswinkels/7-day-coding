---
title: Day 3 - Typography
category: 7 Day Challenge
order: 3
published: true
hidden-from-menu: false
permalink: day-3
---

Today we're going to take the HTML elements that we coded yesterday in codepen and style them\!&nbsp;<br><br>*This video is taken from our Website in a Weekend online course, so please ignore mentions to other lessons and just focus on the content in this one\!&nbsp;*

{% include youtube.html id="aqp9nmGOXH4" %}

Here's a link to the [codepen](https://codepen.io/instituteofcode/pen/dEooWO){: target="_blank"} finished example.

### Styling Text

The **color** property changes the color of text. Colors can be set using color names (`blue, green, yellow`), hex codes (`#FFF`), rgb values (`rgb(60,60,65)`) or rgba values which are like rgb values but also have an 'alpha' value which determines the transparency (`rgba(60,60,65,0.5)`).

Eg. This will set the color of all of the paragraphs to red.

~~~css
p { color: red; }
~~~

The **font-family** property sets the font of the text. By default there are around 15 fonts that are available by default in every browser, including 'Arial', 'Helvetica' and 'Georgia' and 'Courier New'. More often than not though, we will use a more attractive font that is hosted by google – aka a 'Google Font'. We'll learn how to add google font's during the retreat, but for now just have a [look at the google fonts](https://www.google.com/fonts) and see how many there are\!

If you are using a web-font, then you should specify a 'fall-back' font for it to use in case the web-font doesn't load. Options include Serif, Sans-Serif, and Script.

Eg. This will set the font of all h1 headings to Courier New.

~~~css
h1 { font-family: 'Courier New', sans-serif; }
~~~

The **font-weight** property sets the thickness of the font. Depending on your font, the options available may just be normal and bold, or you may have up to 8 variations (100, 200, 300, 400, 500, 600, 700, 800).

Eg. This sets all paragraphs to be bold.

~~~css
p { font-weight: bold;}
~~~

The **text-align** property sets the way that the text flows on the page, it can be left aligned, right aligned, center aligned or justified.

Eg. This will align the body (ie the whole page) to the center.

~~~css
body { text-align: center;}
~~~

The text-decoration property determines any 'decorations' on the text like underline. You will notice that links are underlined by default, so if you want to **remove the underline** you would need to set the text decoration to none.

Eg. This removes the underline from all links and instead makes them bold.

~~~css
a {
  text-decoration: none;
  font-weight: bold;
}
~~~

[LINK TO SLIDES](/Typography.pdf)