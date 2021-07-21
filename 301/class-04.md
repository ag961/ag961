# React and Forms

## React Doc - Forms

Source:

> [React Doc - Forms](https://reactjs.org/docs/forms.html)

1. What is a ‘Controlled Component’?

    - Input form element whose value is controlled by React state

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

    - We should update the state as the user types. Because we receive the current displayed value from the state. And also we can use the data as we type it somewhere else, even before the user clicks submit button.

3. How do we target what the user is entering if we have an event handler on an input field?

    - by using onChange property of input form, and assigning it an event handler.

## The Conditional (Ternary) Operator Explained

Source:

> https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff

1. Why would we use a ternary operator?

    - to shorten our code

2. Rewrite the following statement using a ternary statement:

```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

Solution:

> console.log((x===y) ? 'true' : 'false')




[**<== BACK**](301-toc.md)