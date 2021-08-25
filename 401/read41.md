# React Native

## Review, Research, and Discussion

- Compare and Contrast Redux Toolkit with Redux “Ducks”

  - Ducks is a way to bundle reducers, action types, and actions into the same file.

  - Rather than splitting up related code, it can be packaged into redux modules. Redux Toolkit's goal is to help simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler. Redux Toolkit exports several individual functions that you can use in your application, and adds in dependencies on some other packages that are commonly used with Redux.

- What is the principle advantage of Redux Toolkit

  It helps to solve three major problems with Redux: configuring a Redux store, adding numerous packages to get Redux to things, and removing unnecessary or boilerplate code.

## Document the following Vocabulary Terms

- **redux toolkit slices** is a function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic

- **namespace** is a declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries.

## Preparation Materials

### React Native

  Many different kinds of people use React Native: from advanced iOS developers to React beginners, to people getting started programming for the first time in their career. These docs were written for all learners, no matter their experience level or background.

  To work with React Native, you will need to have an understanding of JavaScript fundamentals. If you’re new to JavaScript or need a refresher, you can dive in or brush up at Mozilla Developer Network.

  With React, you can make components using either classes or functions. Originally, class components were the only components that could have state. But since the introduction of React's Hooks API, you can add state and more to function components.

  React Native is like React, but it uses native components instead of web components as building blocks. So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts, like JSX, components, state, and props. If you already know React, you still need to learn some React-Native-specific stuff, like the native components. This tutorial is aimed at all audiences, whether you have React experience or not.

### Expo

  Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

### Ejecting to ExpoKit

  If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.

  Normally, Expo apps are written in pure JS and never "drop down" to the native iOS or Android layer. This is core to the Expo philosophy and it's part of what makes Expo fast and powerful to use.

  However, there are some cases where advanced developers need native capabilities outside of what Expo offers out-of-the-box. The most common situation is when a project requires a specific Native Module which is not supported by React Native Core or the Expo SDK.

  In this case, Expo allows you to eject your pure-JS project from the Expo iOS/Android clients, providing you with native projects that can be opened and built with Xcode and Android Studio. Those projects will have dependencies on ExpoKit, so everything you already built will keep working as it did before.

  We call this "ejecting" because you still depend on the Expo SDK, but your project no longer lives inside Expo Go. You control the native projects, including configuring and building them yourself.
