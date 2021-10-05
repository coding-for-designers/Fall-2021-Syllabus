# How to steal (responsibly)
Use the inspector to figure out how any website works! In my demo, I'll go through [this site](https://www.aqnb.com/2017/11/22/anja-kaiser-talks-alternative-narrations-of-bodies-new-online-commission-bye-default-in-the-run-up-to-3hd-festival/)

At first, stealing code will be a learning experience. Once you get better at picking websites apart, you can get inspiration from other peoples' source code and start creating your own original styles. This process is my go-to for learning how to do anything cool you see on the web!

Note: don't copy paste code for a real project! Just do this for educational purposes.

## Steps
Select the element you want to inspect. I chose the image hover effect—it starts faded out by default, then fades in when you hover over it.

![](attachments/Screen%20Shot%202021-10-04%20at%209.23.24%20PM.png)

Start unchecking boxes next to properties that you think create the effect. This is largely trial and error. In this case, it was `opacity` that creates the faded effect.
![](attachments/Screen%20Shot%202021-10-04%20at%209.23.31%20PM.png)

Next, click `:hov` to toggle pseudo classes. We'll use this to figure out how the hover effect works.
![](attachments/Screen%20Shot%202021-10-04%20at%209.23.39%20PM.png)

By checking `:hover`, the hover state is permanently activated in the browser. Now, you'll see the hover state for your selected element. Start unchecking things and try to figure out how your effect works through trial and error.
![](attachments/Screen%20Shot%202021-10-04%20at%209.23.46%20PM.png)

After some trial and error, it looks like `opacity: 1` is the part that makes the image fade in. Let's test out the theory by changing the value from 1 to 0.2. Sure enough, the image gets lighter!
![](attachments/Screen%20Shot%202021-10-04%20at%209.24.00%20PM%201.png)

We've narrowed it down to these two sections. Select them and copy + paste to Atom.
![](attachments/Screen%20Shot%202021-10-04%20at%209.24.20%20PM.png)

Add the CSS either to an internal stylesheet or an external one.
![](attachments/Screen%20Shot%202021-10-04%20at%209.26.40%20PM.png)

Now we start to create the HTML elements described in the CSS.
![](attachments/Screen%20Shot%202021-10-04%20at%209.26.51%20PM.png)

Since `img` was nested inside `figure`, we create that here:
![](attachments/Screen%20Shot%202021-10-04%20at%209.28.37%20PM.png)

Save the file and open in your browser. Does the effect work? Yes it does!
![](attachments/Screen%20Shot%202021-10-04%20at%209.28.51%20PM.png)
![](attachments/Screen%20Shot%202021-10-04%20at%209.28.54%20PM.png)

However, the image is huge. Since we only took some of the CSS, we don't have any of the properties that control image size. Let's add in `width: 100%` at the bottom of the `figure img` section
![](attachments/Screen%20Shot%202021-10-04%20at%209.29.29%20PM.png)

The last step is to start unchecking properties to see if they change anything in your desired effect. In your code, delete the ones that are unnecessary. You can also try changing the values (ie., I changed the transition to 3s here for a slower fade)
![](attachments/Screen%20Shot%202021-10-04%20at%209.30.42%20PM.png)

This is my favorite way to learn new techniques—you can search for the new properties you mess with and read the documentation. For example, if you look up [transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition) you can find all kinds of different values you can set here.

## Give it a try!
1. Pick any website
2. Choose one element or style to investigate
3. Follow the steps above to find the CSS
4. Repeat!