---
layout: post
title: Web Development Observations, Recommendations and Other Tidbits
---

Here is my list of recent observations, recommendations and other tidbits based on my web development work at a large retailer over the past several months.

 * Do not use an abstraction layer unless you understand what it is abstracting away. 
 * [TypeScript](https://www.typescriptlang.org) does not add static typing to JavaScript. It is syntactic sugar that when coupled with IDE support, offers type checking when writing and "transpiling" code. By the way, that type support is optional. Before using it, refer to my first item above.
 * Expanding upon the first item, being an effective vanilla JavaScript developer should be a prerequisite for using any JavaScript library or framework. 
 * Expanding upon the first two items, **JavaScript is untyped**. No abstraction layer/library/framework can change this. At best, they can only attempt to abstract it away at code development/transpile time.
 * Frontend web development projects should not have hundreds, much less thousands of CSS/SCSS files. If a project does, it is time to refactor.
 * JavaScript is single threaded. So, all it takes is for one little undefined error to halt execution. To help mitigate this: at a minimum, all functions that are callable outside of their enclosing scope should protect themselves by checking the validity of any arguments passed in. Failing to do so opens the possibility however remote for invalid arguments to get passed in, resulting in the dreaded undefined error. Tests should be added to cover the proper handling of invalid arguments.
 * Creating a working development environment from scratch for a project on a supported development system should always "just work". If the process for doing this does not work, it should be treated as a high priority issue and fixed as soon as possible because inevitably, this will block developers from being able to do their job.
 * Except for maybe the simplest of cases, self-documenting code is not an adequate substitute for code comments. Therefore, all code *at a minimum* should have [javadoc style comments](https://en.wikipedia.org/wiki/Javadoc) that describe what the files, classes and functions do. Ideally, all moderately complex code blocks should be commented as well.
 * Using the space character is the best way to ensure code indent consistency and uniformity.
 * Use tools like [JSCS](http://jscs.info) and [JSHint](http://jshint.com) to check the code during every build to enforce coding standards. Attempting to do this during code reviews is inefficient and will likely miss things.
 * Use [Git Hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) to help enforce coding standards and to ensure all commits contain the necessary comment.  
 * When implementing a story or fixing a bug, favor doing the minimum required to meet the story requirements or to fix the bug. If opportunities to refactor or improve the code present themselves that are outside the scope of the story or bug, open a new story to complete that refactoring work and add it to the backlog.
 * Take the time to test markup and style changes in multiple browsers. Always include Microsoft Edge and Microsoft Internet Explorer if those browsers are supported because unfortunately, there are still significant rendering differences that occur in these browsers. [Modern.ie](http://modern.ie) is a great resource to facilitate Microsoft browser testing, especially if your primary development environment is not Windows. If the site is responsive, include mobile browser testing. Mobile device simulators/emulators can be used to do mobile browser testing.
 
 

