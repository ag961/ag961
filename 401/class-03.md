# Readings: Express REST API

- Name 3 real world use cases where you’d want to change the request with custom middleware
  - Add a time stamp of when the sever recevied the request before passing it to route handler
  - To parse data in the request into a json format
    - To add new properties to request object that we plan to use later for an API

- True or false: The route handler is middleware?
  - False. The goal of a route handler is to end the request-response cycle, while middleware passes req/res to the next middleware or a route handler.
- In what ways can a middleware function end the process and send data to the browser?
  - By using a conditional statement. If the conditional statmenet is met, the middleware should ```res.send```.

- At what point in the request lifecycle can you “inject” middleware?
  - Middleware for all routes has to be used before the routes are defined. Middleware for a specific route is passed as an argument after the route path, but before the route handler.
- What can cause express to error with “Request headers sent twice, cannot start a second response”
  - This will happen if we make a conditional statement within a route handler that sends a response, but fail to put ```return``` statement that is supposed to end the function. Without "return" the function will keep running. And if there is a different response after the conditional statmenet, the same route handler will try to send off two response.

### Terms
Request Object - created by Express and passed as argument to middleware or a route handler; contains data sent by the client. 
Response Object - created by Express and passed as another argument to middleware or a route handler; contains data to be sent back to cient. closes request-response cycle.
Application Middleware - Middleware that is called for all requests
Routing Middleware - Middleware that is called for a request to specific route
Test Driven Development - software building process where building tests happen as the woftware is being created, and not after
Behavioral Testing - esting of the external behaviour of the program, also known as black box testing

### Sources:

ES6 Classes - <https://canvas.instructure.com/courses/3433090/discussion_topics/12497475>
Express routing - <https://expressjs.com/en/guide/routing.html>
Writing middleware - <https://expressjs.com/en/guide/writing-middleware.html>
Understanding node error - <https://www.codementor.io/@oparaprosper79/understanding-node-error-err_http_headers_sent-117mpk82z8>
<https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm>
<https://en.wikipedia.org/wiki/Test-driven_development>

### Preview

- Which 3 things had you heard about previously and now have better clarity on?
  - middleware, route handler, testing
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - middleware, request/reqsponse cycle, error-handling
- What are you most excited about trying to implement or see how it works?
  - working with SQL databases

[**<== BACK**](401-toc.md)
