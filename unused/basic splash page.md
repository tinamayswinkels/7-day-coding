---
title: Basic Spash Page
category: Activities
order: 3
---

### Part 1 - HTML

![](/uploads/versions/screen-shot-2017-11-17-at-5-31-02-pm---x----800-416x---.png)<br>In this exercise make sure you actually type out the code yourself, don't just copy and paste. Typing helps reinforce the memory of how to do it, and a lot of coding is muscle memory.&nbsp;

We're going to do this on CodePen first, then try copying it over to our desktop to use in Atom.&nbsp;

1) Create a new pen in CodePen. CodePen has the document setup built-in so whatever we type will go within the body tags of the html.&nbsp;

2) Let's start by creating a section to hold all of our content.&nbsp;

2) Add a h1 element within the section that says your name

5) Add a h2 element below this that has a ‘tagline’ about you

6) Add a short paragraph (p element) about yourself

```html
<section>
  <h1> Tina May </h1>
  <h2> Co Founder of Institute of Code </h2>
  <p> I’m a 27 year old entrepreneur with a passion for coding and travel (and   wine!). </p>
</section>
```

8) Add an image. Find an image through google images or your profile picture on Facebook. Right click on the image and ‘copy image url’. Add the image to your html document by adding the img tag, with a src (source) of the url.&nbsp;

If you don't have one, you can use `https://unsplash.it/300/300` which generates a stock image from unsplash. Generally image urls will end in .jpg or .png so if yours doesn't work, check that you have the url of the image not just the page where you found it.

```html
<img src="https://unsplash.it/300/300">
```

9) Let's add a couple of links for people to connect with you. Later we'll learn how to add icons, but for now we'll just use the words, let's add this between your h1 and h2.&nbsp;

```html
<nav>
  <a href="http://www.fb.com/tinamay"> Facebook </a>
  <a href="http://www.instagram.com/tinamay"> Insta </a>
  <a href="http://www.linkedin.com/tinamay"> LinkedIn </a>
</nav>
```

At this point it should look something like this, and your image will likely be way too big. That's ok we'll adjust that using CSS.&nbsp;![](/uploads/versions/screen-shot-2017-11-17-at-5-07-05-pm---x----800-262x---.png)

### Part 2 - CSS&nbsp;

Please complete the HTML exercise before attempting this exercise.

1) Let's get ourselves set up by adding the universal reset&nbsp;

```css
* {
  margin: 0;
  padding:0;
  box-sizing: border-box;
}
```

1) First let’s add style to the whole page (the body). Create a body selector and apply a background color and add some padding.

```css
body {
  background-color: #446CB3;
  padding: 1%;
}
```

2) Now let's style the section. We want to change the background color so that we can see it against the blue background, then we want to change the size. We could just px or % – we want it to adapt to the screen size but never get too big so we can use both. Then let's add some padding to give space inside the section.&nbsp;

```css
section {
  background-color: white;
  width: 50%;
  max-width: 700px;
  margin: auto;
  padding: 3%;
}
```

3) Our image is probably too big for it's container so let's fix that by giving it a max-width.&nbsp;

```css
img {
  width: 100%;
}
```

4) Our universal reset removed all the space between our typography, so let's add some of it back so that it doesn't look so squished. We could use pixels or Rems here, but it tends to look best when the space below an element is in proportion to it's font size which is exactly what rem's do.&nbsp;

```css
h1, h2, p, nav {
  margin-bottom: 0.5em;
}
```

5) Next up are our links, and there is quite a bit to do here. Links are naturally inline elements which are finniky to style, so whenever we want to style buttons, we change the display to inline-block.&nbsp;

Then let's add a border and give it rounded corners. Next we need to add some space, both inside of the border (padding) and outside of the border (margin). Then we just change the color, and remove the ugly default underline (text-decoration).&nbsp;

```css
a {
  display: inline-block;

  border: 1px solid #446CB3;
  border-radius: 3px;

  padding: 0.5rem;
  margin: 0.25rem;

  color: #446CB3;

  text-decoration: none;
}
```

6) Now let’s style the headings. I've used the same blue color as I did for the background for the h1s and then a dark grey for the h2s but you can style them however you like!&nbsp;

```css
h1 {
  font-size: 2rem;
  color: #446CB3;
}
h2 {
  color: rgb(60,60,60);
}
```

7) The only thing that's left is to change the fonts. Head over to google fonts and find a font that you like, I chose Montserrat. Copy the embed code, and add it in to the head (which you will find in CodePen by clicking settings) then add it to the body selector.&nbsp;

```css
body {
  background-color: #446CB3;
  padding: 1%;
  font-family: 'Montserrat';
}
```

That's it! Well done. Try to play around with some different styles and just experiment. If you get stuck, save your CodePen and reach out to us through the private facebook group and we'll help you out!&nbsp;

<div class="cp_embed_wrapper"><iframe id="cp_embed_OOOOjR" src="//codepen.io/instituteofcode/embed/OOOOjR?height=265&amp;theme-id=light&amp;slug-hash=OOOOjR&amp;default-tab=html%2Cresult&amp;user=instituteofcode&amp;embed-version=2&amp;pen-title=Portfolio%20-%201" scrolling="no" frameborder="0" height="265" allowtransparency="true" allowfullscreen="true" name="CodePen Embed" title="Portfolio - 1" class="cp_embed_iframe " style="width: 100%; overflow: hidden;"></iframe></div>

<script async="" src="https://production-assets.codepen.io/assets/embed/ei.js"></script>

## Troubleshooting:

* check that you have your syntax right with an open selector `{` and a close selector `}`
* check that you haven’t confused a colon `:` with a semi-colon `;` and aren’t missing any quotes `"`
* check your spelling (color not colour)
* if none of the styles are applying check the link to your css is in your html document and written correctly
* look for unusual colors or error messages in Atom.<!--base32-4cg50wk1cdu6jrv5411pgrbcdhjpwtv5ec-base32--><!--base32-8ngp6u10dxk20x38cmg6cvvcdhqqeubecwg76u31e9jq683md1jj0wv1dnjj0j2m9n62r832enu20t39ctk6awk5dtu20gukacq20mv5cmg6jth0f5qqa833c5q20wk5cdt6arbmcmg78u35dmq0-base32--><!--base32-45dnua3ge9gp6x39cdjjuctee1q6ea8-base32--><!--base32-4chj682md5r76eg-base32--><!--base32-58g58vt0cdt6arbmcmg66ubjcduprrbj41mpurb7cntjr83gdhgqj83qd5u6g83md1jj0rkfe9j6awhde9gp8ubnec-base32--><!--base32-58g58vt0c5r70v3t41u6gt90edgput90edu7jv3541u6y835etjq4ybmd1mpwtt0dxq20x38cmg70rb7cmg7jvvn41hp2vh0entpa83md1jj0r32dxj7j83vfng20wv5dhjp6x3fe8g2gu39dtu2uv39ddjj0x38cmg78tbregpp2v39cxq2j-base32--><!--base32-45dnua3ge9gp6x39cdjjuchee1q6ea8-base32--><!--base32-4chj682md5r76eg-base32--><!--base32-58g5jvvn41hp2vh0cdqpwx3jdxp20ubechmqcub4engpr832dxt68tbjecg7eubmd0g78u3541r74vvgcnt78ub5ecg60rkfe9j6awhddhjpcx305gg60rkfe9j6awhde9mpeu3mc0g6ax335r-base32--><!--base32-58g5jvvn41hp2vh0entpa83md1jj0r3mcnw78bbme9gpwwv6dxt6ur10e1t6yw35e9u7j83mdwg6urbbcmg78u3541u6ay3m41uq0w35e9hp2wv541vpjx38dxuq8833d1gpwtv9dtkj0x38cmg6gx3ddgq0-base32--><!--base32-58g42uk4entq883md1jj0t35ctgqav3m41vpaub7d1u20vv641u6gt90d1jp2t39dtkq683qd5u6g83md1jj0r36dxq78bbqcnmpeu3mc0g70wkfe1jq4x3t5r-base32--><!--base32-45dnua3ge9gp6x39cdjjuc9ee1q6ea8-base32--><!--base32-4chj682md5r76eg-base32--><!--base32-58g44rb3ddkq4vvndtj20jbdc5kpa82na9620r38ehu70wtu5wqpjvb1cxjq6bkndttq0v31edm2wrvfdmqq0u3fehqjuc9m6mt34c9n64wkjctp60pp6c9pc9gk6dtg60upct9zcdt6yw1xcnq78wkfe1wjct3ge8yk49k6d5u3urvjdxr2ctkd7nn70tt6d0ykec1g4tmqgukkeryk4bhh5rr2cubrdhmp4fbjc8pk0bhk5rujcw9x6mr2cxtx64tk0c30-base32--><!--base32-58g64vvjchjq4wt0cdqput90d5q20t39ctk6awk5dtu20wvmf5p6awt0d5q66v3nchmpwtt0edqprub45gg68rbkd1jp8b10cnu66bg-base32--><!--base32-4chj6816dth76w1v-base32--><!--base32-4chj682ddxv6jvk741mq883mdwg42x3fdmk6wrkke0xg-base32--><!--base32-64mj0gvjcngq8t90c4g6wtbq41k6yv34cnt20vve41wpyxbj41j6awvbehqq0818dxt20rbef5vpgtbjcmmj0rbecgg78ubmdhjj0ubm4undefinedc4uy90axjp4wv9ehjundefinedj-base32--><!--base32-68mj0kvgcnq20gbmdxpj0rbecgg76tbccnhq8826d5p6a816cxu3p82fe1jpw826dxp68tbj40k6ex1v416qj82qcnh76ubmcmg2w823e9jp2x3541gj0vk5ewg6cubccmg64y90e9mpeu3m5nhprub3ddmpwtt0d5q20x38cmg6rtb6egg6grbecgg76ub4cnh62wh0c5q6883kcnp6arvmd5q6e83kcnp6arvmd5q6e83ecnvj0tk9dhjjw82ec5ppa839egg6jvk4cnw2wu3mdnp0-base32--><!--base32-6cmj0m3cc5hpa83md1jj0tkfdhp6yxv9dtkj0x35f1u20ube41wpyxbj41m78vbc41k6jv35-base32--><!--base32-c1g60u3mdnp0-base32--><!--base32-7ggm8ku3ahcn0h90d1u6uv1y-base32--><!--base32-7hm78vbc7r-base32--><!--base32-7hm6arb47r-base32--><!--base32-7hu6jx3ccmz20n39ehp6a83fcrg7jvvne8g7etb2edmq8t907gqq8ubmdhjkw-base32--><!--base32-7gqpgtb1cgz0-base32--><!--base32-7hh6yt3t7r-base32--><!--base32-5rq2w-base32--><!--base32-7gqp4vv4f4z0-base32--><!--base32-7gqpgx3ddgz0-base32--><!--base32-c1g60-base32--><!--base32-6wmj0hvf41u6y83tdxuq4836dxp68tbj41gpwt10ctmpwt10f5qqa839dtj6ay1ed1u6uv1e41t6jtv8egg66v39cdnj0vve41mq8831dtj20wv5dhjp6x10c1qq0tbe41vpjx3840z20hvfdxkprt90cdm74vvdcng2w-base32--><!--base32-6gmj0kk5f1u20xv541q6atb441u6y833dxq6wtb3egg78u3541458kac41k6jv3541u6y83tdxuq483ecnvj0gukacg6cubccmq20jbe41u6gt90d1jp2t10edjp6x39dxq20vv641u6gt90d1u6uv10ctmprt9c41gp8t10c4g6rubedcg78u31egg66vvedtjp6x3k41u6gt90ehvpy836d5p6awte-base32--><!--base32-c1g60u3mdnp0-base32--><!--base32-7hm6arb47r-base32--><!--base32-7hp6jvkb41t6av1x3htq8ybccntpgtb5eundefinedej0x3te1jkundefined73mcnw78bv3edtundefinedu838e9jpcfundefinedwedu7jv355thq6wundefinedx7r-base32--><!--base32-7gqpgtb1cgz0-base32--><!--base32-c1g60-base32-->