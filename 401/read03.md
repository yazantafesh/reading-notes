# Express REST API

## Review, Research, and Discussion

- **Name 3 real world use cases where you’d want to change the request with custom middleware**

  1- Enterprise Application Integration.

  2- Data Integration.

  3- Message Oriented Middleware.

- **True or false: The route handler is middleware?**

  False. A route handler can make requests and get responses without middleware. Middleware can be added to route handlers or other functions to alter/shape requests/responses.

- **In what ways can a middleware function end the process and send data to the browser?**

  Through the use of the next() Or 500 errors. If an error is triggered, it will end the WRRC and send the 500 message to the user through the broswer.

- **At what point in the request lifecycle can you “inject” middleware?**

  The generated server allows for 3 extension points to inject middleware in its middleware chain. These have to do with the lifecycle of a request.

- **What can cause express to error with “Request headers sent twice, cannot start a second response”**

  This happens when you have more than one response being sent to your client.

## Document the following Vocabulary Terms

- **Middleware** is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

- **Request Object** is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. The request object is application independent in that both servers and clients use the same Request class.

- **Response Object** is the object which communicates between the server and the output which is sent to the client. To write an ASP page, all you need to do is write a standard HTML page, putting in the Active Server Pages script where needed.

- **Application Middleware** is middleware on a global level. this middleware executes on all route route calls.

- **Routing Middleware** is one of those middleware, what it does actualy is to take the original request, and forward it to a sub handler according to the path example : "/home" for a GET request is mapped to function getHome that handle it and eventually send a response to the client on the behalf of the original handler.

- **Test Driven Development** is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

- **Behavioral Testing** is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.

## Preview

  1- **Which 3 things had you heard about previously and now have better clarity on?**

  - Implementation Tests.

  - Unit Tests

  - Middleware

  2- **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

  - Implementation Tests.

  - Unit Tests

  - Middleware

  3- **What are you most excited about trying to implement or see how it works?**

  Tests in general.

## Preparation Materials

- **Review: ES6 Classes**

  Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.

- **Using Express Routing**

  Routing refers to how an application’s endpoints (URIs) respond to client requests.

  You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function.

- **Express Routing**

  With the inclusion of the Express 4.0 Router, we are given more flexibility than ever before in defining our routes. To recap, we can:

  - Use express.Router() multiple times to define groups of routes
  - Apply the express.Router() to a section of our site using app.use()
  - Use route middleware to process requests
  - Use route middleware to validate parameters using .param()
  - Use app.route() as a shortcut to the Router to define multiple requests on a route.
