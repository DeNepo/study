# Notional Machines

what does it mean to learn a programming language and runtime environment? 

One workable answer is `to learn a "notional machine"`.

A What? Just a fancy way of saying that you are comfortable using words and diagrams to explain what is happening inside of the computer at any point in your program's execution. A series of 

* visualizations
* diagrams
* refactoring techniques
* vocabulary 

That are accurate but manageable; correct enough that you can use them to predict program state, debug your projects, and accurately translate between diagrams & code. But not so precise that you get lost in low-level implementation.

A very important feature of a notional machine is that it doesn't use analogies. It builds new intuitions based on how computers work, instead of building on old intuitions you already have about how the rest of the world works. 

An easy danger when learning to program is to use analogies for familiarity. This is especially dangerous because programming languages & computers are not like other things you know! Any intuitions built off of previous experience will be misleading and can make learning more difficult in the long run.

Using a common set of visualization tools, and correct vocabulary from day 1 is super important. Building up a correct understanding from nothing is only realistic when you, your peers and your coaches all discuss the same visuals with the same vocabulary.

These diagrams and visualizations will expand and become more detailed as you learn more about your programming language and environment. Take JavaScript for example:

1. The first JS notional machine you will learn includes only what takes place on the _callstack_ - variables, functions, types/operators, control flow, data structures, to name a few.
1. Next is _the event loop_.  To understand asynchronous JavaScript, nothing you learned about the CallStack changes.  But you will need to add a _heap_ and a _queue_ to your JavaScript notional machine.
1. Browsers are a ubiquitous runtime environment for JavaScript.  Besides having a JS callstack & event loop, browsers have other components to incorporate into their notional machine including the DOM, local storage, and networking functionalities.
1. Another is Node.js.  Node.js also has a callstack, a heap, and a queue.  But it also has modules, file system access, and can open a port on the internet.  These _add to_ but do not change what you have already learned about JavaScript works.

Your brain will construct an understanding of how JS and these other programming environments work whether or not you intentionally guide it, it's what brains do.  As great as this sounds it is actually quite risky.  Web Development is very complicated and it is very easy to come up with explanations that work for simple projects but are not accurate.  You won't notice at first, but as soon as you try to move on you will find it nearly impossible to understand what's going on, and you will be unable to effectively plan or debug your projects.  Unlearning and relearning how environments like the Browser or Node operate is difficult and will take much more time than learning correctly from the beginning.

---

## References

* [Understanding the Notional Machine](https://www.gvu.gatech.edu/research/projects/understanding-notional-machine)
* [Isolate the Notional Machine](https://github.com/blocks-to-text/isolate-the-notional-machine)
* [defining what it means to understand computing](https://computinged.wordpress.com/2012/05/24/defining-what-does-it-mean-to-understand-computing/)
* [notional machines and misconceptions in CS](https://computinged.wordpress.com/2016/03/07/notional-machines-and-misconceptions-in-cs-developing-a-research-agenda-at-dagstuhl/)
* [a deeper look at notional machines](https://www.researchgate.net/profile/Juha_Sorva/publication/259998496_Notional_Machines_and_Introductory_Programming_Education/links/5586b8f008aef58c039f90f5/Notional-Machines-and-Introductory-Programming-Education.pdf)


---
---
### <a href="https://hackyourfuture.be" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/63941625-4c7c3d00-ca6c-11e9-9a76-8d5e3632fe70.jpg" width="100" height="100" alt="Hack Your Future: Belgium"></a>
