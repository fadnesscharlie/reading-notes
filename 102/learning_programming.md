# Learning JavaScript Programming

[Home](https://fadnesscharlie.github.io/reading-notes/102)

## Goals of a Script

Think of a wireframe for scructure of task/flow chart

You wand to write out what is happening. Think of it as, if i do this, this happens or does not happen. Writing this out helps a lot. It shows step by step what the script is doing.

One thing we have to understand is that the computer only does now add the information around it. It reads what it is told as if it does not know anything besides what is written in the code.

Having a good understanding of logic chains is a very good skill. When we have an idea of what happens next in the chain, we can know where to code for the computer to understand where to go next.

## Operations

### **Assignment Operators**

Assign a value to a variable

`color = 'red';`

The value of color is now red

### **Comparison Operators**

Compare two values and return true or false

`buy = 3 > 6;`

the value of buy is false

### **Artihmetic Operators**

Perform basic math

`area = 2 * 3;`

The value of area is now 6

### **Logical Operators**

Combine expressions and return true or false

`buy = (6 > 3) && (2 < 4);`

The value of buy is now true

### **String Operators**

Combine two strings

`greeting = 'Hi ' + 'Jasmine';`

The value of greeting is now Hi Jasmine

## Functions

The format of a function is below. We look at the function, what we want to call the function `sayHello()`, we can name this whatever we want. The main goal is to make sure the name relates to the function for better user ability. If we called it `pumpkingPieRecipe()` when we called it later, we would think it would relate to pumpkings, and not just writing hello for us.

`function sayHello() {`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello!');`  
`}`

`function` is the function keyword.

`sayHello()` is our function name. We can name this whatever we want.

`{`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello!');`  
`}`

This is our code block. Our list of commands of what we want the function to do for us.

### Parameters

`function sayHello(parameter) {`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write('Hello!');`  
`}`

In functions, we can state a parameter, and when we call the function, we will need to add a parameter when we call it.

`sayHello(addParameterHere)`

### Calling the function

You can call the function as many times as you want

`sayHello();`

Group set of statements or instructors together to perform a specific task

Offer a way to store the steps

### Return keyword

In a function, we use the `return` keyword to return what the function has done. When the function does something for us, we need it to give us what it has done. That is what the `return` keyword does. If we give it parameters, we will get the parameters from the return key.

## Example Function

`function getArea(width, height) {`

&nbsp;&nbsp;&nbsp;&nbsp;`return width * height;`

`}`

When calling the function:
`getArea(3,4);`

The `3` is the width and the `4` is the height
This is called perameters
You can use arguemtns as variables as well.

In this case it would be `wallWidth = 3;` and `wallHeight = 4;`
This is called arugments

`getArea(wallWidth, wallHeight);`
