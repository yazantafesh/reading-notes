# Context API

## Review, Research, and Discussion

- Describe use cases useState() vs useReducer()

  useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

- Why do custom hooks need the use prefix?

  Custom hooks are normal JS functions, named with the prefix ‘use’, that can use hooks inside of it and contain a common stateful logic to be reused in other components.

- What do custom hooks usually do?

  Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

- Using any list of custom hooks, research and name one that you think will be useful in your applications

  useScript React hook to dynamically load an external script and know when its loaded

- Describe how a hook that fetches API data might work

  Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = “...”})
  Links to an external site.

## Document the following Vocabulary Terms

- **reducer** is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

## Preparation Materials

### Context

  Context provides a way to pass data through the component tree without having to pass props down manually at every level.

  In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

  Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

  Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

  If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

### Hooks and context example

  After performing an audit on how we communicate with our users, we landed with a simple system of three classes of communication, and snackbars fit perfectly on the ‘low priority’ end of that spectrum. They are small notifications that show up on the screen when a user performs an action. They are not intrusive at all and appear for just a brief moment.

  From an engineering standpoint, our snackbar system must easy to use and generally be very lightweight. We want to be able to place one on the screen with just a couple of lines of code. Anything more and it’s overkill.

  This means forget render props and higher order components. We don’t want to deal with a messy React tree and wrappers. We don’t want action creators, reducers*, or any of that stuff.
