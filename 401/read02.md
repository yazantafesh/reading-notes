# Express

## What’s the difference between PUT and PATCH?

  In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced.

  With PATCH, however, the enclosed entity contains a set of instructions describing how a resource currently residing on the origin server should be modified to produce a new version.

  Also, another difference is that when you want to update a resource with PUT request, you have to send the full payload as the request whereas with PATCH, you only send the parameters which you want to update.

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

- Postman.

- Mocky.io.

- MockServer.

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

  apiDocjs: Inline Documentation for RESTful web APIs. It creates a documentation from API annotations in your source code. It includes a default template which uses handlebars, Bootstrap, RequireJS and jQuery for the output of the generated apidata.js and apiproject.js as a html-page; Swagger Inspector: Test and Document Your APIs With Ease. It is a free cloud-based API testing and documentation tool to simplify the validation of any API and generate its corresponding OpenAPI documentation. apiDocjs and Swagger Inspector can be primarily classified as “API” tools.

## Compare and contrast SOAP and ReST

- SOAP stands for Simple Object Access Protocol whereas REST stands for Representational State * Transfer.

- SOAP is a protocol whereas REST is an architectural pattern.

- SOAP uses service interfaces to expose its functionality to client applications while REST uses Uniform Service locators to access to the components on the hardware device.

- SOAP needs more bandwidth for its usage whereas REST doesn’t need much bandwidth.

- SOAP only works with XML formats whereas REST work with plain text, XML, HTML and JSON.

- SOAP cannot make use of REST whereas REST can make use of SOAP.

## Document the following Vocabulary Terms

- ***Web Server***: is computer software and underlying hardware that accepts requests via HTTP, the network protocol created to distribute web pages, or its secure variant HTTPS.

- ***Express***: is a back end web application framework for Node.js, released as free and open-source software under the MIT License. It is designed for building web applications and APIs. It has been called the de facto standard server framework for Node.js

- ***Routing***: refers to how an application’s endpoints (URIs) respond to client requests.

- ***WRRC***: web request/response cycle traces how a user’s request flows through the app.

## Preparation Materials

- An introduction to NodeJS and Express

  Express and Node's main benefits, and roughly what the main parts of an Express app might look like (routes, middleware, error handling, and template code). I should also understand that with Express being an unopinionated framework, the way you pull these parts together and the libraries that you use are largely up to you!

- What is NPM?

  npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.

  **npm consists of three distinct components:**

  - the website
  - the Command Line Interface (CLI)
  - the registry

- What is TDD?

  “Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).

  It can be succinctly described by the following set of rules:

  - write a “single” unit test describing an aspect of the program
  - run the test, which should fail because the program lacks that feature
  - write “just enough” code, the simplest possible, to make the test pass
  - “refactor” the code until it conforms to the simplicity criteria
  - repeat, “accumulating” unit tests over time

- CI/CD

  Continuous integration(CI) is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently. Because most modern applications require developing code in different platforms and tools, the team needs a mechanism to integrate and validate its changes.
  