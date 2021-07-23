# Introduction to React and Components

## Component Based Architecture

- What is a component?
  A block of code that you can use and reuse. Examples of this would be header, main, and footer. Its purpose is to be able to create small functionalities and be able to implement these where ever needed or even replaced with newer components that will not break the code.

- What are the charactistics of a component?
  - **Reusability** − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.
  - **Replaceable** − Components may be freely substituted with other similar components.
  - **Not context specific** − Components are designed to operate in different environments and contexts.
  - **Extensible** − A component can be extended from existing components to provide new behavior.
  - **Encapsulated** − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
  - **Independent** − Components are designed to have minimal dependencies on other components.
- What are the advantages of using component based architecture?
  - **Ease of deployment** − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
  - **Reduced cost** − The use of third-party components allows you to spread the cost of development and maintenance.
  - **Ease of development** − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
  - **Reusable** − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
  - **Modification of technical complexity** − A component modifies the complexity through the use of a component container and its services.
  - **Reliability** − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
  - **System maintenance and evolution** − Easy to change and update the implementation without affecting the rest of the system.
  - **Independent** − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

## What is Props and How to Use it in React

- Props?
  - Probs is passed down data and information from the parent to the child. Simular to arugments in a function.
- What is props short for?
  - Props is short for properties
- How are props used in React?
  - Props are used simular to arugments. They used a key value pair to get the information through dot notation. THe key value pairs look simular to how an image tag as `src=""` and `alt=""`. Props look like the same using the key value pairs. Then we access those with `prop.src` or `props.alt`.
- What is the flow of props?
  - It goes only **one direction**
  - The child **cannot** change props

## Referneces

- [Component Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.html)

## BookMark/Skim

- [React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
- [React Docs - Hello World](https://reactjs.org/docs/hello-world.html)
- [React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
- [React Docs - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)
- [React Docs - Components and Props](https://reactjs.org/docs/components-and-props.html)

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
