# Express REST API

### 1- Name 3 real world use cases where you’d want to change the request with custom middleware

- Comprehensive integration
- Data streaming
- Optimization of existing applications

### 2-True or false: The route handler is middleware?

- false

### 3- In what ways can a middleware function end the process and send data to the browser?

- Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to. ... This “chaining” of middleware allows you to compartmentalize your code and create reusable middleware

### 4- At what point in the request lifecycle can you “inject” middleware?

- when an error is happening or next() or throw error

### 5- What can cause express to error with “Request headers sent twice, cannot start a second response”

- means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.

### Document the following Vocabulary Terms

- Middleware: software which lies between an operating system and the applications running on it

- Request Object: the main entry point for an application to issue a request to the Library

- Response Object: the object which communicates between the server and the output which is sent to the client

- Application Middleware: this can include security authentication, transaction management, message queues, applications servers, web servers and directories

- Routing Middleware: It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware

- Test Driven Development: a software development practice that focuses on creating unit test cases before developing the actual code.

- Behavioral Testing: investigates propensities towards certain kinds of behaviour and styles of interaction with others.
