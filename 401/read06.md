# Authentication

## Review, Research, and Discussion

1. **Explain what a “Singleton” is (in Computer Science terms)**

  A Singleton is an object which can only be instantiated one time. Repeated calls to its constructor return the same instance and in this way one can ensure that they don’t accidentally create, say, two Users in a single User application.

2. **Explain how the Singleton pattern can be used with Node modules, specifically with classes**

  The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.

3. **If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**

  Using Singleton approach.

## Document the following Vocabulary Terms

- **Router Middleware**

What it does is to take the original request, and forward it to a sub-handler according to the path.

- **Dynamic Module Loading**

Function-like form of import that returns a promise of the requested module

- **Singleton Pattern**

A creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.

- **CRUD -> REST Method Matches**

Create - Post

Read - Get

Update - Put

Destroy - Delete

- **Mock Testing**

An approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.

## Preparation Materials

### **Securing Passwords**

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have.

General-purpose hash function designed for speed,because they are often used to calculate checksum values for large data sets and files, to check for data integrity. Using a modern computer one can crack a 16 Character Strong password in less than an hour, thanks to GPU.

To overcome such issues, we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.

### **Basic Auth**

In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic credentials, where credentials is the Base64 encoding of ID and password joined by a single colon :.

It is specified in RFC 7617 from 2015, which obsoletes RFC 2617 from 1999.

HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

### **OWASP Auth Cheatsheet**

**Authentication** is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

**Session Management** is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. The Session Management Cheat Sheet contains further guidance on the best practices in this area.

The cheatsheet also has all useful info someone might need when dealing with OWASP Auth.

### **Bcrypt Docs**

**bcrypt** is a password-hashing function designed by Niels Provos and David Mazières, based on the Blowfish cipher and presented at USENIX in 1999. Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.

The bcrypt function is the default password hash algorithm for OpenBSD and was the default for some Linux distributions such as SUSE Linux.

There are implementations of bcrypt for C, C++, C#, Elixir, Go, Java, JavaScript, Perl, PHP, Python, Ruby, and other languages.
