# Funcitonal Programming

## Functional Programming Concepts

Sources:

```
https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa
https://en.wikipedia.org/wiki/Functional_programming
```


1. What is functional programming?
    - a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
1. What is a pure function and how do we know if something is a pure function?
    - It returns the same result if given the same arguments (it is also referred as deterministic)
    - It does not cause any observable side effects
1. What are the benefits of a pure function?
    - It is stable, consistent, predictable.
    - The code iseasier to test.
1. What is immutability?
    - When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.
1. What is Referential transparency?
    - if a function consistently yields the same result for the same input, it is referentially transparent.
    - pure functions + immutable data = referential transparency

## Node JS Tutorial for Beginners #6 - Modules and require()

> Source: https://www.youtube.com/watch?v=xHLd36QoS4k

1. What is a module?

    - a piece of code that has a certain functionality

1. What does the word ‘require’ do?

   - it is importing a module

1. How do we bring another module into the file the we are working in?

  require('path to a module')

1. What do we have to do to make a module available?

    - module.exports= (whatever we we want to be available for use outside)

[**<== BACK**](301-toc.md)