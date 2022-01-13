# Read 29: Advanced State with Reducers

1. How can we ensure that an useEffect hook runs only once?
    Use an empty array as a second parameter in useEffect() hook.  [Ref](https://css-tricks.com/run-useeffect-only-once/)
2. Can useState() update more than one state variable at the same time?
   Not if they are standalone variables. However, they can be placed as valuables inside of an object, and that object can be updated through useState() hook. In this case, all the properties of an object can get updated at the same time. [Ref](https://stackoverflow.com/questions/53574614/multiple-calls-to-state-updater-from-usestate-in-component-causes-multiple-re-re) 
3. Is useState() synchronous?
   Asynchronous. The state is not updated immediately.

## Vocabulary

- State Hook - Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class. [Ref](https://reactjs.org/docs/hooks-state.html)
- Component Lifecycle - Each component has several “lifecycle methods” that you can override to run code at particular times in the process. [Ref](https://reactjs.org/docs/react-component.html)

## Resources

[useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
[Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook/)



[**<== BACK**](401-toc.md)