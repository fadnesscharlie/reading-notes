# Putting it all together

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

## Thinking in React

1. How would you break a mock into a component heirarchy?
   1. By breaking dwon each section that could potentially have their own styling, render changing, or feels seperate from the others.
2. What is the **single responsibility principle** and how does it apply to components?
   1. Simular top functions, it should do just one thing.
3. What does it mean to build a ‘static’ version of your application?
   1. Building a static version of our App means you will want props or just components. Not to add state as it takes in information, and re-renders the page which we do not need for a static site.
   2. Building something that takes a lot of typing and less thinking.
4. Once you have a static application, what do you need to add?
   1. Props that take information down to components.
5. What are the three questions you can ask to determine if something is state?
   1. Does it change over time.
   2. We use the value from the user.
   3. Sites that have interactivity
6. How can you identify where state needs to live?
   1. A hierachy of where it exsist, or when you need the data to change into that component.

## Resources

- [React Docs - thinking in React](https://reactjs.org/docs/thinking-in-react.html)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
