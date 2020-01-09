---
title: Contact Forms
category: Hello HTML
order: 5
---

To create a form we use the `<form>` element (pretty simple hey?). We’ll wrap all of the form fields inside of the form element.

### A Basic Form&nbsp;

The main element we use to collect text from users is the `<input>` element. This uses a **type** attribute to define what type of information is being captured within the control (the most common type is text), and a **name** & **id** attribute to uniquely identify it.&nbsp;` <input type="text" id="username" name="username">`{: .language-html}

Originally the only input types were text and password, but in HTML5 we have many more types to provide more semantic meaning: - color - email - range - time - date - month - search - url - datetime - number - tel - week

The name attribute describes the input field, and is what we will see attached to the&nbsp; users form submission when it arrives in our email.

&lt;SCREENSHOT OF FORMSPREE&gt;

These types can impact how different browsers might render the field, for example the date field on an iPhone will display a calendar scroller, while an email input will show the keyboard that has the @ and .com buttons on it and a tel input would show the number keyboard.&nbsp;

They can also optionally have a **placeholder** attribute which will display before the user has typed anything in the input fields.&nbsp;

```html
<form>
    <input type="text" name="full-name" id="full-name" placeholder="Your Full Name">
    <input type="email" name="email" id="email" placeholder="Your Email Address">
    <input type="submit" name="submit" value="Send">
</form>
```

This is what the above form would look like, without any additional css styling.&nbsp;

![](/uploads/versions/screen-shot-2017-11-16-at-5-11-59-pm---x----682-86x---.png)

## RADIO BUTTONS & CHECKBOXES

Radio buttons allow you to choose one from a small list of options. The browser will know they are all part of a single question because they share a name value. It is best practice to give each input a label and associate it with the field using the for attribute, where the value of the **for** attribute is the **id** of the field’s corresponding **id**. When the label text is clicked the radio or the checkbox will be selected.

```html
<input type="radio" name="day" id="friday" value="Friday" >
<label for="friday">Friday</label>

<input type="radio" name="day" id="saturday" value="Saturday">
<label for="saturday">Saturday</label>

<input type="radio" name="day" id="sunday" value="Sunday" checked>
<label for="sunday">Sunday</label>
```

Checkboxes are similar but they allow multiple to be selected. Adding the boolean ‘checked’ inside the tag sets that at the pre-chosen option (this is optional).

### Textarea

To capture longer blocks of text we use the textarea element, which doesn’t use a type attribute and has start and end tags that allow you to pre-fill text if you wanted to.

```html
<textarea name="comment" id="comment" placeholder="Send us a message!"></textarea>
```

## DROP-DOWN LISTS

To create a drop-down list we’ll use the `<select>` and `<option>` elements. The `<select>` element wraps all of the menu options, and each menu option is marked up using the `<option>` element.

```html
<select name="day" id="day">
<option value="Friday">Friday</option>
<option value="Saturday">Saturday</option>
<option value="Sunday" selected>Sunday</option>
</select>
```

If you add the boolean ‘selected’ to one of the options, this would function just like ‘checked’ for checkboxes and set a default value. Additionally, if you add the boolean ‘multiple’ to the select element, then you allow the user to select multiple options (although they would need to hold down shift to do so).

```html
<select name="day" multiple> ... </select>
```

## SUBMIT BUTTONS

At the end of your form you need some way to submit your information, you can do that with an input element with a type of submit. A submit button performs the action set on the form element. The value attribute is the text displayed on the button.

```html
<input type="submit" value="Send">
```

## Organising Form Elements

The way we organise and layout forms is critical in making them user friendly.

**Labels** create captions or headings for form controls. To link the label to the input field, we need to include a ‘for’ attribute that matches the "id" attribute of the input.

```html
<label for="username">User name</label>
<input type="text" name="username" id="username">
```

You can also wrap the label around the input to avoid having to use the for and id attributes, however this is not best practice. It is not semantic and it does not allow for separate styling of the label and the input. **Fieldsets** group sections of the form, just like a section or a div. By default they have a border outline but this can be modified in the CSS like all default styles.

```html
<fieldset>
  <label for="username"> Username </label>
  <input type="text" name="username" id="username">

  <label for="password"> Password </label>
  <input type="password" name="password" id="password">
</fieldset>
```

## LEGEND

The legend provides a caption or heading for the fieldset, and should go just after the opening fieldset tag.

```html
<fieldset>
<legend>Login</legend>
...
</fieldset>
```

See the Pen [Forms](http://codepen.io/instituteofcode/pen/oxEypP/) by The Institute of Code ([@instituteofcode](http://codepen.io/instituteofcode)) on [CodePen](http://codepen.io).
{: .codepen}

<script async="" src="//assets.codepen.io/assets/embed/ei.js"></script>

## OTHER FORM ATTRIBUTES

**disabled** - a boolean that prevents the user from interacting with the input placeholder - a hint or trick that disappears when you start to type

**required** - the form cannot be submitted while leaving this field blank or invalid (ie invalid email address)

### Making your forms work&nbsp;

Typically to make a form actually work you needed some backend programming and often a database, but there are a number of tools now to allow you to easily add forms to any site.&nbsp;

The most common attributes for the form element are action and method. The action attribute contains the URL to send the collected information to for the server to process. The method attribute is the HTTP method that browsers should use to submit data to the form. In this course, we won’t be digging in too deep into how information from a form is processed and handled on the back end of a website.

We’ll teach you three simple options for form submission that you can use on your site without ever needing to touch a backend, first using Formspree and secondly using CloudCannon or Netlify's built in form submission.

To use **Formspree**, just add these attributes to your form element…&nbsp;

```html
<form action="//formspree.io/your@email.com" method="post"> ...
</form>
```

To use CloudCannon's built in forms see their documentation [here&nbsp;](https://docs.cloudcannon.com/hosting/contact-forms/)

To use Netlify's built in forms see their documentation [here](https://www.netlify.com/docs/form-handling/)&nbsp;

<div class="cp_embed_wrapper"><iframe id="cp_embed_peZLvB" src="//codepen.io/instituteofcode/embed/peZLvB?height=265&amp;theme-id=light&amp;slug-hash=peZLvB&amp;default-tab=html%2Cresult&amp;user=instituteofcode&amp;embed-version=2&amp;pen-title=Simple%20Contact%20Forms%20V1" scrolling="no" allowtransparency="true" allowfullscreen="true" allowpaymentrequest="true" name="CodePen Embed" title="Simple Contact Forms V1" class="cp_embed_iframe " style="width: 100%; overflow: hidden;" height="265" frameborder="0"></iframe></div>

<script async="" src="https://production-assets.codepen.io/assets/embed/ei.js"></script>