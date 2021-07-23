# React and Forms

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

## React Forms

1. What is a ‘Controlled Component’?
  a. A controlled component is something that combines the form's states and updating the states all in one.
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
  a. Updating the state as they update their response can be better, I would like like a search bar, to see what your search will give you based on just the bits of information first instead of waiting for the whole response then loading the search results.
3. How do we target what the user is entering if we have an event handler on an input field?
  a. With `this.state` or using a name to categorize which form element is being used at the time.

## Conditional Ternary Operator

1. Why would we use a ternary operator?
  a. a few examples of when using ternary operator would be is: in an object to delcare a yes or no and to make code shorter.
2. Rewrite the following statement using a ternary statement:

&nbsp;&nbsp;&nbsp;&nbsp;`if(x===y){`<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`console.log(true);`<br>
&nbsp;&nbsp;&nbsp;&nbsp;`} else {`<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`console.log(false);`<br>
&nbsp;&nbsp;&nbsp;&nbsp;`}`

`x===y ? console.log(true) : console.log(false)`

You can also have a nested ternary as well, in your else statement you would put another ternary which will test more, make sure you are very specific at first then less specific as you go.

## BookMark/Skim

- [React Bootstrap - Forms](https://react-bootstrap.github.io/components/forms/)
- [React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)

## Things I want to know more about

- When setting a name to a form. using this.setState, when I see `[name]: value` I am not sure why it is in an array. My guess would be to store multiple names, which makes more sense now.

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
