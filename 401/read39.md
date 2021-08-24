# Redux - Additional Topics

## Review, Research, and Discussion

- What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

  The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

- When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

  You export the actual action from the reducer.

## Document the following Vocabulary Terms

- **middleware** is a snippet of code that provides a third-party extension point between dispatching an action and the moment it reaches the reducers.

- **thunk** is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. One of the main use cases for this middleware is for handling actions that might not be synchronous, for example, using axios to send a GET request.

## Preparation Materials

### Redux Toolkit (RTK)

  Redux Toolkit is our official, opinionated, batteries-included toolset for efficient Redux development. It is intended to be the standard way to write Redux logic, and we strongly recommend that you use it.

  It includes several utility functions that simplify the most common Redux use cases, including store setup, defining reducers, immutable update logic, and even creating entire "slices" of state at once without writing any action creators or action types by hand. It also includes the most widely used Redux addons, like Redux Thunk for async logic and Reselect for writing selector functions, so that you can use them right away.

  The Redux core library is deliberately unopinionated. It lets you decide how you want to handle everything, like store setup, what your state contains, and how you want to build your reducers.

  This is good in some cases, because it gives you flexibility, but that flexibility isn't always needed. Sometimes we just want the simplest possible way to get started, with some good default behavior out of the box. Or, maybe you're writing a larger application and finding yourself writing some similar code, and you'd like to cut down on how much of that code you have to write by hand.

  **Redux Toolkit** was originally created to help address three common concerns about Redux:

- "Configuring a Redux store is too complicated"

- "I have to add a lot of packages to get Redux to do anything useful"

- "Redux requires too much boilerplate code"

  Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience. It can be added at the start of a new project, or used as part of an incremental migration in an existing project.

  **Redux Toolkit includes:**

- **configureStore():** wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

- **createReducer():** that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos.completed = true.

- **createAction():** generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

- **createSlice():** accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

- **createAsyncThunk:** accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise

- **createEntityAdapter:** generates a set of reusable reducers and selectors to manage normalized data in the store
The createSelector utility from the Reselect library, re-exported for ease of use.
