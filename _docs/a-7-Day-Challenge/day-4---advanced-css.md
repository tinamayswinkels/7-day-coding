---
title:
category: 7 Day Challenge
order: 3
published: false
---

Today we're going learn how to create structural html elements, and style individual and groups of elements with classes.&nbsp;

{% include youtube.html id="RUEX9trmzUY" %}

### Activity 1

P.S. Try not to copy and paste but rather to type yourself, as the muscle memory &nbsp;helps you to learn

1\. In the html, create two h2, h3 and p elements

~~~html
<h2> My name is Tina </h2>
<h2> I'm the co-founder of IOC </h2>
<h3> I was born in Australia </h3>
<h3> I live in Bali </h3>
<p> I love sunset walks on the beach with my puppy Houdini </p>
<p> My favourite coffee is a soy latte </p>
~~~

2\. Write a default style for each

~~~css
h2 {
  ...
}
h3 {
 ...
}
p {
 ...
}
~~~

3\. Create a 3 classes with unique styles in your css. Experiment with adding these classes to various the html elements and watch as they override the default styles for each element (these are examples but feel free to use your own).

~~~css

.bg-featured {
  background-color: #ff7979;
}

.big-text {
  font-size: 2rem;
}

.underline {
  border-bottom: 2px solid;
}

.fancy-text {
  font-family: font-family: 'Dancing Script', cursive;
~~~

Here's a link to the [codepen](https://codepen.io/instituteofcode/pen/bJzKNo?editors=1100){: target="_blank"} finished example.