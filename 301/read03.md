# Lists and Keys

- What does .map() return?

We return a `<li>` element for each item. Finally, we assign the resulting array of elements to listItems.

- If I want to loop through an array and display each value in JSX, how do I do that in React?

```
function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);
```

- Each list item needs a unique **KEY**.

- What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

# The Spread Operator

- What is the spread operator?

In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

- List 4 things that the spread operator can do.

Copying an array,
Concatenating or combining arrays,
Using Math functions,
Using an array as arguments.

- Give an example of using the spread operator to combine two arrays.

```
[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
```

- Give an example of using the spread operator to add a new item to an array.
```
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
```

- Give an example of using the spread operator to combine two objects into one.

```
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```

# How to Pass Functions Between Components

- In the video, what is the first step that the developer does to pass functions between components?

Create a function where the state is.

- In your own words, what does the ```increment``` function do?

Increase the value of a variable by one each time the button is pressed.

- How can you pass a method from a parent component into a child component?

Using state.

- How does the child component invoke a method that was passed to it from a parent component?

I dont know.

## Things I want to know more about

***Nothing in this lecture***
