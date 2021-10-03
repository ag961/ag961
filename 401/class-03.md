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

### Sources:

ES6 Classes - <https://canvas.instructure.com/courses/3433090/discussion_topics/12497475>
Express routing - <https://expressjs.com/en/guide/routing.html>
Writing middleware - <https://expressjs.com/en/guide/writing-middleware.html>
Understanding node error - <https://www.codementor.io/@oparaprosper79/understanding-node-error-err_http_headers_sent-117mpk82z8>

### Terms
Request Object
Response Object
Application Middleware
Routing Middleware
Test Driven Development
Behavioral Testing


[**<== BACK**](401-toc.md)
