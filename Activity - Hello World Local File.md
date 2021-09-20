# Activity - Hello World Local File
## Goal
Create a basic HTML page that says "Hello World" by using Atom, a code editor program on your computer.

`Local` = your computer. By opening an HTML file in your web browser, you'll see the URL start with `file:///`, meaning it's loading from your computer and not the www.

## Instructions
### Copy your code
1. Open a code editor such as Atom
	1. View [suggested code editors here](https://github.com/coding-for-designers/getting-started)
	2. You can also use TextEdit or Notepad, as long as you're in "Plain Text" mode

![](attachments/Screen%20Shot%202021-09-19%20at%2010.20.06%20PM.png)

2. Copy your HTML code from [Activity - Hello World Codepen](Activity%20-%20Hello%20World%20Codepen.md)
3. Paste into your text editor
4. Save file as `helloworld.htm`
	1. Make sure your text editor doesn't add any other extensions, such as `.txt`
	2. Best practice: Don't use spaces or symbols, except `-` and `_`
5. Open `helloworld.htm` in your web browser
6. Take a screenshot and share with the Classroom Figma!

### Add Structure
HTML documents need some elements by default. Add these to your `helloworld.htm` file and save it.

`<!DOCTYPE HTML>` must be placed at the top of the file.
`<html>` is where all your code goes
`<head>` contains metadata elements such as `<title>`, which controls the title in the browser window
`<body>` is where you paste all your content—aka everything from your Codepen.

```
<!DOCTYPE HTML>
	<html>
		<head>
			<title>Page Title</title>
		</head>
		<body>
			<h1>Hello World!</h1>
		</body>
	</html>

```

### Create a folder
Create a place for all your web projects! I like to put all my projects in folders inside a larger folder called `Web`

Here's an example of the folder nesting:
- Web
	- Hello World
		- helloworld.htm

For each new activity, create a new folder under `/Web` !

### Add images
1. Find an image you'd like to display on your page (jpg, png, gif)
2. Save the image to the `Hello World` folder you created in the last step. Make sure the image is in the same folder as `helloworld.htm`
3. Use the `img` tag to display the image on the page ([instructions](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img))
4. Use the `width` attribute to change the image dimensions (height will be calculated automatically)

### Add more elements
If you have more time, browse the WHATWG's index of [HTML Elements](https://html.spec.whatwg.org/multipage/indices.html#elements-3) or the [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML) and choose some elements to add to your Codepen. Have fun!

Here are some to get started with: 
- [Blockquote](https://html.spec.whatwg.org/multipage/grouping-content.html#the-blockquote-element)
- [Bulleted List](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)
- [Code](https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-code-element)
- [Horizontal Rule](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/hr)
- [Tables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)
- [Marquee](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/marquee)

## Share your work
**Share a screenshot of your page on the Classroom Gallery!**