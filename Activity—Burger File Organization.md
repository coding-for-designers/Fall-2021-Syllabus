# Activity—Burger File Organization
**Updated Thursday September 23rd, 2021**
The font files will work now! Please re-download if you'd like to try this activity again.

## Setup
1. Download the [Burger Boilerplate](https://github.com/coding-for-designers/burger-boilerplate) files as a ZIP by clicking `Code > Download ZIP`
https://github.com/coding-for-designers/burger-boilerplate

Example:
![](attachments/Screen%20Shot%202021-09-20%20at%2010.06.42%20PM.png)

2. Next, open the `burger-boilerplate` folder in Atom (or other code editor)
3. In your browser, open `burger-boilerplate/index.htm`

## Activity
### Goal
Your goal is to re-arrange the files in `puzzle-pieces` to the correct folders so that the page looks like this:

`burger-boilerplate/index.htm`
![](attachments/Screen%20Shot%202021-09-20%20at%2010.09.16%20PM.png)

`burger-boilerplate/burger/index.htm`
![](attachments/Screen%20Shot%202021-09-20%20at%2010.09.07%20PM.png)

### Clues & Hints
1. You do not need to edit any code in Atom
	1. You can also open the code in your browser by clicking Tools > Web Developer > Page Source
2. You can achieve the goals by simply moving files from `puzzle-pieces` to the other folders
3. You only need to move the files in `puzzle-pieces`

**So, why open Atom?**
There are clues inside the code!
![](attachments/Screen%20Shot%202021-09-20%20at%2010.11.53%20PM.png)

This is what the page looks like when the images are broken, and only the alt text shows up:
![](attachments/Screen%20Shot%202021-09-20%20at%2010.12.40%20PM.png)

**What are all these fonts file formats?**
[WOFF2](https://caniuse.com/?search=woff2) is the most compressed, most modern web font format as of 2021, with 96% browser support.
WOFF is the previous version, with slightly wider compatibility with older browsers.
TTF is an even older version of webfont
EOT stands for "Embedded Open Type" and is used by older versions of Internet Explorer. 

By using all of these files, we can get close to 100% custom font support (but I usually only use WOFF2 with a system font fallback, more on this as we learn CSS in later weeks)