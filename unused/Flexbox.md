---
title: Flexbox
category: Layouts and Positioning
order: 3
---

*All GIFs in this article courtesy of [Scott Domes](https://medium.freecodecamp.org/an-animated-guide-to-flexbox-d280cf6afc35).*

The Flexible Box Model (aka Flexbox) is a set of css properties that allow you to create flexible layouts and grids easier than ever before (it became widely available in the end of 2016). With Flexbox, things that used to be really hard, like vertical centering, same-height columns, reordering and changing direction is now a breeze.

Flexbox is based on having a set of item elements within a container element.&nbsp;

The main idea behind the flexbox is to give the container the ability to alter its items' width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space, or shrinks them to prevent overflow.

Let's look at an example together. Here we have a grey container div, and 4 divs inside. Even when we set the width of the colourful divs, they still take up the fill line, as block elements do.&nbsp;

### Property #1 - Display Flex

Then as soon as we set the display property of the parent container to flex, they line up next to each other.&nbsp;

![](/uploads/versions/flexbox-2---x----1432-618x---.gif)

```html
<section class="container">
    <div class="green"> 1 </div>
    <div class="yellow"> 2 </div>
    <div class="red"> 3 </div>
    <div class="blue"> 4 </div>
</section>
```

(Obviously there would be additional CSS to control the width and colors, but we assume you've got that by now!).

```css
.container {
    display: flex;
}
```

Pretty easy huh?&nbsp;

&nbsp;

### Property # 2 - Flex Direction&nbsp;

The next property is the flex-direction, previous to flexbox it was very difficult to dynamically arrange content on the page, and this becomes very handy later in responsive design. Don't worry too much about how you would use this, just know that it exists.&nbsp;

![](/uploads/versions/flexbox-1---x----1432-618x---.gif)

The default option is row, and the other options are row-reverse, column, and column-reverse. Again this is applied to the container element and impacts all of the child elements.&nbsp;

### Property #3: Justify Content

Justify-content controls how you align the items along the main axis (which could be vertical or horizontal depending on the flex-direction). There are 5 values available to justify-content:

1. Flex-start
2. Flex-end
3. Center
4. Space-between
5. Space-around

![](/uploads/versions/flexbox-3---x----1418-318x---.gif)

### Property #4&nbsp; - Align Items&nbsp;

Following along so far? Where justify-content controls the alignment along the main axis (typically horizontally) then align items controls the alignment along the cross axis (typically vertically).&nbsp; There are 5 align-items values;

1. Flex-start
2. Flex-end
3. Center
4. Stretch
5. Baseline

![](/uploads/versions/flexbox-4---x----1354-474x---.gif)

The first three are exactly the same as justify-content, so they are typically the easiest to understand. **Stretch** stretches the height of those items to fill their container (so long as their individual height it set to auto). Now for those of you just starting out this doesn't sound to exciting but for anyone who has been in the web development world for a while the ability to easily create equal height columns is a HUGE deal. While it's easy to set **width: 100%**, setting the **height: 100%** doesn't work, so flexbox introduces the first way to have dynamic (they grow and shrink as the container does) equal height columns.&nbsp;

### Property # 5 - Align Self

Align-self allows you to manually control the alignment of one particular child element.&nbsp;

![](/uploads/versions/flexbox-5---x----1350-424x---.gif)

### Try it out for yourself.&nbsp;

Test it out for yourself in codepen or see how you go with the [Flexbox froggy](http://flexboxfroggy.com/)&nbsp;or [Flexbox Defence](http://www.flexboxdefense.com/).

&nbsp;