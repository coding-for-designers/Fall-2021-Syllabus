# Week 2 - Styles
Apply styles with CSS. Unlearn pixel-based thinking and design a system of constraints.

Skip to [Homework](#Homework)

# Food for Thought
What is the role of default design in web development? How can we design a website directly in the browser?

What happens if we try to design "against the flow" of a browser's default settings? How can we design web experiences that will last 10, 20, 30 years? 

>The saga of CSS starts in 1994. Håkon Wium Lie works at CERN – the cradle of the Web – and the Web is starting to be used as a platform for electronic publishing. One crucial part of a publishing platform is missing, however: There is no way to style documents.
>https://www.w3.org/Style/CSS20/history.html

>CSS allows complete and total control over the style of a hypertext document. The only way this can be illustrated in a way that gets people excited is by demonstrating what it can truly be, once the reins are placed in the hands of those able to create beauty from structure. Designers and coders alike have contributed to the beauty of the web; we can always push it further.
>http://www.csszengarden.com/, launched in [2003](https://en.wikipedia.org/wiki/CSS_Zen_Garden)

>Learn to extrapolate your layouts from your text’s intrinsic dimensions and your designs will be beautiful.
>https://every-layout.dev/rudiments/units/

>"...we must relinquish control to the algorithms (like text wrapping) browsers use to lay out web pages automatically... Think of yourself as the browser’s mentor, rather than its micro-manager."
https://every-layout.dev/rudiments/axioms/

>"I think we've reached the point where html/css is more powerful, and nicer to use than ever before. Instead of starting with a giant template filled with .js includes, it's now okay to just write plain HTML from scratch again.“
>https://jeffhuang.com/designed_to_last/

# Theory
CSS is elegant! CSS is powerful!

Goals: By the end of this course, I'd like you all to think of **Firefox + Atom** when you want to design a website. Not Sketch, Figma, etc. CSS can do so much that graphics programs cannot, and the happy accidents that occur while coding a page in the browser's Inspector are an important part of the web design process.

- Browser is like Photoshop
	- assets like fonts must be installed on system with the same name
	- or embedded in the page
	- pages are loaded and rendered by the browser software
- client side vs. server side
	- local vs remote environment
	- there is no cloud
- The Small web
	- Designing this way is simple, minimal, small
	- Doesn't rely on plugins
- Privacy and third party scripts
- css changes styles of html
- history of css
- backgrounds, background images
- svg mask, border radius
- outer glow, drop shadow
- basic selectors, classes & IDs
- CSS validator
- Atom & Github setup

- [Pixel Scaling Across Devices](Tutorials/Pixel%20Scaling%20Across%20Devices.md)
- [CSS Syntax](Tutorials/CSS%20Syntax.md)
- [CSS Selectors](Tutorials/CSS%20Selectors.md)
- [Inline vs Linked Stylesheet](Tutorials/Inline%20vs%20Linked%20Stylesheet.md)
- [Order Matters - The Cascade](Tutorials/Order%20Matters%20-%20The%20Cascade.md)
- [Comments and CSS organization](Tutorials/Comments%20and%20CSS%20organization.md)
- [Classes & IDs](Tutorials/Classes%20&%20IDs.md)
- [Pixel Perfect doesn't exist on the web](Tutorials/Pixel%20Perfect%20doesn't%20exist%20on%20the%20web.md)
- [Common CSS Properties](Tutorials/Common%20CSS%20Properties.md)
- [Box Model](Tutorials/Box%20Model.md)
- [Web Inspector](Tutorials/Web%20Inspector.md)
- [Tutorials/Aligning to Center](Tutorials/Aligning%20to%20Center.md)
- [Styling Images in CSS](Tutorials/Styling%20Images%20in%20CSS.md)
- [Responsive Images](Tutorials/Responsive%20Images.md)
- [Browser Compatibility & CSS](Tutorials/Browser%20Compatibility%20&%20CSS.md)

Remember! `font-color` doesn't exist. It's `color`!!

# Workshop
## Demo—Live Coding
I'll style the [HTML demo from last week](https://github.com/meewgumi/Coding-For-Designers/blob/main/Code%20Demos/Week%201%20-%20HTML/html.htm), inspired by this [Actual Source email design](https://mailchi.mp/49d14e17f6ad/actual-source-spring-sale2021).

**STUDENTS SHOULD LEARN CODEPEN OR GLITCH HERE**
Github Gist
Share code on Slack
Markdown code tick marks

## Demo—Inspector Workflow
I'll explain [Box Model](Tutorials/Box%20Model.md) viewer in Inspector. How to use arrow keys to adjust units and use that to copy + paste to your code editor. In this way, we can use the Inspector as a design tool.

![](attachments/Screen%20Shot%202021-04-06%20at%207.01.59%20PM.png)

I'll probably go through this process:
- max-width and `margin: 0 auto`
- Resize browser and adjust width until it looks good at all sizes
- Add padding with em, rem
- Style `a` and `a:hover`
- font-size
	- set at `:root` level
- background-color
- line-height `%`
- letter-spacing use `em`
- **text-transform**
	- uppercase
	- lowercase
- **text-align**
	- left, center, right
- text-decoration
- width - use `%`, `em`, or `vw`
- `border: 1px solid #000000`

## Furniture as website
Using `div`, gradients, border radius, z-index, and rotations, create a page for a piece of furniture.

Familiarize yourself with the `em` as a unit.

Custom cursor as PNG

![[2021-06-19 19.46.37.png]]

# Homework
*due by the start of next class, submit via Slack*

1. Discuss site references with Megumi during Office Hours (or via email or Slack). Come up with a plan to implement a style for your final project.
2. Update your Github Pages website with Site Requirements below
3. Complete Required Reading

**Tips:**
- Edit `index.htm` alongside `style.css` to achieve the best styling
- Use semantic elements like `section` and `figcaption` first, `div` and [Classes & IDs](Tutorials/Classes%20&%20IDs.md) as a last resort
- `color:` edits font color (font-color doesn't exist!)
- Use [CSS Validator](https://jigsaw.w3.org/css-validator/validator.html.en#validate-by-input) to check for errors

## Site Requirements
Add a stylesheet to your Github site. Use any styles you learned today!

- Save a file called `style.css`
- Link this file to all your HTML pages (Instructions at [Inline vs Linked Stylesheet](Tutorials/Inline%20vs%20Linked%20Stylesheet.md))

### Optional
- Define font face using [system stack](https://css-tricks.com/snippets/css/font-stacks/)
- Style links with `a` selector
- Style link hover with `a:hover`
- If you have images on the page, add a `max-width`
- Add images and figcaption, style with CSS
- Test your CSS in https://doiuse.herokuapp.com/ and achieve <10% breakage

## Required Reading
- [CSS Reference](https://www.w3schools.com/cssref/) - list of CSS Properties
- [wrapped up in curly braces](https://curly-braces.hashbase.io/) - a love letter to css. Also a walkthrough of basic CSS concepts, history, and properties to get started with!
- [CSS System Font Stacks](https://css-tricks.com/snippets/css/font-stacks/) - Add these to `:root` or `body` to set your page's typeface using fonts most people already have installed. We'll embed custom typefaces in [Week 5 - Animation](Week%205%20-%20Animation.md).
- [Units](https://every-layout.dev/rudiments/units/) - How to use CSS units algorithmically instead of defining every `px` manually
- [CSS pro tips: responsive font-sizes and when to use which units](https://bits.theorem.co/css-pro-tips-responsive-font-sizes-and-when-to-use-which-units/) - One line hack for responsive typography sizing, building on the theory in "Units" above

## Optional Reading
- [Old CSS, New CSS](https://eev.ee/blog/2020/02/01/old-css-new-css/) - a history of CSS by a web designer who has been coding since the 90s.
	- As you read, think about the Space Jam case study and how difficult it would be to maintain page styling using those methods today
	- Think about how archaic techniques such as `float` and `div` for layout are still widespread. "The web is still a _little bit_ of a disaster. A lot of folks don’t even know that flexbox and grid are supported [almost universally](https://www.caniuse.com/#feat=css-grid) now"
- [A brief history of CSS until 2016](https://www.w3.org/Style/CSS20/history.html) by the W3
	- Try disabling the CSS on this page—are the animations and styling pure CSS, including the start/stop animation button? No Javascript necessary?
	- This is the site I shared in [Week 1 - Hypertext](Week%201%20-%20Hypertext.md)!
- [Focus vs. Hover](https://thatjdanisso.cool/a11y/focus-vs-hover) - tips on `:hover` styling for accessibility
- [Anchor Links#Original Hypertext Goals](Anchor%20Links#Original%20Hypertext%20Goals.md) - 1983 web experiment called [Intermedia](https://www.are.na/blog/hyperland-intermedia-and-the-web-that-never-was) and how it shaped the anchor link today
- [CSS Selectors](https://flaviocopes.com/css-selectors/) - by Flavio Copes