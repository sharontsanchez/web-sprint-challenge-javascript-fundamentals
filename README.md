# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 
.map 
The map() method creates a new array by calling the callback function provided as an argument on every element in the input array. 
The map() method will take every returned value from the callback function and creates a new array using those values.
use case: we have an array containing the birth year of different persons and we want to create an array that contains their ages. We can use 
map() to return a new array that doesnt manipulate the original array by converting data into what we need. 

.reduce
The reduce method executes the callback function on each member of the calling array which results in a single output value. 
The reduce method accepts two parameters: 1) The reducer function (callback), 2) and an optional initialValue. 
The reducer function (callback) accepts four parameters: accumulator, currentValue, currentIndex, sourceArray.
If an initialValue is provided, then the accumulator will be equal to the initialValue and the currentValue will be equal to the first element in the array.
If no initialValue is provided, then the accumulator will be equal to the first element in the array and the currentValue will be equal to the second element in the array.
use case: when we need to sum an array of numbers, we can use .reduce(acc,current value) to return acc + current value. This wont manipulate the original array and will return a value. 

.filter 
The filter() method creates a new array with all elements that pass the test provided by the callback function. The callback function passed to the filter() method accepts 3 arguments: element, index, and array.
use case: we have an array which contains objects with name and age properties. We want to create an array that contains only the persons with full age (age greater than or equal to 18). we can use filter() to filter out results into a new array without manipulatibg the original array.

2. Explain the difference between a callback and a higher order function.

A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.
Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them. In simple words, A Higher-Order function is a function that receives a function as an argument or returns the function as output.

3. Explain what a closure is.
    
A closure is when an inner function reaches out of its scope to grab a variable defined in an outer function. Closures give us the ability to put functions together. Its the ability to access functions from a parent level scope in child level scope even after the parent function has been terminated. It is code that has been identified elsewhere that we can use later. 

4. Describe the four principles of the 'this' keyword.

The 4 Principles of 'this'
1.Window Binding: Window binding is not something we aim to use. It's what happens when we do not give context for the 'this' keyword. If we don't tell JavaScript what 'this' is it will return the window to us, the global object in node or undefined in strict mode.
2.Implicit Binding: Implicit binding is probably the most common principle of 'this', it apply to objects with methods and it says when the function is invoked, look to the left of the dot. A good way to remember implicit binding is that it's IMPLIED that whatever is to the left of the dot when the function is invoked that's what 'this' will refer to.
3.Explicit Binding: With explicit binding we explicitly pass in as an argument what we want 'this' to refer to. We do that using .call(), .apply(), or .bind(). There are some differences with how we use these.
.call() - will immediately invoke the function, with .call you pass in the arguments 1 by 1
.apply() - will immediately invoke the function, with .apply you would pass in the arguments as an array
.bind() - you will pass in your arguments 1 by 1 but it does not immediately invoke the function, instead it returns a brand new function that can be invoked later.
4.New Binding: New binding is used with constructor functions. It says that when a function is invoked as a constructor function using the 'new' keyword 'this' points to the newly created object. A constructor function constructs other objects. Some things you may notice about a constructor function is that it has a capitalized function name, there is an assignment of the 'this' keyword and it may be missing a return statement.

5. Why do we need super() in an extended class?

Extends tells the child who its parent is and also tells super what to super to. Super replaces parent.call. Super and extends do what .call and object.create did (they inherit methods and attributes from the parent). The super() keyword is used in a child class to call its parent's constructor. It is used to access and call functions on an object's parent.



You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade. 

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://www.notion.so/lambdaschool/Submitting-an-assignment-via-Code-Grade-A-Step-by-Step-Walkthrough-07bd65f5f8364e709ecb5064735ce374)

