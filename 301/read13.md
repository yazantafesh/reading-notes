# Status Codes Based On REST Methods

1. In your own words, describe what each group of status code represents:

    - 100’s = These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.

    - 200’s = These are the success codes. They tell the client that its request was accepted. In case of asynchronous processing of a request (202), this doesn’t mean the request was successfully processed only that it met all validation requirements at the time of sending.

    - 300’s = These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore. This can have multiple reasons, be temporary or permanent, but the client has to issue a request to the new location.

    - 400’s = These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc. A client is sending incorrect input and should confirm the input parameters are correct before retrying the request.

    - 500’s = These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies, but sometimes they can be directly related to client requests that trigger error exceptions on the server. These errors can be temporary or permanent. Usually it’s best for the client to retry the same request.

2. What is a status code 202?

    Accepted.

3. What is a status code 308?

    This tells the client to use another URL to access the resource and not use the current URL anymore.

4. What code would you use if an update didn’t return data to a client?

    204 No Content - A proper code for updates that don’t return data to the client.

5. What code would you use if a resource used to exist but no longer does?

    410 code is an explicit indication that the requested resource used to exist, but it has since been permanently removed and will not be available in the future.

6. What is the ‘Forbidden’ status code?

    Client error status response code indicates that the server understood the request but refuses to authorize it.

# Build A REST API With Node.js, Express, & MongoDB - Quick 

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    Because it have a sensitive information.

2. What is middleware?

    A software that provides common services and capabilities to applications outside of what’s offered by the operating system.

3. What does app.use(express.json()) do?

    express.json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app.use(express.json());

4. What does the /:id mean in a route?

    This means the component will see the dynamic part in the id parameter.

5. What is the difference beween PUT and PATCH?

    PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely. PATCH is used when you want to apply a partial update to the resource.

6. How do you make a defalut value in a schema?

    Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

7. What does a 500 error status code mean?

    Internal Server Error.

8. What is the difference between a status 200 and a status 201?

    - 200 - OK : The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed.

    - 201 - Created : A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).

## Things I want to know more about

learn more about CRUD methods.
