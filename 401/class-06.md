# Read Class 06: Authentucation

- Explain what a “Singleton” is (in Computer Science terms)
  - it is a software design pattern that restricts the instantiation of a class to one "single" instance ([source](https://en.wikipedia.org/wiki/Singleton_pattern))
- Explain how the Singleton pattern can be used with Node modules, specifically with classes
  - If we wanted to limit the use of a module and instanciating a class to only once, we could use a Singleton pattern
- If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
  - I would make sure each middleware only performs one thing

## Vocabulary

- Router Middleware - Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router() ([Source](https://expressjs.com/en/guide/using-middleware.html#middleware.router))
- Dynamic Module Loading - allows you to dynamically load modules only when they are needed, rather than having to load everything up front. ([Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules#dynamic_module_loading))
- Singleton Pattern - software design pattern that restricts the instantiation of a class to one "single" instance ([source](https://en.wikipedia.org/wiki/Singleton_pattern))
- CRUD -> REST Method Matches - Create -> Post, Read -> Get, Update -> Put/Patch, Destroy -> Delete  
- Mock Testing - Mocking means creating a fake version of an external or internal service that can stand in for the real one, helping your tests run more quickly and more reliably. ([source](https://circleci.com/blog/how-to-test-software-part-i-mocking-stubbing-and-contract-testing/))

## Resources

[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
[Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)
[OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)
[bcrypt docs](https://www.npmjs.com/package/bcrypt)


[**<== BACK**](401-toc.md)