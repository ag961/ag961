# CRUD

## Status Codes Based On REST Methods

Source:

> https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/

1. In your own words, describe what each group of status code represents:
    - 100’s = informative codes
    - 200’s = successful requests
    - 300’s = redirection request. the resource isn't avaliable anymore at the location the request was made to,
    - 400’s = client side error
    - 500’s = server side error
1. What is a status code 202?
    - asynchronous processing of a request
1. What is a status code 308?
    - Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.
1. What code would you use if an update didn’t return data to a client?
    - 204 No Content
1. What code would you use if a resource used to exist but no longer does?
    - 410 Gone
1. What is the ‘Forbidden’ status code?
    - 403 Forbidden

## Video - Build A REST API With Node.js, Express, & MongoDB - Quick 

Source:

> https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
    - so that when we deploy our server, it doesn't try to connect the hardcoded string (for example a local host)
1. What is middleware?
    - code that runs when the server gets the request but before it gets passed to your routes
1. What does app.use(express.json()) do?
    - lets the server accept JSON as a body instead of a a get, post, etc. element.
1. What does the /:id mean in a route?
    - gives access to a specific element;
1. What is the difference between PUT and PATCH?
    - PUT replaces entire data, PATCH only replaces specific element in database
1. How do you make a default value in a schema?
    - > { default: 'some value'}
1. What does a 500 error status code mean?
    - there is an error on the server side
1. What is the difference between a status 200 and a status 201?
    - 201 is used with "post" and means successfully created an object. It is more specific that 200, which means everything went well.

[**<== BACK**](301-toc.md)
