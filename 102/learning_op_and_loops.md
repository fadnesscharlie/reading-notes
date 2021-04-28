# Learning Operators and Loops

[Home](https://fadnesscharlie.github.io/Reading-notes1000/) 

## Logical Operators

### Logical "And"

`&&`  
Returns true if both are true, returns false if both are not true

### Logical "Or"

`||`  
Tests at least one condition

### Logical "Not"

`!`  
Inverts the boolean. Makes True become False, and False become True

## Comparison Operators

`==` is equal to: `'hello' == 'hello'`  
You want it to be the same

`!=` is not equal to: `'hello' != 'goodbye'`  
This will come back True

`===` is strict equal to: `'4' === 4`  
This comes back false. The first 4 is a string and not a number

`!==` is strict not equal to: `'4' !== 4`  
This comes back True. It is not strictly equal

We also have `<` less then, `>` greater than, `<=` less than or equal to, `>=` greater than or equal to


## Loops

### For Loops

Example:  
`for (let i = 0; i < 10; i++) {`  
&nbsp;&nbsp;&nbsp;&nbsp;`document.write(i);`  
`}`  

Initialization: `let i = 0`

Condition: `i < 10;`

Update: `i++`

This example of a for loop. What is happening is that i is being declared as 0. Since 1 < 10, it is false and then writes the document and then `i++` adds 1 to 0,and now `i` is declared as 1.  
This process runs over and over through until  i is 11, then it becomes false, and exits out of the loop.

### While Loops

While loops are very simular to for loops. One of the main differences is that with a for loop, its more towards setting to something. A while takes in more of a boolean, which is true or false. If the while loop is true, it will keep going __UNITL__ it gets a false. Then it will break out of the loop.
