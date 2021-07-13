# Arrow Functions

## Brief Explanation

- There many uses for arrow functions, and many situations where arrow functions are not the proper tool. We want to look at arrow function as a simple one task that does one things.
- When we use arrow functions, we usually do not need a return if it can be a one-liner. If we need to insert lines of code in the code block, then we need to bring back the return as the code will not know what you want to return in bigger arrow functions.
- With arrow functions we do not need to give it a name, and it will run automatically as it comes up.

### Syntax

Parameter => expression

- If using multple parameters, you will need to insert `(a, b)` parentheses.

#### Multiple statements

`(Parameter1, Parameter2) => {`
&nbsp;&nbsp;`Let i = 1;`
&nbsp;&nbsp;`return i + Parameter1 + Parameter2;`
`}`

## Things that do not work with arrow functions

- You can not use arrow functions as a method
- Call, apply, and bind not suitable for arrow functions

### Call

With using `call()` method, you can call an object that would not normally be in scope. Then using a `this.something`, you can call an object, and that object will use the `this.something` from the object you called as if it were in the scope when it actually is not.

Only works when calling an object or something that has `this`.

### Apply

Apply is very simular to call. The main different is what its used for. `apply()` takes in arguments of array rather then just an object.

### Bind

Bind creates new functions that bind together. Still understanding.
