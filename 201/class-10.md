# Class 201 Reading Notes

* [201 Home](https://fadnesscharlie.github.io/reading-notes/201/)

## Debugging

### Global variable vs Function-scope variable

When declaring a variable in a function, it is only used within that function, just locally, while declaring a variable globally, can be used everywhere making it eaiser to use in a whole.

### The Stack

The stack is how a function and code works. As it runs through the program. For a function, as it reads line by line, as it needs to do more things, it puts the current task on hold, places another task on top to form that task, making a stack. The will constantly add more, or decrease as it moves through the code to fulfill its duties.

### 7 types of Javascript Errors

#### Error

Generic Error. The other errors are based on this error.

#### SyntaxError

Most common of this type is a typo error. It can range from not having a closing parentethesis, mis matching quotes, or not having a comma seperating things.

#### RefernceError

Mostly undeclared and indefined variables or functions.

#### TypeError

Incorrect calling of data types, from DOM, to `document.write()`, to methods that dont exsist.

#### RangeError

Number error, when something is outside of the expected range of numbers.

#### URIError

Charcters are not escaped: "`/ ? $ # : ;`".

#### EvalError

When `eval()` function runs, but most of the time, you will get an error from the above from this.

### Debugging Calmness

Writing steps of what you have done tested and tried can help you stay calm when you are in a state of frustration and as you keep going and stay calm you will be able to slowly further your debugging and will be able to find the problem.

### Console Methods

#### Console Logs

Using console logs help a ton. From being able to see how far your code has gone to, seeing what answers are being displayed or calculating from the functions or code. An example of this would be if you want to see how far something is running, or even if the code is making into a certain area in your code. With console logs responding back to you, you can see how far the code has been and whats being returned or if it has entered say some loops or not.

#### Console Info Warn and Error

These three other consoles can give us more context instead of just logging the output or certain message. With multiple `console.log()`'s, it can get crowded, these console logs also show a small icon which can help determine them from other console methods.

`console.info()` is a general inforamtion log.

`console.warn()` Is used for warnings which can be useful when testing.

`console.error()` This will hold errors, this can be very useful when trying to fix a certain error and wanting it to be differnt then the others.

#### Grouping Console Methods

Using `console.group('Group Name')` we can put multiple console methods inside, open and close this box from the console, once we are finished, we have to place `console.groupEnd()` at the end to clarify the end of the group.

#### Console Table/Tabular Data

We can console out a table with the `console.table('table variable here')`. Through the console it will show the table and what we have inside the table from the console.

#### Console Assert(Conditions)

In here, we can write out `console.assert(What we want to test, 'Mesage here')`. In our message, it will display if the condition is false. An example would be `console.assert(isBoolean(true), 'Message if passed argument is not a boolean')`

### Breakpoints

Using Chrome, we open the developer tools, go to sources, highlight an area that we want to stop, now the code will see that as a breakpoint, and will run the code up to that point and stop.

From here we can play the code step by step to find the errors. We will get 4 options:

* a pause/play
* step through - run code by line
* step into - steps into a function as sometimes they bypass them
* step out - steps outside of a function

We can set the breakpoint to have a conditional statement. For that we:

* Right-click on the actual line number in our code the code is written on
* Select Add Conditional breakpoint
* In the box, we then write out condition that we want to it to break to
* The code will stop when the conditional statement is true

#### Debugger Keyword

Here we can actually create a breakpoint in our code as long as the developer tools page is open. We write out: `debugger;`. As we move into the developer tools, we then can add a conditional statement for the breakpoint.

### Handling Exceptions

If we have a concern if our code will run at all, we can try **try**, **catch** and **finally**. Note that each of these will have its own code block to run.

The code that is inside try will run first, then if it can not run or an error pops up, it will continue to catch, finally, or both. Note that if you have a continue, break, or return keyword, it will move towards catch or finally right after.

The catch will have an exception to run this code. It will let the user know if something is wrong at all.

Lastly, it will always move to finally, even if the try block succeeded or failed. It will run even if there is a return keyword inside the code block.

If you want to test this, you can even nest these inside of each other.

### Throwing Errors

We can throw an error before an error pops up if we think there might be one there. This can be helpful for when there is something that is getting placed into a variable or array that is not the right data type. Being able to catch this error before it happens and runs into other code that does not know what to do with the set of data type is does not work with.

We can use try, catch, finally and add in throwing errors to make our code bug proof and catch anything that might be harmful to the rest of our code base.

We use the throwing errors by typing: `throw new Error('message');`. You want to be extremely descriptive and one place to put this is in an if else statement to catch the error.
