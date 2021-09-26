# Read: Class 01: Readings: Node Ecosystem, TDD, CI/CD

1. **Describe (in plain English) what Array.map() does**

    - Array.map() is a javascript method that loops through an array and creates a new array of an equal length.

2. **Describe (in plain English) what Array.reduce() does**

    - Arra.reduce() produces a single value from an array, by performing actions on its elements. For example, it can be used to find out a total sum or a product of all the elements in the, or find the largest/smallest value wihtin an array. It uses an accumulator to store the "accumulating" while it's looping through each element of the array it working on.

3. **Provide code snippets showing how to use superagent() to fetch data from a URL and log the result**
    - With normal Promise .then() syntax

    ```node
    superagent
    .get('https://pokeapi.co/api/v2/pokemon/')
    .then(res => console.log(res.body))
    ```

    - Again with async / await syntax

    ```node
    async () => {
      res = await superagent.get('https://pokeapi.co/api/v2/pokemon/')
      console.log(res)

    ```

4. **Explain promises as though you were mentoring a Code 301 level student**

    - Promises is one way to run an asynchronous function by creating a promise that needs to be fulfilled either by waiting for a function to complete its action or by catching an error.  

5. **Are all callback functions considered to be Asynchronous? Why or Why Not?**

    - No. Callbacks are just regular functions that are being passed as an argument into another function and will be invoked within.


[**<== BACK**](401-toc.md)