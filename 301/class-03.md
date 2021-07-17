# Read 03: Passing Functions as Props




## React Docs - lists and keys

Source:
> https://reactjs.org/docs/lists-and-keys.html

1. What does .map() return?
An array with the same length asan array that is being passed in
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
Wrap it into the cruly braces
3. Each list item needs a unique key.
4. What is the purpose of a key?
Keys identify which items have changed, are added, or are removed.

## The Spread Operator

Source:

> https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

1. What is the spread operator?
expands an iterable object into the list of arguments
2. List 4 things that the spread operator can do.
    - spread an array into seaparate arguments
    - copying an array
    - concatenating arrays
    - adding to state in React
3. Give an example of using the spread operator to combine two arrays.

```
const firstArray = [1, 2, 3]
const secondArray = [10, 20, 30]
const combinedArray = [...firstArray, ...secondArray]
```
4. Give an example of using the spread operator to add a new item to an array.

```
const firstArray = [1, 2, 3]
const newArray = [...firstArray, 4, 5, 6]
const combinedArray = [...firstArray, ...secondArray]
```

5. Give an example of using the spread operator to combine two objects into one.

```
const objectOne = {name: "Ayrat"}
const objectTwo = {age: 35}
const objThree =  {...objectOne, ...objectTwo}
```


[**<== BACK**](301-toc.md)