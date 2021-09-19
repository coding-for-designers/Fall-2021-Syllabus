# Week 3 - Layouts
Create fluid layouts and control the flow of content with minimal code.

Skip to [Homework](#Homework)

# Food for Thought
How can we shift our mindsets to design a system of constraints rather than absolutes? 

>"**Good things come to those who wait:** Projects sometimes take time to flourish. Avoid over-optimizing when you start out – many small steps over a longer period can lead to great things."
>
> [Web design principle 9: Use small and slow solutions](https://allcodesarebeautiful.com/en/permaculture-principle-9/ "Web design principle 9: Use small and slow solutions"), allcodesarebeautiful

>"They're less rigid, less performative, and less perfect than the personal websites we're used to seeing. It harkens back to the early days of the web when people had fewer notions of how websites "should be." It's an ethos that is both classically old and newly imagined."
>
>[Garden History](https://maggieappleton.com/garden-history), Maggie Appleton

>"If you find yourself wrestling with CSS layout, it’s likely you’re making decisions for browsers they should be making themselves."
>
>[Multi-column manipulation](https://every-layout.dev/blog/multi-column-manipulation/), Every Layout

>"A lot of folks don’t even know that flexbox and grid are supported [almost universally](https://www.caniuse.com/#feat=css-grid) now; but given how long it took to get from early spec work to broad implementation, I can’t really blame them."
>
>[Old CSS, new CSS](https://eev.ee/blog/2020/02/01/old-css-new-css/), eev.ee

>"As mobile phones have gotten bigger, many sites are setting this threshold higher. (I’ve seen it as high as 1400 pixels.) The problem is that this causes the mobile layout to show up even in reasonably sized desktop browser windows."
>
> On breakpoints. [Responsive web design](https://practicaltypography.com/responsive-web-design.html), Butterick's Practical Typography.

# Theory
CSS grids are powerful! Responsive design is algorithmic!

- CSS emulates print design
	- history of multicolumn layouts
- CSS for print
- CSS for screen
- multiple stylesheets
- font embeds
	- FOUT - Flash of Unstyled Text
- advanced css selectors like `+` and `>` and `:only-child` and `nth of type`
- Link `:hover` vs `:focus`
- `float` for text wrap
- E-publishing as subverting capitalism
	- Downloading is subversive
	- Website as free information distribution
	- Cost of creating a website vs. print publication
	- Creative print layouts on the screen, in the browser
- `vw` and `section`

## Fundamentals
- [Semantic Elements Review](Tutorials/Semantic%20Elements%20Review.md)
- [Display & Visibility](Tutorials/Display%20&%20Visibility.md)
- [Flexbox](Tutorials/Flexbox.md)
- [CSS Grids](Tutorials/CSS%20Grids.md)
- [Breakpoints](Tutorials/Breakpoints.md)

## Extras
- [Background Images & Gradients](Tutorials/Background%20Images%20&%20Gradients.md)
- [Column Grid for Images](Tutorials/CSS%20Column%20Grid.md)
- [Grid Sidebar Layout](Tutorials/Grid%20Sidebar%20Layout.md)
- [Sticky Elements](Tutorials/Sticky%20Elements.md)

# Workshop
## Activity—Two Rounded Rectangles
![](attachments/Screen%20Shot%202021-04-07%20at%203.36.17%20PM.png)

Apply a simpler version of the [Grid Sidebar Layout](Tutorials/Grid%20Sidebar%20Layout.md).

1. Create HTML document with two `<section>` tags, empty, side by side.
2. Set CSS body background to black and section `background-color` to white.
3. Set CSS section height to something like `20em`, adjust in Inspector
4. Set CSS body to `display:grid` with `grid-template-columns: 30% 1fr;`. Adjust `30%` to your liking.
5. Add `border-radius: 7em` and adjust to your liking. Add `grid-gap: 1.3em;` and adjust.
6. Resize browser. Cool!

### Responsive Rectangles
![](attachments/Screen%20Shot%202021-04-07%20at%203.36.25%20PM.png)

You must decide what width to "break" this layout. Use a [Breakpoint](Tutorials/Breakpoints.md) to collapse the rectangles for smaller screens. Publish on your Github site.

1. Using Inspector with Rulers turned on, resize page to find your ideal breakpoint width in pixels
2. Add media query for `@media (max-width: 775px)`, or whatever measurement you took in Inspector
3. Inside media query, style body with `grid-template-columns: 1fr;`. This creates a single column layout.
4. Resize browser. Wow! 👀

## Demo—Image Grid
Masonry grid with pure CSS. In Code Demos > Week 3

![](attachments/Screen%20Shot%202021-04-24%20at%205.00.50%20PM.png)
See [CSS Column Grid](Tutorials/CSS%20Column%20Grid.md)

## Print to screen
Using columns, grid, and `<section>`, `<aside>`, recreate a printed editorial or book layout as a website.

Remember to use units `%`, `em`, and `vw`

Copy text from gutenberg project

# Homework
1. Update your Github Pages website with styles
2. Complete Reading

## Site Requirements
Apply any responsive layout technique to your site. 
Suggestions:
- [Grid Sidebar Layout](Tutorials/Grid%20Sidebar%20Layout.md)
- [Breakpoints](Tutorials/Breakpoints.md)
- [1 Line Layouts](https://1linelayouts.glitch.me/) - one line CSS layouts! Must-see!

## Reading
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