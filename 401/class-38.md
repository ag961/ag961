# Read 38: Redux - Asynchronous Actions, Thunk, Redux Thunk

By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store. ([source](https://redux.js.org/tutorials/fundamentals/part-6-async-logic))

Redux can't have side-effects.

But Redux middleware can handle side effects instead.

- Redux middleware has access to `dispatch` and `getState`. We can do some logic in middleware and then interact with Redux store.


### Redux Middleware

Middleware written as ES5 functions

Outer function:
function exampleMiddleware(storeAPI) {
  return function wrapDispatch(next) {
    return function handleAction(action) {
      // Do anything here: pass the action onwards with next(action),
      // or restart the pipeline with storeAPI.dispatch(action)
      // Can also use storeAPI.getState() here

      return next(action)
    }
  }
}

([source](https://redux.js.org/tutorials/fundamentals/part-4-store#middleware))

## Resources

[async actions](https://redux.js.org/advanced/asyncactions)

[thunk middleware](https://github.com/reduxjs/redux-thunk)

[redux thunk](https://alligator.io/redux/redux-thunk/)


[**<== BACK**](401-toc.md)