# Week 5 - Animation
Harness the power of variable fonts. Customize features such as ligatures, stylistic sets, and tabular numbers.

Skip to [Homework](#Homework)

# Food for Thought
_What are designers better at coding, compared to non-designers?_ Which CSS concepts seem to be created for designers? CSS is wide and expansive, what corner of it can designers stake a claim in?

>“In any case, however the system looks in three, five, or fifty years, we believe that the vision we've laid out above has the flexibility and functionality to start tying everything together without forcing everyone to use the same access methods or to look at the net the same way.”  
>
>[RFC 1727](https://tools.ietf.org/html/rfc1727) Resource Transponders, December 1994

>"...associative indexing, the basic idea of which is a provision whereby any item may be caused at will to select immediately and automatically another. This is the essential feature of the memex. The process of tying two items together is the important thing."
>
1945 article in The Atlantic: https://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/

>There are now online services where you can find and download fonts (both free and non-free). And some even offer to host the fonts on their servers. In some cases even for free. (Which means they provide bandwidth, but in return they gather statistics on font usage).
>
>https://www.w3.org/Style/CSS20/history.html

# Theory
- Keyframes
- History of CSS animation
- CSS is absorbing other languages, especially Javascript
- Use Javascript to fill in gaps
	- CSS limitations and Javascript library examples
	- Where to put Javascript in your site
	- Browse web with Javascript turned off
- FOUT - Flash of Unstyled Text
	- Javascript loads after HTML and CSS, be aware of this
- What can you animate in CSS?
- CSS animation is more lightweight and accessible than JS in most cases, but it has limitations
	- Can load on browsers with JS disabled, including old Cricket phone
- CSS `:before` and hover styles
- Video background
- Gif hover effects
- Computing power, energy, and the green web


- [Custom font embeds](Tutorials/Custom%20font%20embeds.md)
- [WOFF2 Conversion](Tutorials/WOFF2%20Conversion.md)
- [OpenType Features](Tutorials/OpenType%20Features.md)
- [Variable Fonts in Inspector](Tutorials/Variable%20Fonts%20in%20Inspector.md)
- [Editorial Style Paragraphs](Tutorials/Editorial%20Style%20Paragraphs.md)
- [Floats](Tutorials/Floats.md)

# Workshop
See [Week 5 Demos](Code%20Demos/Week%205/Week%205%20Demos.md) for live links

## Editorial Styling
Go over `@font-face`
[Editorial Style Paragraphs](Tutorials/Editorial%20Style%20Paragraphs.md)
Small caps instead of bold type

## Variable Space Grotesk
Use Dev tools to customize variable fonts
Use Wakamai Fondue to see OTF font features

## Hello World hover emoji

## nth of type image cursor hover

## animated gradient background

## cut fruit rotation hover

## Movement
What is a "button" ? Think of the metaphor of a button as you create an interactive or animated page with a clickable button.

Your button can be `button` or `a`, and it doesn't need to go anywhere, but it needs at least two "states":
- Base (default) state
- Secondary state that appears with either: hover, click, or time delay animation


- You may include more than two states

# Homework
1.  For next week, bring any mobile devices you have so we can test our sites on different operating systems

## Site Requirements
- Your site should use at least 1 custom webfont. (Do NOT upload paid typefaces to Github unless your repo is private. Avoid font piracy!)
- Apply everything you've learned so far to customize your index and about pages. Expand on the content there, personalize it, make it about you as a web designer.

## Reading
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



