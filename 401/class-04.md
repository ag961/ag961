# Readings: Data Modeling

- Name 3 advantages to Test Driven Development ([source](https://www.codica.com/blog/test-driven-development-benefits/))
  1. Better program design and higher code quality
  2. Detailed project documentation
  3. TDD reduces the time required for project development
- In what case would you need to use beforeEach() or afterEach() in a test suite? ([source](https://stackoverflow.com/questions/21418580/what-is-the-difference-between-before-and-beforeeach))
    - when each test within "describe" relies on the exact same data, but each test is also modifying it data, we can use "beforeEach()" and "afteEach()" to bring the data to its original state before or after each test. 
- What is one downside of Test Driven Development
    - tests need to be maintained as code changes
- What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
    - With ES6 Classes we can "extend" and use functionality of a parent class, while in Contructor functions, everything needs to be carried over manually.
- Why REST?
    - because of the simplicity, scalability, flexibility.

## Vocabulary

- functional programming - Functional programming (often abbreviated FP) is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. ([source](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0))
- object-oriented programming (OOP) - application state is usually shared and colocated with methods in objects. ([source](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0))
- class - is a spceial funciotn used to construct objects
- super - refers to parent class
- this - refers to current class
- Test Driven Development (TDD) - software development practice enabling developers to create proper specifications about how their code should be written and implemented. Fundamentally, TDD is a practice when a programmer writes a functional test before building a code. ([source](https://www.codica.com/blog/test-driven-development-benefits/))
- Jest - it's a test libary
- Continuous Integration (CI) - practice of automating the integration of code changes from multiple contributors into a single software project. ([source](https://www.atlassian.com/continuous-delivery/continuous-integration))
- REST - Representational state transfer
- Data Model - visual data map that describes the structure ([source](https://understandingdata.com/what-is-data-modelling/)).

## Resources

[sql vs nosql(Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
[sql modeling techniques](https://www.essentialsql.com/get-ready-to-learn-sql-7-simplified-data-modeling/)
[sequelize api](https://sequelize.org/master/https://sequelize.org/master/)

[**<== BACK**](401-toc.md)