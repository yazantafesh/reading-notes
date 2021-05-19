# Thinking in React

1. How would you break a mock into a component heirarchy?

    - **FilterableProductTable** : contains the entirety of the example
    - **SearchBar** : receives all user input
    - **ProductTable** : displays and filters the data collection based on user input
    - **ProductCategoryRow** : displays a heading for each category
    - **ProductRow** : displays a row for each product

2. What is the single responsibility principle and how does it apply to components?

    ***component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.***

3. What does it mean to build a ‘static’ version of your application?

    To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

4. Once you have a static application, what do you need to add?

    To build your app correctly, you first need to think of the minimal set of mutable state that your app needs. The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand. For example, if you’re building a TODO list, keep an array of the TODO items around; don’t keep a separate state variable for the count. Instead, when you want to render the TODO count, take the length of the TODO items array.

5. What are the three questions you can ask to determine if something is state?

    - Is it passed in from a parent via props? If so, it probably isn’t state.

    - Does it remain unchanged over time? If so, it probably isn’t state.

    - Can you compute it based on any other state or props in your component? If so, it isn’t state.

6. How can you identify where state needs to live?

    **For each piece of state in your application:**

    - Identify every component that renders something based on that state.

    - Find a common owner component (a single component above all the components that need the state in the hierarchy).

    - Either the common owner or another component higher up in the hierarchy should own the state.

    - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Things I want to know more about

new methods in react.
