# Socket.io


### Review, Research, and Discussion 


1. What is the benefit of transforming data into packets?
- to meet the demands of pervasive data-centric applications and services
- A file has to be broken up into small chunks of data
2. UDP is often refereed to as a connectionless protocol. Why is this?
- It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.
- is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet.
3. Can a socket server application have multiple socket connections?
- Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.
4. Can a socket connection application be connected to multiple socket servers?

- A server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

- On the client-side, it is common practice for new outbound connections to use a random client-side port, in which case it is possible to run out of available ports if you make a lot of connections in a short amount of time.


### Document the following Vocabulary Terms

**Observer Pattern**
- The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.
- It is mainly used for implementing distributed event handling systems
**Listener**
- Much of the Node. js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called. ... All objects that emit events are instances of the EventEmitter class.
**Event Handler**
- allows us to create and handle custom events easily by using events module. Event module includes EventEmitter class which can be used to raise and handle custom events.
**Event Driven Programming**
- js uses events heavily and it is also one of the reasons why Node. js is pretty fast compared to other similar technologies. As soon as Node starts its server, it simply initiates its variables, declares functions and then simply waits for the event to occur.
**Event Loop**
- Event loop is an endless loop, which waits for tasks, executes them and then sleeps until it receives more tasks. The event loop executes tasks from the event queue only when the call stack is empty i.e. there is no ongoing task. The event loop allows us to use callbacks and promises
**Event Queue**
- Node. js is a single-threaded application, but it can support concurrency via the concept of event and callbacks. ... Node thread keeps an event loop and whenever a task gets completed, it fires the corresponding event which signals the event-listener function to execute
**Call Stack**
- The call stack is a LIFO (Last In, First Out) stack. The event loop continuously checks the call stack to see if there's any function that needs to run. While doing so, it adds any function call it finds to the call stack and executes each one in order.

**Emit/Raise/Trigger**
- The EventEmitter is a module that facilitates communication/interaction between objects in Node. EventEmitter is at the core of Node asynchronous event-driven architecture. ... The concept is quite simple: emitter objects emit named events that cause previously registered listeners to be called

**database**
- A database is an organized collection of structured information, or data, typically stored electronically in a computer system.