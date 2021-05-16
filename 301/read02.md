# React Lifecycle

1. According to the diagram, rendering happens before and after componentDidMount.
2. The first thing that happens is Mounting and it is Constructor specifically.
3. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.
4. This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

# React State Vs Props

1. It can be many things like the initial value for a counter or any different attributes for various tags like img src and alt or title.
2. You pass props into a component while they are handled outside of it, but states are already handled inside a component and can be updated inside the component.
3. When the user has done some changes or activated an event.
4. State is mainly used when when we need to re-render the page when the user commits a change like in a form for example, as the user fills out data and submits, we will need to re-render the page, or maybe in some sort of counter.

## Things I want to know more about

***Nothing in this lecture***
