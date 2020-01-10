---
title: Day 2 - Hello CSS
category: 7 Day Challenge
order: 3
---

Today we're going to take the HTML elements that we coded yesterday in codepen and style them\!&nbsp;

{% include youtube.html id="vKkds7j6i7Y" %}<br><br>*This video is taken from our Website in a Weekend online course, so please ignore mentions to other lessons.&nbsp;*

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

1. Create 6 html element (for example, h1 to h5 and then a paragraph)
2. Use the universal selector and CSS reset to reset your browser styles&nbsp;<br>&nbsp;

   ~~~css
   * {
     margin: 0;
     padding: 0;
   }
   ~~~
3. Give the body element some padding and a background color<br>&nbsp;

   ~~~
   body {
     padding: 5%;
     background-color: #FCF7DE;
   }
   ~~~
4. Let's use a multiple selector to select all the headings and paragraphs and give them the same padding and margin.<br>&nbsp;

   ~~~css
   h1, h2, h3, h4, h5, p {
     padding: 1rem;
     margin: 0.5rem;
   }
   ~~~

   &nbsp;

5. ~~~
   Now let's style each individual element one by one

   ~~~

![](/uploads/screen-shot-2020-01-11-at-8-56-43-am.png){: width="800" height="514"}

&nbsp;