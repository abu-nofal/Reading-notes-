# `useState()` Hook

### Review, Research, and Discussion

1. How does React differ from vanilla JS/HTML/CSS?

- JavaScript is a text-based programming language used both on the client-side and server-side that allows you to make web pages interactive. Where HTML and CSS are languages that give structure and style to web pages
- React JS is a JavaScript library for single page applications. React also allows us to create reusable components. React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple. It works only on user interfaces in the application. This corresponds to the view in the MVC template

2. What is the primary difference between a function component and a class component?

1. function components :

- use normal js functions
- called stateless components. (don't have states)
- can use props as arguments in the function
- don't have a render method(return JSX directly for rendering).
- don't have life cycle methods( there is useEffect instead of them).

2. class components :

- use ES6 classes
- called stateful components (it have a states)
- can use props.
- it have a render method to render the HTML elements.
- it have a life cycle methods.

### Document the following Vocabulary Terms

1. Functional Components

- react components that use normal functions instead of classes.

2. Children / Child Components

- any component that renderd and imported inside another component called child and the parent will be the other component that recieved the child one.