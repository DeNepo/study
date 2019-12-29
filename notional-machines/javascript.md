# JavaScript

The best way to learn JavaScript is from the inside-out, focusing first on how your code is interpreted and how memory is managed then later learning to apply this to practical problems. Most introductions to JS cover the language from the outside in, focusing on the most interesting, practical or "intuitive" features first and directly apply them to programming challenges.

This approach feels satisfying at first but will quickly slow your progress when you have difficulties determining if your bugs come from mistakes in logic or a misunderstanding of JavaScript. Integrating more advanced language features like reference/value or asynchronous execution will also be nothing but confusion if you don't have a solid mental model of JS to build them on top of.

Instead take the time to learn from the inside out, building your notional machine in layers. focusing first on how the JS engine interprets commands and manages memory, building from the base concepts of program execution and errors all the way up to more complicated features like `this` and closure.  After mastering JavaScript's inner workings you'll find problem solving and programming strategies are much more approachable.

Many of the exercises you will be assigned while at HYF are designed specifically to help you master the JS notional machine.  These exercises will all have links that help you to study your exercises directly in a visualization tool.  Many of these exercises will also feel abstract and irrelevant. But push through, and use the visualization tools!  If you spend the time to complete these exercises, you'll find that the more interesting problem-solving exercises and weekly projects will be much more understandable.

## The Core

> psst.  "The Core" isn't an official term, it's just a helpful way to talk about all JS language features that take place on the main _thread_.  Don't worry too much about this for now, you'll more about this later on.

At the core of JS are a few key concept necessary to understand how memory works in JS scripts, these include:

* _program life-cycle_: JS scripts are executed in two phases. The initial _creation phase_ reads through your source code already preparing certain things in memory ("hoisting").  The subsequent _execution phase_ is when the JS interpreter steps through your code one step at time, following your instructions on how to update program memory.
* _errors_:  Errors occur when you instruct the JS interpreter to do something it can't do or isn't allowed to do. There are two major types of errors, and these can happen in either of the 2 stages of your program's life-cycle.
* _variables and their values_: Point at any variable in a file of JS code, can you say exactly where it's value is coming from? This may sound like a strange question and unrelated to solving cool problems, but it's actually one of _the most important skills_ you can develop while with us at HYF. Without this skill debuggers won't make sense, errors can be impossible to track down, and it's next to impossible to come up with clever solutions to the problems you encounter.
* _types, values & operators_: The heart of any application is it's data.  And data is represented at it's lowest level as primitive values.  Understanding how _primitive types & values_ work, and how they're transformed throughout program execution using _primitive operators_ is the purest and most basic of programming skills. If you master this before moving on, you'll see that everything else in JS and web development is just fancy ways of working with primitive types. Moving on before internalizing primitive types and values is the fastest way to slow down your progress.
* _reference vs. value_: Common mistakes like _side effects_ are the result of mis-understanding how reference works in JS.  Understanding reference vs. value is also key to understanding closure, asynchronous programming, and many other tricky topics in JS.
* _callstack_: Last, but not least, the callstack is so important to how JavaScript works that without a clear understanding of it almost nothing else will ever make sense!  You won't be able to read error messages, understand modules in Node, work with Callbacks, understand closure, the event loop, and much much more. So much of how memory and variables work in JS is determined by the callstack.

To understand how memory is handled in JS (which is the key to effective programming and debugging!) you need to build a solid notional machine that includes all of the topics above.  It may sound daunting, but with the help of __Python Tutor for JavaScript (JS Tutor)__ and some disciplined study habits you'll find it's not so bad after all.

* [JS Tutor](http://pythontutor.com/javascript.html#mode=edit)
* [Intro Video](https://www.youtube.com/watch?v=u0FbLpRDcxU)
* [Intro Article](http://pgbovine.net/python-tutor-live.htm)
* [About PythonTutor](https://www.youtube.com/watch?v=sVtXLdBRfyE)
* [GitHub Repo](https://github.com/pgbovine/OnlinePythonTutor)

[TOP](#javascript)

---

## The Event Loop

Everything in the "core" of JS happens _synchronously_, meaning that each line of code will finish executing before the next one starts.  But part of what makes web development possible is the ability to tell the browser to start one task before another finishes, or the ability to program _asynchronously_.  This is possible because of the _Event Loop_.  Understanding the Event Loop means adding to the notional machine you learned for the core of JS without changing what you've already learned.

The tool you will use to understand the Event Loop is called Loupe, and it comes along with one of the best explanations of the event loop you can find anywhere:

* [Loupe](http://latentflip.com/loupe/)

[TOP](#javascript)

---

## Browser APIs

[Client-Side Web APIs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Introduction) are software implemented in browsers that allow you to do extra cool things with in your web pages.  The core JavaScript engine can't do anything _visible_, it's main responsibility is to manage program memory and execute the next line of your code.  Want to update the DOM, that's not actually JavaScript!  Want to fetch data from a public API, not the JavaScript engine!

These tasks are all handled by other software running in the browser, and each one has a different notional machine.  Their relationship to JavaScript is that there is JS syntax that allows you to write instructions for them inline with your JS code.  This makes it _feel and look_ like the DOM is "part of" JavaScript, but after carefully studying Loupe (the Event Loop) you'll see how it's not. JavaScript uses it's event loop to tell the Browser what you want to do, but then it's up to the Browser and it's APIs!

Some Browser APIs you'll definitely come across are:

* [The Document Object Model (DOM)](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model) - `document.*`
* [CSS Object Model (CSSOM)](https://developer.mozilla.org/en-US/docs/Web/API/CSS) - `CSS.*`
* [Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) - `fetch("url")`
* [Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) - `HTMLCanvasElement.*`
* [Web Storage](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API) - `sessionStorage.*` & `localStorage.*`

Incorporating them into your JS notional machine is not so complicated after all! Remember the big box on the right in Loupe? All of these other services happen there.  To learn more about each one, take a scroll over to `Browsers`.


[TOP](#javascript)

---
---
### <a href="https://hackyourfuture.be" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/63941625-4c7c3d00-ca6c-11e9-9a76-8d5e3632fe70.jpg" width="100" height="100" alt="Hack Your Future: Belgium"></a>
