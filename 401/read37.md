# Redux - Combined Reducers

## Review, Research, and Discussion

- Why choose Redux instead of the Context API for global state?

  Redux is the industry standard for managing the state of large applications. It is more optimized for larger projects because the context API re-renders more often.

- What is the purpose of a reducer?

  A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application’s state changes in a single store so that they behave consistently.

- What does an action contain?

  An action contains a action type and whatever payload you want it to have.

- Why do we need to copy the state in a reducer?

  The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state.

## Document the following Vocabulary Terms

- **Immutable State** is a state that cannot be modified, reducers must make copies of existing state to make updates.

- **Time travel in redux** is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.

- **Action Creator** simply return an action object and pass the argument value if necessary(The only way to change the state is to dispatch an action, an object that describes what happened.)

- **Reducer** is a pure function that take the previous state and an action, and return the next state. Like any other functions, you can split reducers into smaller functions to help do the work, or write reusable reducers for common tasks.

- **Dispatch** is the act of sending something somewhere. In computer science, this term is used to indicate the same concept in different contexts, like to dispatch a call to a function, dispatch an event to a listener, dispatch an interrupt to a handler or dispatch a process to the CPU.

## Preparation Materials

### Multiple Reducers

  Reducers are a great concept in Redux, because they allow your react application to have specific pieces of data that all update synchronously.  All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders.
  
  The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

  There are two ways to define the initial shape and contents of your store's state. First, the createStore function can take preloadedState as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser's localStorage. The other way is for the root reducer to return the initial state value when the state argument is undefined. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using combineReducers.

  combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object. The correlation between these names is not always apparent, especially when using ES6 features such as default module exports and object literal shorthands.
  