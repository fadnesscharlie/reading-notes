# State and Props

- [Home](https://fadnesscharlie.github.io/reading-notes/301/)

## React Lifestyle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
  a.
2. What is the very first thing to happen in the lifecycle of React?
  a.
3. Put the following things in the order that they happen: **componentDidMount**, **render**, **constructor**, **componentWillUnmount**, **React Updates**
  a. Constructor
  b. React Updates
  c. render
  d. componentDidMount
  e. componentWillUnmount
4. What does componentDidMount do?
  a.

## React State Vs Props

1. What types of things can you pass in the props?
  a. Arguments: Like title, name, car type. What you want your component to render.
2. What is the big difference between props and state?
  a. Props are handled outside while state is handled inside the component.
3. When do we re-render our application?
  a. When we make change to the state.
4. What are some examples of things that we could store in state?
  a. Forms are one good example because it will change what is inside the component when the user adds their information.

### What are Props

Props are like arguments you can pass through the component that will update outside of the component. Since props are constantly changing depending on what information we give it, it is not hard coded into our component.

Let us pass dara from aprent to component to child component. One direction. Child cannot change the props.

### What are States

States are handled inside the component. It updates based on what the user or information that is changing. Thing of when we want something to render each time the information is changed, that is what state is for. Think of a form when something enters something, you want something to update so the user can see the changes that have been made.

Lets a component save AND update data FOR ITSELF. Within one component. Can be updated using setState.

## Things I want to know more about

- State and Props

## BookMark/Skim

- [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
- [React Docs - Handling Events](https://reactjs.org/docs/handling-events.html)
- [React Turorials through 'Developer Tools'](https://reactjs.org/tutorial/tutorial.html)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
