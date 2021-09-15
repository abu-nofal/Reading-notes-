# Advanced State with Reducers



### Review, Research, and Discussion

1. How can we ensure that an effect hook runs only once?

- If we pass an empty array [] , it just renders the component only once like componentDidMount .

2. Can useState() update more than one state variable at the same time?

- You could combine the state into one state object and then you could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.

```
  const [form, setState] = useState({
    username: '',
    password: ''
  });

```

3. Is useState() synchronous?

- useState and setState both are asynchronous. Even though they are asynchronous, the useState and setState functions do not return promises.
Therefore we cannot attach a then handler to it or use async/await to get the updated state values.



### Document the following Vocabulary Terms

1. State Hook

- The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

2. Component Lifecycle

- the series of methods that are invoked in different stages of the component’s existence. The three phases are: Mounting, Updating, and Unmounting.

