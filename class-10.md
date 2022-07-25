
# Debugging

## Index

[Home](./README.md)  
[What Went Wrong? Troubleshooting JavaScript](#what-went-wrong-troubleshooting-javascript)  
[The JavaScript Debugger](#the-javascript-debugger)

## [What Went Wrong? Troubleshooting JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_went_wrong)

1. Name some key differences between a Syntax Error and a Logic Error.
   - **Syntax errors:** These are spelling errors in your code that actually cause the program not to run at all, or stop working part way through — you will usually be provided with some error messages too. These are usually okay to fix, as long as you are familiar with the right tools and know what the error messages mean!
   - **Logic errors:** These are errors where the syntax is actually correct but the code is not what you intended it to be, meaning that program runs successfully but gives incorrect results. These are often harder to fix than syntax errors, as there usually isn't an error message to direct you to the source of the error.
2. List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.
   - I've run into miss-spelling errors.  Specifically in HTML I remember wrighting `src` as "scr".  Such a tiny mistake but it took me about 15 mintues to find. I narrowed down what wasn't working and stayed in that ballpark until I verified it was with the link declaration.  I poured over the link until it finally jumped out at me.
   - I've run into order of operations errors.  Where initialization was an issue and the order things were effected how the script executed. I read the console and realized that it wasn't getting the data even though I'd already verified that part was working.  Looked at the order and knew right away.
   - I've run into many syntactical errors and logic errors along my path and will likely run into plenty more.
   - Console log and dev tools console log and dev tools console log and dev tools.
3. How will this topic continue to influence your long term goals?
   - Any tools I can get that help me find problems faster is going to help me manage time beter, complete projects with fewer bugs, and alow me to prototype faster.  Debugging offers a major boost to speed of delivery.

## [The JavaScript Debugger](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools#the_javascript_debugger)

1. How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?
   - The JavaScript debugger is like xray vision into webpages and sheds light onto what makes them tick.
2. Define what a breakpoint is.
   - Breakpoints are places in your code that you want to pause execution and identify the problems that prevent your code from executing properly.
3. What is the call stack?
   - The callstack shows you what code was exectued in order to get to the current line.

[Back to Top](#index)
