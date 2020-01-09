---
title: What goes in the head?
category: Hello HTML
order: 4
---

Everything in a html document is nested within either the &lt;head&gt;or the &lt;body&gt;. The &lt;head&gt; provides additional data to the browser that won’t be displayed on the main page, such as the document title &lt;title&gt; (which you’ll see on the title bar in the browser window), links to any external files (like your css or javascript), and any other beneficial metadata. The &lt;body&gt; element contains the actual content of the website; everything you see in the browser.

### General Meta Data

This defines the character set that the browser will use to decode the website (just add it to every site).&nbsp;

`<meta charset="utf-8">`{: .language-html}

This tells the browser that your website is responsive and works well on mobile phones and tablets. It's highly recommended.&nbsp;

```html
<!-- meta data to tell the browser that your device is responsive -->
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="robots" content="index, follow">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
```

### SEO & Social Meta tags

While there are lots of different strategies involved in ranking for SEO, providing appropriate meta data is certainly important. The title attribute is what will show in the tab at the top of the browser, and in the preview on google. The description shows up under the title, and the keywords give context of what the site is about.

![](/uploads/versions/screen-shot-2017-11-16-at-3-43-01-pm---x----800-260x---.png)

```html
<!-- Meta data for SEO purposes. -->
<title> The Institute of Code </title>
<meta name="description" content="With little to no previous technical experience, we'll teach you how to write HTML, CSS & Javascript code to build responsive websites from scratch and built a portfolio of live websites">
<meta name="keywords" content="coding, web development, html, css, bali, course">
```

**Open Graph tags** affect what will display when someone shares your website on social media (especially Facebook and Twitter). If you don't manually set this it will pull the first image from your website which is likely your logo or something similar.&nbsp;

```html
<!--  Social media sharing META Tags -->
<meta property="og:title" content="Institute of Code">
<meta property="og:description" content="With little to no previous technical experience, we'll teach you how to write HTML, CSS & Javascript code to build responsive websites from scratch and built a portfolio of responsive sites.">
<meta property="og:image" content="/images/terry-pool.jpg">
<meta property="og:url" content="www.instituteofcode.com">

<meta name="twitter:card" content="With little to no previous technical experience, we'll teach you how to write HTML, CSS & Javascript code to build responsive websites from scratch and built a portfolio of responsive sites.">
<meta name="og:site_name" content="The Institute of Code">
```

![](/uploads/versions/screen-shot-2017-11-16-at-4-11-34-pm---x----1891-2000x---.png)

If you are using **Social Analytics** to track links from social media to your website, you should add this meta data also.&nbsp;

```html
<!-- Social Media Analytics IDs -->
<meta property="fb:app_id" content="your_app_id" />
<meta name="twitter:site" content="@website-username">
```

### Connect your Stylesheets

Any css stylesheet that you want to use (including your own) must be linked in the head in order for it to apply. This includes things like Font Awesome Icons, Google Fonts, etc.

```html
<!-- External CSS Stylesheets always go first -->
<link href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Lato" rel="stylesheet">

<!--  Your CSS Stylesheets  -->
<link href="/css/main.css" rel="stylesheet">
```