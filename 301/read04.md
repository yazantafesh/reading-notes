# Forms

- What is a ‘Controlled Component’?

React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React

- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

update the state with their responses as soon as they enter them; you can pass the value to other UI elements, or reset it from other event handlers.

- How do we target what the user is entering if we have an event handler on an input field?

by adding onChange to the input element and assigning a function, the function will runs on every keystroke to update the React state, and the value will be in event.target.value

# The Conditional (Ternary) Operator Explained

- Why would we use a ternary operator?

to have less lines of code or make the code shorter.

- Rewrite the following statement using a ternary statement:

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

```

x === y? console.log(true) : console.log(false);

```

## Things I want to know more about

***I want to know more about forms in react***
