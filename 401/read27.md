# useState Hook

## Review, Research, and Discussion

- How does React differ from vanilla JS/HTML/CSS?

  - With React, we write HTML using JavaScript. We rely on the power of JavaScript to generate HTML that depends on some data, rather than enhancing HTML to make it work with that data. Enhancing HTML is what other JavaScript frameworks usually do.
  - Vanilla JS is nothing but plain JS without any external libraries or frameworks. Using this we can build powerful and cross-platform applications.
  - React is a Javascript library used for building user interfaces. It allows us to make complex UIs from isolated pieces of code called "components".
  - In Vanilla JS, the code becomes very difficult to maintain if the application is large because in such cases the UI needs to be updated regularly.

- What is the primary difference between a function component and a class component?

  A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

## Document the following Vocabulary Terms

- **Functional Components** are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword.

- **Children / Child Components**  allow you to pass components as data to other components, just like any other prop you use. The special thing about children is that React provides support through its ReactElement API and JSX. XML children translate perfectly to React children.

## Preparation Materials

### Making Sense of React Hooks

  We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them “separate concerns.”

  These cases are very common and include animations, form handling, connecting to external data sources, and many other things we want to do from our components. When we try to solve these use cases with components alone, we usually end up with:

- Huge components that are hard to refactor and test.
- Duplicated logic between different components and lifecycle methods.
- Complex patterns like render props and higher-order components.

### Using the State Hook

  **What is a Hook?** A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We’ll learn other Hooks later.

  **When would I use a Hook?** If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. We’re going to do that right now!

### Hooks at a Glance

  Here, **useState** is a Hook (we’ll talk about what this means in a moment). We call it inside a function component to add some local state to it. React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else. It’s similar to this.setState in a class, except it doesn’t merge the old and new state together. (We’ll show an example comparing useState to this.state in Using the State Hook.)

  The only argument to **useState** is the initial state. In the example above, it is 0 because our counter starts from zero. Note that unlike this.state, the state here doesn’t have to be an object — although it can be if you want. The initial state argument is only used during the first render.
