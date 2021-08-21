# Event Driven Applications

### Review, Research, and Discussion


1. Why is access control important?
- Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach
2. Describe an application that would need access control.
- like the canvas web application there is role for the user and other for TA , and instructor
3. What is a role used for?
-  the role determines which permissions the system grants to the user. For example, you can designate whether a user is an administrator, a specialist, or an end-user, and limit access to specific resources or tasks. An organization may let some individuals create or modify files while providing others with viewing permission only.


### Document the following Vocabulary Terms

1. Authorization
- Authorization is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs
- allows the user to access the various resources based on the user's identity

2. Role Based Access Control
- Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control.
- The roles in RBAC refer to the levels of access that employees have to the network.
3. Capabilities

- A capability  is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights.

### Preparation Materials

1. Event Driven Programming

- Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision

- Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

> Event-Driven Programming makes use of the following concepts:

- An Event Handler is a callback function that will be  called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

> EventEmitter

- Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. 

- We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

``` 
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter; 
```

[ref](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)