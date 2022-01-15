# Read 31: Context API

1. Describe use cases useState() vs useReducer()
    - useState() - used when manipualting a single state element.
    - useReducer() - used when manipualting moe complex state.
2. Why do custom hooks need the use prefix?
    - `A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.  Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.` [Ref](https://reactjs.org/docs/hooks-custom.html)
3. What do custom hooks usually do?
    - They share logic between other components. Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks. [Ref](https://www.wix.engineering/post/custom-react-hook-when-software-design-meets-react-hooks)
4. Using any list of custom hooks, research and name one that you think will be useful in your applications
    - useToggle ([source](https://usehooks.com/))
``` javascript
import { useCallback, useState } from 'react';
// Usage
function App() {
    // Call the hook which returns, current value and the toggler function
    const [isTextChanged, setIsTextChanged] = useToggle();
    
    return (
        <button onClick={setIsTextChanged}>{isTextChanged ? 'Toggled' : 'Click to Toggle'}</button>
    );
}
// Hook
// Parameter is the boolean, with default "false" value
const useToggle = (initialState = false) => {
    // Initialize the state
    const [state, setState] = useState(initialState);
    
    // Define and memorize toggler function in case we pass down the comopnent,
    // This function change the boolean value to it's opposite value
    const toggle = useCallback(() => setState(state => !state), []);
    
    return [state, toggle]
}
```

5. Describe how a hook that fetches API data might work
   
   A custom hook would take in a URL as a parameter. Then it would call the fetch method inside with that URL.

## Term

**reducer** - The reducer is a pure function that accepts 2 parameters: the current state and an action object. Depending on the action object, the reducer function must update the state in an immutable manner, and return the new state. ([source](https://dmitripavlutin.com/react-usereducer/))

## Resources

- [context api](https://reactjs.org/docs/context.html)
- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [react context links](https://github.com/diegohaz/awesome-react-context)


[**<== BACK**](401-toc.md)