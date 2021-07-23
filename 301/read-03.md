# Passing Functions as Props

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

## React Docs - lists and keys

- What does .map() return?
  - It maps through the array, then returns the action of the map through a function or arrow function back into an assigned array.
- If I want to loop through an array and display each value in JSX, how do I do that in React?
  - Ways you can implement this:
    - Is with curly braces and a possible inline.
    - Using curly braces as the return variable to see it as an expression.
- Each list item needs a unique **Key**.
- What is the purpose of a key?
  - Helps React identify which items have changed, added, or moved.

## The Spread Operator

- What is the spread operator?
  - The spread operator spreads the array into seperate arguments.
- List 4 things that the spread operator can do.
  1. Concatenating or combining arrays
  2. Use an array as arguments
  3. Adding to state in React
  4. Combining objects
- Give an example of using the spread operator to combine two arrays.
  - An example would be, if you want to group together exsisting arrays without having to push each index into through a loop. Syxtax `let newVariable = [...exsistingArray];`
- Give an example of using the spread operator to add a new item to an array.
  - An example of adding new items to an array could be placement, without having to make a new function to them push or add them to the array then return the array or new array, you can just `let addingToArray = [...exsistingArray, 'addMe', 5, true];` This will add `'addMe', 5, true` to the end of the array in that order.
- Give an example of using the spread operator to combine two objects into one.
  - Same as the example from above, when wanting to add a new objects together, instead of making an loop which would declare the key and values then push them into an array, you can just: `let newObject = [... exsitingObject1, ... exsistingObject2, newObject: 'newObjectValue'];`
- Another example using Math function would be if the Math function requires a list of arguments, and not arrays. Using the spread operator, you can turn an array into a list of arguments.

## How to Pass Functions Between Components

- In the video, what is the first step that the developer does to pass functions between components?
  - He passed the function down into the person object first before declaring it into another level of the app.
- In your own words, what does the increment function do?
  - The increment function increases the number by one each time it is clicked. It updates through the eventListener by targeting the value of the key:name and returning that value.
- How can you pass a method from a parent component into a child component?
  - You have to call the function through `this.props.methodName()`
- How does the child component invoke a method that was passed to it from a parent component?
  - Using an event listener. In the video, it would be a button.

## Things I want to know more about

- Functions and useage of spread operators

## BookMark/Skim

- [React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
