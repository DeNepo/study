# The DOM

The simplest way to begin understanding how the DOM works is to understand the lifecycle of an HTML/cSS web page.

You'll know you have mastered this repo when you understand (and can explain to someone else!) the 3 stages in an HTML page's life-cycle using your DevTools and any simple website:

1. __HTML & CSS Source Code__: This is the text that you write in a .html file and open with your browser.  HTML is a _mark up language_, meaning it describes to a computer how you want the content on your web page to be organized behind the scenes. CSS is a language to describe how your web page should be rendered on the screen. You can't edit the source code from the browser, only from your text editor. Any changes you make in the browser will disappear when you refresh the page.
2. __The DOM Tree__: When you open an HTML file in your browser, it _parses_ the code you wrote and builds the __DOM Tree__.  The DOM Tree is very similar to your HTML but will not be exactly the same, \<table> tags are helpful for understanding this.
3. __Rendered Content__: The DOM is an _abstract representation_ of the content in your website, it is NOT exactly what you see on the screen. This is easiest to understand when you think of CSS: it is possible to write one div below anther in your .html file, have them in that order in the DOM (dev tools), then switch them on screen in the final rendering using CSS. Why is this? Because (aproximately) HTML is used to describe the DOM, and CSS is used to describe how the DOM is rendered.  (don't worry if that doesn't make sense right away, it'll take some practice to wrap your head around the idea).

"Great!" you say  "This is a very well written explanation. But why does this matter, can't I just make pretty things?".  Yes, you could just hack together some HTML & CSS to make pretty pages, but without learning to use the Developer Tools and without understanding the HTML lifecycle (_HTML+CSS source code -> the DOM -> rendered content_), you'll never leave the minor leagues.

Not only is it very difficult to catch your mistakes in HTML & CSS without mastering the DevTools, but mastering the DevTools _before_ moving on to JavaScript DOM Manipulation is one of the single most helpful things you can do to prepare.

JavaScript DOM Manipulation interacts with __The DOM Tree__ _after_ the DOM is built for the first time, and triggers the browser to create new Rendered Content with each manipulation.  If you do not understand the difference between these 3 steps, you will have a hard time understanding what's going on with JavaScript and will often ask questions like "why did my JavaScript not change the HTML file?" or "How come what I see in my inspector looks nothing like my source code?".

---

## Resources

### What is the DOM?

* articles: [w3schools.com](https://www.w3schools.com/js/js_htmldom.asp), [css-tricks.com](https://css-tricks.com/dom/)
* videos: [freecodecamp](https://www.youtube.com/watch?v=80Mr2Z6Qikc), [udacity](https://www.youtube.com/watch?v=tSv2KIF7uE4)
* [javascript.info](https://javascript.info/document) - .1 & .2 are enough for this purpose

### HTML -> DOM, CSS -> Rendering:

* [stack overflow](https://stackoverflow.com/questions/4800538/client-side-html-dom-and-css)
* [frontend babel](http://frontendbabel.info/articles/webpage-rendering-101/)

### Interactive Study

* [Live DOM Viewer](https://software.hixie.ch/utilities/js/live-dom-viewer/)
* [DOM Tutor](https://janke-learning.org/dom-tutor)
* [Inspecting the DOM](https://hackyourfuture.be/inspecting-the-dom/)
* [In-Depth Embedded Tutorial](https://dom-tutorials.appspot.com/static/index.html) - uses some JavaScript


### Dev Tools:

* FireFox: [what are the devtools?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools), [how to open them](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Open_the_Inspector), [editing live sites](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Examine_and_edit_HTML)
* Chrome, Chromium, Brave: [Getting Started Inspecting](https://developers.google.com/web/tools/chrome-devtools/dom/)

---
---
### <a href="https://hackyourfuture.be" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/63941625-4c7c3d00-ca6c-11e9-9a76-8d5e3632fe70.jpg" width="100" height="100" alt="Hack Your Future: Belgium"></a>
