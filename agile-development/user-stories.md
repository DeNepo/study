## User Stories


---

## Basic Case Study

Learning to break a whole application into user stories takes experience.  This is easier to learn by practicing with existing applications instead of ones you dream up.

The first step to mastering user stories is to practice asking and answering these questions:

1. __What are the different components on the user interface?__
1. __What interaction does each component enable a user to have with your website?__
1. __How do these stories depend on each other?__
1. __What is a logical order for building these stories?__


Let's see these questions in action with a simple website:
* [tomato timer!](https://tomato-timer.com/)

Here are some possible answers to these questions based on the Tomato Timer (but not the only answers! there are many ways to split a project):

##### What are the different components on the user interface?

* There is a red button that says "stop"
* There is a white button that says "reset"
* There are some numbers
* There is a green button that says "start"

##### What interaction does each component enable a user to have with your website?

* A user can stop the count-down without resetting the time
* A user can stop the count-down and set it back to 25:00
* A user can see how much time is left
* A user can start (or restart!) the count-down

##### How do these stories depend on each other?

* You can't stop a count-down unless it is started
* It is not practical to be able to reset the count-down every time you want to stop it
* You can see how much time is left without being able to start the timer (even if this isn't very useful :)
* There is no point to have a count-down until there is a time to see

##### What is a logical order for building these stories?

1. A user can see how much time is left
1. A user can start (or restart!) the count-down
1. A user can stop the count-down without resetting the time
1. A user can stop the count-down and set it back to 25:00

> [Here's another worked example for further study](https://github.com/elewa-student/User-Centered-Development)
