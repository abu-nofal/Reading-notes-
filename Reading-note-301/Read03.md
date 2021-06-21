## React Docs - lists and keys 

1. What does .map() return?
return the new array 


2. If I want to loop through an array and 
display each value in JSX, how do I do that in React?

- You can build collections of elements and include them in JSX using curly braces {}

- and render it to the DOM: 

>const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  `<li>{number}</li>`
);

>ReactDOM.render(`<ul>{listItems}</ul>`,
  document.getElementById('root')
);



3. Each list item needs a unique ____.

A **“key”** is a special string attribute you need to include when creating lists of elements 



4. What is the purpose of a key?



## The Spread Operator 

1. What is the spread operator?

- is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

- In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.


2. List 4 things that the spread operator can do.


- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array



3. Give an example of using the spread operator to combine two arrays.


> const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩







4. Give an example of using the spread operator to add a new item to an array.

> const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]





5. Give an example of using the spread operator to combine two objects into one.

> const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂 



## How to Pass Functions Between Components 

1. In the video, what is the first step that the developer does to pass functions between components?


2. In your own words, what does the increment function do?
its increse the intinl value (update the intial value )

3. How can you pass a method from a parent component into a child component?
whit the props 


4. How does the child component invoke a method that was passed to it from a parent component?


[refrance](https://reactjs.org/docs/lists-and-keys.html)
[refrance](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
[refrance](https://www.youtube.com/watch?v=c05OL7XbwXU)