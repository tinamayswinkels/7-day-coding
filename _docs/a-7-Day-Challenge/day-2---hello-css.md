---
title: Day 2 - Hello CSS
category: 7 Day Challenge
order: 3
published: true
permalink: /day-2-css
---

Today we're going to take the HTML elements that we coded yesterday in codepen and style them\!&nbsp;<br><br>*This video is taken from our Website in a Weekend online course, so please ignore mentions to other lessons and just focus on the content in this one\!&nbsp;*

{% include youtube.html id="vKkds7j6i7Y" %}

As elements are added to a web page, they may be styled using CSS. A selector designates exactly which element or elements within our HTML to target and apply styles to (such as color, size, and position). The most basic form of selectors target the type of element, such as&nbsp;`<h1>`or&nbsp;`<p>`.

CSS is made up of selectors, properties and values.

~~~css
selector { property: value; }
~~~

Within CSS, selectors are followed with curly brackets, \{ \}, which encompass the styles to be applied to the selected element. Below is an example of a p selector that would apply the styles listed within the curly brackets to all paragraphs on the page.

~~~css
p {...}
~~~

Once an element is selected, a property determines the styles that will be applied to that element. Property names fall after a selector, within the curly brackets, \{ \}, and immediately preceding a colon, :. There are numerous properties we can use, such as background, color, font-size, height, and width.

Here we are selecting all&nbsp;`<p>`&nbsp;elements and setting the value of the (font) color property to be blue and the value of the font-size property to be 16 pixels (px).

~~~css
p {
  color: blue;
  font-size: 16px;
}
~~~

Each property has particular units of values that it will accept. For example, the value or a color property can be a common color name (like red, blue or green) or a hex code (\#FEFEFE) or an rgb value ( rgb(60,60,60) ).

It is a common practice to indent property and value pairs within the curly brackets. As with HTML, these indentations help keep our code organized and legible.

## CSS Cheat Sheet

| Examples | Notes |
| `background-color: red; `<br><br>`background-color: #FCF7DE; `<br><br>`background-color: rgb(60,60,65); ` | You can use simple color names, hex codes or rgb values&nbsp; |
| `color: #FF9AA2;` | As with background colors, you can use names, hex codes or rgb values.&nbsp; |
| `padding: 2.5rem;`<br><br>`padding: 5%;`<br><br>`margin: 10px;`<br><br>`margin-bottom: 1rem;` | Padding and margin can be specified in lots of different units, most commonly pixels, rems, and %.&nbsp;<br><br>You can apply them on all sides by just using the padding or margin property or target specific sides with the properties like 'padding-left' or 'margin-bottom'&nbsp; |
| `font-size: 16px;`<br><br>`font-size: 2rem;` | Font sizes are commonly set it rems or pixels.&nbsp; |
| `text-align: left;`<br><br>`text-align: center;`<br><br>`text-align: right;` | Text alignment can be applied to individual elements or the whole page (the body) |

### Universal Selector & CSS Reset

This selector selects everything on the page, and we use it to override the default browser styles.&nbsp;

~~~css
* {
  padding: 0;
  margin: 0;
}
~~~

### Multiple Selector&nbsp;

This is an advanced selector that wasn't covered in the video but might be helpful for this activity. You can use the multiple selector by putting a comma in between each element name and it will then select multiple elements and style them all together.&nbsp;

~~~css
h1, h2, h3 {
  color: red;
}
~~~

This for example would select all the h1, h2 and h3 elements and make them red.&nbsp;

&nbsp;

## Activity Styling with CSS

This is what we'll be creating. If you get stuck, you can have a look at [my codepen here](https://codepen.io/instituteofcode/pen/gJOdgL?editors=1100){: target="_blank"}.&nbsp;

![](/uploads/screen-shot-2020-01-11-at-8-56-43-am.png){: width="800" height="514"}

1. Create 6 html element (for example, h1 to h5 and then a paragraph)
2. Use the universal selector and CSS reset to reset your browser styles&nbsp;<br>&nbsp;

   ~~~css
   * {
     margin: 0;
     padding: 0;
   }
   ~~~
3. Give the body element some padding and a background color

   ~~~
   body {
     padding: 5%;
     background-color: #FCF7DE;
   }
   ~~~
4. Let's use a multiple selector to select all the headings and paragraphs and give them the same padding and margin.

   ~~~css
   h1, h2, h3, h4, h5, p {
     padding: 1rem;
     margin: 0.5rem;
   }
   ~~~
5. Now let's style each element one by one

   ~~~
   h1 {
     color: #ff6874;
     background-color: #FF9AA2;
     font-size: 2.5rem;
   }

   h2 {
     color: #ff877f;
     background-color:#FFB7B2;
     font-size: 2.2rem;
   }
   ~~~

> **Hint: Colors**
>
>
> You are welcome to use your own colors for this challenge but if you want it to look the same as the example the color codes are:<br><br>H1 &nbsp; \#ff6874 & &nbsp;\#FF9AA2
>
>
> H2 \#ff877f &nbsp;& \#FFB7B2
>
>
> H3 \#ffbc8e & \#FFDAC1
>
>
> H4 &nbsp; \#c1df90 & \#edf6df&nbsp;
>
>
> H5 &nbsp; \#79d9b7 &nbsp;& \#c9f0e2
>
>
> P \#8f9dd5 &nbsp;& \#C7CEEA

[Printable CSS Cheat Sheet - Download here&nbsp;](/CSS Cheat Sheet.png){: target="_blank"}