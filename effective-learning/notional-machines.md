# Notional Machines

what does it mean to learn how a programming language and runtime works? It means to learn a "notional machine" - a series of visualizations, diagrams, refactoring techniques, and vocabulary that are accurate but manageable; correct enough that you can use them to predict program state, debug your projects, and accurately translate between diagrams & code, but not so precise that you get lost in how compilers and interpreters work.

A very important feature of the notional machine is that it does not attempt to describe the programming language as like something else. One easy danger when learning to program is to use analogies to make it all feel more familiar. This is especially dangerous because programming languages & computers are not like other things you know! Any intuitions built off of previous experience will be misleading and can make learning more difficult for in the long run.

Using a common set of visualization tools, and correct vocabulary from day 1 is super important. Building up a correct understanding from nothing is only realistic when you, your peers and your coaches all discuss the same visuals with the same vocabulary.

These diagrams and visualizations will expand and become more detailed as you learn more about your programming language and environment. Take JavaScript for example:

1. The first notional machine you will learn includes only what takes place on the _callstack_ - so variables, functions, types/operators, control flow, data structures, and the console.
1. Next is _the event loop_.  To understand asynchronous JavaScript, nothing you learned about the CallStack changes.  But you will need to add a _heap_ and a _queue_.
1. Finally is Node.js.  Node.js also has a callstack, a heap, and a queue.  But it also has modules, file system access, and can open a port on the internet.

Your brain will construct an understanding of how JS works whether or not you intentionally guide it, it's what brains do.  As great as this sounds it is really very dangerous.  JavaScript is a complicated language and it is very easy to come up with explanations that work for simple programs but are not accurate.  You won't notice at first, but as soon as you try to move on you will find it nearly impossible to understand what's going on.  Unlearning and relearning how JavaScript executes is very difficult and will take much more time than learning it right from the beginning.


### Index

* [Git](#git)
* [CLI and File System](#cli-and-file-system)
* [JavaScript](#javascript)
  * [Callstack](#callstack)
  * [Event Loop](#event-loop)
* [The Internet](#the-internet)
* [Browsers](#browsers)
  * [The DOM](#the-dom)
  * [Events](#events)
  * [Network Requests](#network-requests)
* [Node.js](#node-js)
* [Fullstack Web Apps](#fullstack-web-apps)
* [Relational Data Bases](#relational-data-bases)

---

per section
* why this topic & how it fits in
* tools for visualizing and exploring

---

## JavaScript


The best way to learn JavaScript is from the [inside-out](https://github.com/janke-learning/js-in-order), focusing first on how your code is interpreted and how memory is managed then later learning to apply this to practical problems. Unfortunately most introductions to JS cover the language from the outside in, focusing on the most interesting or intuitive features first and directly apply them to programming challenges.  This approach will feel satisfying at first but will quickly slow your progress as you have difficulty separating JS behavior from strategy bugs.


Instead, take a look through [JavaScript in order](https://github.com/janke-learning/js-in-order).  It's a guide to JavaScript that builds your understanding of the JS Notional Machine from the inside out focusing first on how the JS engine interprets your commands, building from the simplest concepts of program execution and errors all the way up to more complicated features like contextual free variables.  After mastering JavaScript's inner workings you'll find [problem solving strategies](https://github.com/colevandersWands/top/#strategy) are much more approachable.

[JavaScript in order](https://github.com/janke-learning/js-in-order) is not just a better explanation of JS.  It's an entirely different approach encouraging you to learn JS by visualizing and studying the behavior of carefully designed snippets, building your own correct understanding instead of learning our best explanation.



### CallStack

__about PythonTutor__

* [Intro Video](https://www.youtube.com/watch?v=u0FbLpRDcxU)
* [Intro Article](http://pgbovine.net/python-tutor-live.htm)
* [About PythonTutor](https://www.youtube.com/watch?v=sVtXLdBRfyE)
* [GitHub Repo](https://github.com/pgbovine/OnlinePythonTutor)

---

## Node.js

The most important thing to understand about Node.js is that it's basically just JavaScript with superpowers - reading & writing to the file system, opening a port on the internet, and working with modules.  The notional machines you've learned for the JS Callstack and Eventloop are still relevant, but with a couple key changes:
* (needs help)
* user events are triggered via a live server instead of the DOM
* access to the computer direclty instad of just the browser (thus file systems, databases, and the like)
* source code can be interpreted and loaded dynamically from any file at any time.  projects can be built in modules with no need for building, bunding and transpiling

Learning a notional machine for Node.js is about building on top of those, not starting from scratch.

> find a good diagram to include

---

* [Understanding the Notional Machine](https://www.gvu.gatech.edu/research/projects/understanding-notional-machine)
* [Isolate the Notional Machine](https://github.com/blocks-to-text/isolate-the-notional-machine)
* [defining what it means to understand computing](https://computinged.wordpress.com/2012/05/24/defining-what-does-it-mean-to-understand-computing/)
* [notional machines and misconceptions in CS](https://computinged.wordpress.com/2016/03/07/notional-machines-and-misconceptions-in-cs-developing-a-research-agenda-at-dagstuhl/)
* [a deeper look at notional machines](https://www.researchgate.net/profile/Juha_Sorva/publication/259998496_Notional_Machines_and_Introductory_Programming_Education/links/5586b8f008aef58c039f90f5/Notional-Machines-and-Introductory-Programming-Education.pdf)
