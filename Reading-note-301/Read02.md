## React lifecycle 

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? 

the (**render**)

2. What is the very first thing to happen in the lifecycle of React? 

**constructor()** 

3. Put the following things in the order that they happen: 

- constructor
- render 
- React Updates
- componentDidMount 
- componentWillUnmount 

4. What does componentDidMount do?

load anything using a network request or initialize the DOM ,
(dom mainplution , network request)

## React State Vs Props 

1. What types of things can you pass in the props?
as like argument to a function 
(what you want your function or your component to actually take is going to be props )


2. What is the big difference between props and state?
- **props** you pass into component (props handled outside of component  )
- **state** is handled inside that component and you can updated inside the component


3. When do we re-render our application?
- when we change the state inside of the app.
- or change the props outside the component 


4. What are some examples of things that we could store in state?

- if we have a counter app , and we want to update the count 
and then we need state to store these updating .

- useful inside form also .

[refrance](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093),

[refrance](https://www.youtube.com/watch?v=IYvD9oBCuJI),