# Express REST API

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware
   - Being able to see the request before it goes through to make sure it will not break your code.
   - Make sure no foriegn answers come in.
   - Log all of the request.
2. True or false: The route handler is middleware?
   - True
3. In what ways can a middleware function end the process and send data to the browser?
   - with the `next()` method
4. At what point in the request lifecycle can you “inject” middleware?
   - Whenever you are getting a request.
5. What can cause express to error with “Request headers sent twice, cannot start a second response”

## Define

- Middleware
  - A function that will receive the request and response
- Request Object
  - Request a query of things including strings, parameters, body, HTTP headers, etc
- Response Object
  - The Object it sends when it gets a HTTP request
- Application Middleware
  - Code that lies in between the oporating system and the application.
- Routing Middleware
  - Code that runs when routes are run
- Test Driven Development
  - Creating test cases before the software is fully developed vs the usual instance of creating tests after the software is fully developed.
- Behavorial Testing
  - The same as testing but more specific to behaviors of how things are working.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
   - Express
   - Routing
   - Class
2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
   - Possible deep dive into Express
   - More on middleware
   - More on tests and how it can run functions into our code
3. What are you most excited about trying to implement or see how it works?
   - Middleware and tests are something that I believe is very powerful and probably something that companies use a lot.

## Resources

- [Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
- [Using Express Routing](https://expressjs.com/en/guide/routing.html)
- [Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

## Things I want to know more about

- Middleware and testing

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
