# Resources
*This page is in the process of being organized and adapted for fall cohort*

## General Principles
>"**Good things come to those who wait:** Projects sometimes take time to flourish. Avoid over-optimizing when you start out – many small steps over a longer period can lead to great things."
>
> [Web design principle 9: Use small and slow solutions](https://allcodesarebeautiful.com/en/permaculture-principle-9/ "Web design principle 9: Use small and slow solutions"), allcodesarebeautiful

## HTML
- [List of HTML elements](https://html.spec.whatwg.org/multipage/#toc-semantics) from the current maintainers of HTML - the WHATWG
- [Intro to HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) from the MDN Web Docs
- [HTML Accessibility](https://www.w3schools.com/html/html_accessibility.asp) - tips on which elements to use for semantic meaning
- [Organize your text content](https://thomasorus.com/organize-your-text-content.html) - More tips on HTML elements
- [What is alt-text and why is it important?](https://poetry.arizona.edu/blog/what-alt-text-and-why-it-important) - Best practices for alt text as poetry

>"If you find yourself wrestling with CSS layout, it’s likely you’re making decisions for browsers they should be making themselves."
>
>[Multi-column manipulation](https://every-layout.dev/blog/multi-column-manipulation/), Every Layout

- [Build an Under Construction Page](https://www.zinesbyjackie.com/activities/build-an-under-construction-page) - 90s inspired activity with step by step HTML generation
- [On Gathering](https://www.shiftspace.pub/on-gathering-mindy-seu) - Article by Mindy Seu
	- As you read, think about the connotation of the word `index` as the default page
- [WHATWG's Living Standard](https://html.spec.whatwg.org/multipage/introduction.html#history-2) - explanation for the drama between browsers and the W3, why we're in a post-HTML5 world
- https://html.energy/ - Podcast on HTML


## CSS
- [CSS Reference](https://www.w3schools.com/cssref/) - list of CSS Properties
- [system stack](https://css-tricks.com/snippets/css/font-stacks/)
- Use [CSS Validator](https://jigsaw.w3.org/css-validator/validator.html.en#validate-by-input) to check for errors
- [wrapped up in curly braces](https://curly-braces.hashbase.io/) - a love letter to css. Also a walkthrough of basic CSS concepts, history, and properties to get started with!
- [CSS System Font Stacks](https://css-tricks.com/snippets/css/font-stacks/) - Add these to `:root` or `body` to set your page's typeface using fonts most people already have installed.
- [Units](https://every-layout.dev/rudiments/units/) - How to use CSS units algorithmically instead of defining every `px` manually
- [CSS pro tips: responsive font-sizes and when to use which units](https://bits.theorem.co/css-pro-tips-responsive-font-sizes-and-when-to-use-which-units/) - One line hack for responsive typography sizing, building on the theory in "Units" above

>CSS allows complete and total control over the style of a hypertext document. The only way this can be illustrated in a way that gets people excited is by demonstrating what it can truly be, once the reins are placed in the hands of those able to create beauty from structure. Designers and coders alike have contributed to the beauty of the web; we can always push it further.
>http://www.csszengarden.com/, launched in [2003](https://en.wikipedia.org/wiki/CSS_Zen_Garden)

>Learn to extrapolate your layouts from your text’s intrinsic dimensions and your designs will be beautiful.
>https://every-layout.dev/rudiments/units/

>"...we must relinquish control to the algorithms (like text wrapping) browsers use to lay out web pages automatically... Think of yourself as the browser’s mentor, rather than its micro-manager."
https://every-layout.dev/rudiments/axioms/

>"I think we've reached the point where html/css is more powerful, and nicer to use than ever before. Instead of starting with a giant template filled with .js includes, it's now okay to just write plain HTML from scratch again.“
>https://jeffhuang.com/designed_to_last/

- [Old CSS, New CSS](https://eev.ee/blog/2020/02/01/old-css-new-css/) - a history of CSS by a web designer who has been coding since the 90s.
	- As you read, think about the Space Jam case study and how difficult it would be to maintain page styling using those methods today
	- Think about how archaic techniques such as `float` and `div` for layout are still widespread. "The web is still a _little bit_ of a disaster. A lot of folks don’t even know that flexbox and grid are supported [almost universally](https://www.caniuse.com/#feat=css-grid) now"
- [A brief history of CSS until 2016](https://www.w3.org/Style/CSS20/history.html) by the W3
	- Try disabling the CSS on this page—are the animations and styling pure CSS, including the start/stop animation button? No Javascript necessary?
	- This is the site I shared in [Week 1 - Hypertext](Week%201%20-%20Hypertext.md)!
- [Focus vs. Hover](https://thatjdanisso.cool/a11y/focus-vs-hover) - tips on `:hover` styling for accessibility
- [Anchor Links#Original Hypertext Goals](Anchor%20Links#Original%20Hypertext%20Goals.md) - 1983 web experiment called [Intermedia](https://www.are.na/blog/hyperland-intermedia-and-the-web-that-never-was) and how it shaped the anchor link today
- [CSS Selectors](https://flaviocopes.com/css-selectors/) - by Flavio Copes

### CSS Display
- https://www.w3schools.com/css/css_display_visibility.asp
- [Understanding CSS Display: None, Block, Inline and Inline-Block](https://betterprogramming.pub/understanding-css-display-none-block-inline-and-inline-block-63f6510df93?gi=e30442b6d8ee)

### CSS Flexbox Tutorials
- [Flexbox, the GOAT](https://thomasorus.com/flexbox-the-goat.html)
- [The Flexbox Guide](https://flaviocopes.com/flexbox/)
- [Common Flexbox Patterns](https://tobiasahlin.com/blog/common-flexbox-patterns/)

### CSS Grid Tutorials
- [CSS Grid Tutorial](https://flaviocopes.com/css-grid/)
- [The Sidebar](https://every-layout.dev/layouts/sidebar/)

### Sticky elements
- [How To - Sticky Element](https://www.w3schools.com/howto/howto_css_sticky_element.asp) - Sticky header on W3Schools
- [How to Use CSS Grid for Sticky Headers and Footers](https://css-tricks.com/how-to-use-css-grid-for-sticky-headers-and-footers/)
- [Beginner CSS Grid: Sticky Navigation, Scrolling Content](https://medium.com/@beyondborders/beginner-css-grid-sticky-navigation-scrolling-content-7c4de0a8d1dc)

### Optional Reading
- [Multi-column manipulation](https://every-layout.dev/blog/multi-column-manipulation/) using `column:` property
- [CSS Columns](https://developer.mozilla.org/en-US/docs/Web/CSS/columns)
- [Responsive Spacing with Viewport Units](https://chipcullen.com/responsive-spacing-with-viewport-units/)
- [Building websites for Safari Reader Mode and other reading apps](https://medium.com/@mandy.michael/building-websites-for-safari-reader-mode-and-other-reading-apps-1562913c86c9)

>“Have you had it with linear media?” it asks. “Are you tired of television that just _happens_ to you_?_”
>
>[Hyperland](https://www.are.na/blog/hyperland-intermedia-and-the-web-that-never-was), a BBC documentary released in 1990

### Translation & Transformation
- https://codyhouse.co/nuggets/3d-perspective
- https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate()
- https://developer.mozilla.org/en-US/docs/Web/CSS/transform

### Animation
- https://developer.mozilla.org/en-US/docs/Web/CSS/transition
- https://developer.mozilla.org/en-US/docs/Web/CSS/@keyframes
- https://developer.mozilla.org/en-US/docs/Web/CSS/animation
- [CSS Animation Libraries](Tutorials/CSS%20Animation%20Libraries.md)

### Custom Domain Name
- [Github and Dreamhost Custom Domain](https://medium.com/@melissamcewen/getting-github-pages-to-work-with-a-dreamhost-domain-5fcefac93063)
- [Namecheap Domain with Github Pages](https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages/)

### Custom Cursor
- [Using URL values for the cursor property](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Basic_User_Interface/Using_URL_values_for_the_cursor_property) - Custom cursor tutorial by Mozilla
- [Custom Cursor & Hover](Tutorials/Custom%20Cursor%20&%20Hover.md)

### Overlapping Images
- [How to Overlap Images in CSS](https://bricampgomez.com/blog/how-to-overlap-images-in-css/) - Trendy overlapping photo grid (check out the custom cursor on this site also!)

### Backgrounds
- [https://css-tricks.com/full-page-background-video-styles/](https://css-tricks.com/full-page-background-video-styles/)
- [Background Images & Gradients](Tutorials/Background%20Images%20&%20Gradients.md)

### Border Radius
- [Expanded Use of box-shadow and border-radius](https://moderncss.dev/expanded-use-of-box-shadow-and-border-radius/) - create blob shapes with pure CSS
- [Fancy Border Radius Generator](https://9elements.github.io/fancy-border-radius)

### Outer Glow
- [CSS Glowing Text](https://www.w3schools.com/howto/howto_css_glowing_text.asp)

>“In any case, however the system looks in three, five, or fifty years, we believe that the vision we've laid out above has the flexibility and functionality to start tying everything together without forcing everyone to use the same access methods or to look at the net the same way.”  
>
>[RFC 1727](https://tools.ietf.org/html/rfc1727) Resource Transponders, December 1994

### Fonts Fonts Fonts!
- [Webfonts Guide by Mozilla](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts) - step by step including `font-face` and file conversion
- [font-feature-settings by Mozilla](https://developer.mozilla.org/en-US/docs/Web/CSS/font-feature-settings) - alternate stylistic sets for OpenType fonts, referenced in [OpenType Features](Tutorials/OpenType%20Features.md)
- [Variable Fonts Guide by Mozilla](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts/Variable_Fonts_Guide) - in depth explanation of static vs variable webfonts
- [Introduction to variable fonts on the web](https://web.dev/variable-fonts/) - good reference for CSS you can copy
- [Implementing Variable Fonts](https://variablefonts.io/implementing-variable-fonts/) - good advice on self hosting and how to write fallbacks with `@supports` in a minimal way with just one font file
- [Wakamai Fondue](https://wakamaifondue.com/beta/) - tool to check what stylistic sets and glyphs your font has as well as generate CSS
- [Alternate Figures](https://practicaltypography.com/alternate-figures.html) on Butterick's Practical Typography
- [font-variant by Mozilla](https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-variant) - how to activate alternate figures like small caps, ordinal numbers, tabular nums, etc.
- [Lusitana Font Download](https://megu.space/free-font-lusitana-by-ana-megda/) - the one I used in the Editorial Layout demo
- Remember to check caniuse.com for advanced font CSS that I didn't list above, since they might not be supported on a majority of browsers yet

### Editorial Styling
- [A Whole Bunch of Amazing Stuff Pseudo Elements Can Do](https://css-tricks.com/pseudo-element-roundup/) - check out the image floated between two columns for an editorial look
- [Smart Quotes Plus](https://atom.io/packages/smart-quotes-plus) - Atom plugin to replace all quotes and apostrophes with smart ones

### Advanced CSS
- [::before / ::after](https://css-tricks.com/almanac/selectors/a/after-and-before/)
- [Multi-column manipulation](https://every-layout.dev/blog/multi-column-manipulation/) - Every Layout explains CSS columns
- [CSS Scroll Snap](https://codyhouse.co/nuggets/scroll-snap)
- [calc()](https://css-tricks.com/a-complete-guide-to-calc-in-css/)
- [Responsive font size calc() hack](https://bits.theorem.co/css-pro-tips-responsive-font-sizes-and-when-to-use-which-units/) - using `vw`



>Back in 1993, you weren't a designer, developer, copywriter or in devops. You were a fucking webmaster, and your name was at the bottom of every page.
>
>If you had a question, you emailed [webmaster@tomstrucking.net](mailto:webmaster@tomstrucking.net).
And that address got a lot of emails:
>-   "Please play the Star Trek theme when people get to my site."  
>-   "Can you put a hit counter on my web page?"  
>-   "I want my headline to be blinking."
>
>Folks treated webmasters like goddamned magicians. Just email us with your cyberspace dreams, and we'll make them a reality.
>
>https://justinjackson.ca/webmaster/