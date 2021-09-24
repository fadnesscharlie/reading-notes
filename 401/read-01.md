# Node Ecosystem, TDD, CI/CD

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## Review, Research, and Discussion

- Describe (in plain English) what Array.map() does
   a. Array.map() maps through, like a for loop and returns the results of that into an array
- Describe (in plain English) what Array.reduce() does
  - Array.reduce() has a container, then a accumulator. With these first two out of 4 parameters, you can accumulate whatever you want, and the container or "bucket" will hold the results of that. You can also specify what container it is, wether it be an array, number, etc at the end after the arrow function.
- Provide code snippets showing how to use superagent() to fetch data from a URL and log the result
  - With normal Promise .then() syntax
    - `superagent.('API CALL HERE')`
    - `.then()`
  - Again with async / await syntax
    - `async function () {`
      - `await superagent.('API CALL HERE')`
    - `}`
- Explain promises as though you were mentoring a Code 301 level student
  - Promises is like what it says. You are going to do something, and the code expects the promise to resolved or rejected.
- Are all callback functions considered to be Asynchronous? Why or Why Not?
  - It is not because as the first function runs, it has to wait for the call back function to finish running before it can finish. Which means they do not run at the same time.

## Things I want to know more about

- Superagent vs axios.

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
