# API Design Best Practices

1. What does REST stand for?

    REST stands for Representational State Transfer. (It is sometimes spelled "ReST".) It relies on a stateless, client-server, cacheable communications protocol -- and in virtually all cases, the HTTP protocol is used. REST APIs are designed around a resources.

2. REST APIs are designed around a ____.

    resources, which are any kind of object, data, or service that can be accessed by the client.

3. What is an identifer of a resource? Give an example.

     a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:
     ```https://adventure-works.com/orders/1```

4. What are the most common HTTP verbs?

    GET, POST, PUT, PATCH, and DELETE.

5. What should the URIs be based on?

    resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

6. Give an example of a good URI.

    I don't know

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

    web APIs that expose a large number of small resources. Bad thing.

8. What status code does a successful GET request return?

    2xx Successful: This means the server successfully processed the request, but is not returning any content.

9. What status code does an unsuccessful GET request return?

    412:“Precondition Failed.” Your browser included certain conditions in its request headers, and the server did not meet those specifications.

10. What status code does a successful POST request return?

    HTTP status code 201 (Created)

11. What status code does a successful DELETE request return?

    A 202 ( Accepted ) status code if the action will likely succeed but has not yet been enacted.

## Things I want to know more about

API best practices.

