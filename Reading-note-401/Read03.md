# Express REST API

### Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware

- process incoming intercept HTTP requests,


- decide if the request should be handed over to the next middleware or just end the response
- process outgoing responses


2. True or false: The route handler is middleware?
- false 



3. In what ways can a middleware function end the process and send data to the browser?

- when the process is finish , the route handler will send the data 
- when there is an error in request ,the error handler will send an error 




4. At what point in the request lifecycle can you “inject” middleware?

- after the route and befor the route handler 





5. What can cause express to error with “Request headers sent twice, cannot start a second response”

- That particular error message is pretty much always caused because of a timing error in the handling of an async response that causes you to attempt to send data on a response after the response has already been sent.
- It usually happens when people treat an async response inside an express route as a synchronous response and they end up sending data twice.


### Document the following Vocabulary Terms

1. Middleware
- a pice of code that may be used to handle and process the request and the response 
2. Request Object
- Request is used to describe an request to a server. Use with fetch() to perform the request and get a Response. Request, fetch(), and Response are a new, low level replacement for XMLHttpRequest.
3. Response Object
- Represents a response from a web request initiated by fetch(). fetch(), Request and Response are a new, low level replacement for XMLHttpRequest.
4. Application Middleware
-  is software that lies between an operating system and the applications running on it
5. Routing Middleware
-  the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware.
6. Test Driven Development
- (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.
7. Behavioral Testing
- Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

[ex ref1](https://stackoverflow.com/questions/63106648/what-is-router-middleware-in-express)
[ex ref2](https://en.wikipedia.org/wiki/Test-driven_development)
[ex ref3](https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm)
[ex ref4](https://www.javascripture.com/)
[ex ref5](https://expressjs.com/en/guide/routing.html)
[ex ref6](https://stackoverflow.com/questions/34983520/express-js-routing-error-cant-set-headers-after-they-are-sent)
