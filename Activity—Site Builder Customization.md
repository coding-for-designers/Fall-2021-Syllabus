# Customizing CSS
Here's how to modify the templates on site builders like Cargo or Squarespace. It's a bit trickier than editing your own site due to all the stylesheets already on the page. To try to make sense of the madness, these will be our tools:

- [Inspector](https://github.com/coding-for-designers/ICD-Course-Reader/blob/main/Tutorials/Web%20Inspector.md)
- Knowledge of [Specificity](https://github.com/coding-for-designers/ICD-Course-Reader/blob/main/Tutorials/Order%20Matters%20-%20The%20Cascade.md)

## Cargo
Create a free test site on [Cargo](https://cargo.site). Cargo offers you a way to edit all your site's CSS by clicking `Design > CSS Editor`

Here's the Design tab

![](attachments/Screen%20Shot%202021-10-04%20at%209.51.21%20PM.png)

At the bottom you'll see an option for CSS Editor

![](attachments/Screen%20Shot%202021-10-04%20at%209.51.25%20PM.png)

Now you'll see the full template stylesheet that loads on every page on your site.

![](attachments/Screen%20Shot%202021-10-04%20at%209.51.30%20PM.png)

Editing styles here should be self explanatory, when they're already defined. Use your Inspector to figure it out.

I've picked a tricky example here by choosing a link that does not have an element definition in the stylesheet already:

![](attachments/Screen%20Shot%202021-10-04%20at%209.54.39%20PM.png)

I'm using the Safari inspector here, and when I hover over some styles in the Inspector, I can see that the only predefined rule select all `bodycopy a` links, which is not what I want to do.

![](attachments/Screen%20Shot%202021-10-04%20at%209.55.33%20PM.png)

Since I want to select only the link in the top left corner, I keep hovering on the styles until I find one that gives me what I want to edit.

![](attachments/Screen%20Shot%202021-10-04%20at%209.54.28%20PM.png)

Cargo uses [data attributes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes) for specific elements, which means they're ultra-specific, kind of like an ID if you think about [specificity](https://github.com/coding-for-designers/ICD-Course-Reader/blob/main/Tutorials/Order%20Matters%20-%20The%20Cascade.md).

You can use data attributes to select elements [based on custom HTML attributes](https://css-tricks.com/a-complete-guide-to-data-attributes/). For example, Cargo has added the following to the HTML on the page:

`<div local-style="7485711">`

This is not a standard attribute in HTML, instead it's something that Cargo has decided to use in order to target this element with CSS and Javascript.

Back to the Inspector, if we select this element, it's already formatted to target the exact link that I want to target:

![](attachments/Screen%20Shot%202021-10-04%20at%209.54.46%20PM.png)

Copy and paste this into the CSS Editor and be sure to add the proper curly bracket formatting:

![](attachments/Screen%20Shot%202021-10-04%20at%209.55.06%20PM.png)

Here's the code I added to the CSS Editor:
```
[data-predefined-style="true"] [local-style="7485711"] bodycopy a {
    color: red;
}
```

It worked! Save the page.

![](attachments/Screen%20Shot%202021-10-04%20at%209.55.22%20PM.png)

Cargo adds these unique local style attributes to each component of your template. Use data attributes to target specific elements of the page without changing all of them.

## Squarespace
Create a new Squarespace trial site and click on Design in the left sidebar:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.23.01%20PM.png)

At the bottom, you'll find an option for Custom CSS.

![](attachments/Screen%20Shot%202021-10-04%20at%2010.23.27%20PM.png)

Unlike Cargo, Squarespace doesn't let you edit the full stylesheet. Instead, you can only **add new styles** that override the previous ones. (This is why I asked you to override my styles in [Activity—Burger CSS](Activity—Burger%20CSS.md))

![](attachments/Screen%20Shot%202021-10-04%20at%2010.23.42%20PM.png)

Note: If you open the Inspector with the CSS panel open, the page will display in mobile mode. Click the arrow in the top right to make the site fullscreen:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.25.51%20PM.png)

Say I want to make the "Shop Now" button have rounded corners.

![](attachments/Screen%20Shot%202021-10-04%20at%2010.31.57%20PM.png)

I locate the code in the inspector:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.31.55%20PM.png)

And add `border-radius: 100%` to the `element` section of the CSS:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.32.01%20PM.png)

It worked!

![](attachments/Screen%20Shot%202021-10-04%20at%2010.32.04%20PM.png)

Now, how to add this to your custom CSS?
If you want to change all buttons with this class, you'd copy this part of the HTML:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.32.50%20PM.png)

What you get is actually two different classes, separated by a space:
`sqs-block-button-element--large` and `sqs-block-button-element`

Since `sqs-block-button-element` sounds like it'll apply to more elements than the `large` option, I'll create CSS for that. I usually open up Atom to use as scratch paper.

```
.sqs-block-button-element {

}
```

![](attachments/Screen%20Shot%202021-10-04%20at%2010.34.59%20PM.png)

Copy the CSS you added to the element and put it inside the curly braces:

```
.sqs-block-button-element {
border-radius: 100%;
}
```

Now, copy this from Atom to the Squarespace CSS Editor and Save to test if it works.

![](attachments/Screen%20Shot%202021-10-04%20at%2010.36.06%20PM.png)

It works! All the buttons are rounded now.

![](attachments/Screen%20Shot%202021-10-04%20at%2010.36.18%20PM.png)

Say you only wanted to change the top button, not all of them. To select that one, look in your Inspector until you find a `div` with an `id` that starts with `yui`. Pick the closest parent to the button you're targeting:

![](attachments/Screen%20Shot%202021-10-04%20at%2010.36.27%20PM.png)

In this case, it's the `div` directly above the `a`

Select the `id` name

![](attachments/Screen%20Shot%202021-10-04%20at%2010.33.11%20PM.png)

Add the ID `yui_3_17_2_1_1633411800000_361` to your CSS so that you only target buttons that are nested inside elements with this ID.

```
#yui_3_17_2_1_1633411800000_361 .sqs-block-button-element {
border-radius: 100%;
}
```

Save your custom CSS. Now only that specific button will change.

Squarespace adds these unique IDs to every single section in your template. As you create new sections, you can always click in to select and change them individually by ID.