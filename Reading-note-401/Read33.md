# `<Login />` and `<Auth />`

---

### Review, Research, and Discussion 

**Why is the Context API useful?**

- we dont need to pass the props each time so that a good thing
- The Context API is a React structure that enables you to exchange unique details and assists in solving prop-drilling from all levels of your application

**Can a component outside of a provider get its context?**

- To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext .  

**What are some common use cases for using the Context API?**

- auth  
- them  

**Describe “Context Hell”**

- is the nasty code you get taking advantage of the React Context API.

--- 

### Document the following Vocabulary Terms

**global state**

- Context provides a way to pass data through the component tree without having to pass props down manually at every level, managing state in multiple components that are not directly connected. ... Enough talking about it

**global context**

- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component: class App extends React.

**provider**

- Overview. The `<Provider>` component makes the Redux store available to any nested components that need to access the Redux store. Since any React component in a React Redux app can be connected to the store, most applications will render a `<Provider>` at the top level, with the entire app's component tree inside of it.

**consumer**

- A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. Requires a function as a child. The function receives the current context value and returns a React node.