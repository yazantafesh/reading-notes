# Component Lifecycle / useEffect() Hook

## Review, Research, and Discussion

1- Why do we not need more .html pages in a multi-page React app?

  In the Multipage apps , we split up our components but a lot of pages are going to be normal HTML pages, and widgets we dump in like an Image gallery that is managed by React, so the entire page is not under React control.

2- If we wanted a component to show up on every page, where would we put it and why?

- **Inside the BrowserRouter , outside a Route**

3- What does routing do with the components that were rendered when a new route is requested

  it goes to the new componetnt and remove the old one

4- What does props.children contain?

  it has the value that we return from the component

5- How do useState() and this.setState() differ?

  setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Document the following Vocabulary Terms

- **State Hook** is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

- **Mounting and Un-Mounting** The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by mounting (adding nodes to the DOM), unmounting (removing them from the DOM), and updating (making changes to nodes already in the DOM).

## Preparation Materials

### Using the Effect Hook

  **What does useEffect do?** By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

  **Why is useEffect called inside a component?** Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

  **Does useEffect run after every render?** Yes! By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.
