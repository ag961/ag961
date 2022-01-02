# Read 28: Component Lifecycle / useEffect() Hook

1. Why do we not need more .html pages in a multi-page React app?

    *Because React is a one page framework. It uses one ```index.html```. It creates new html code and injects it into that single page at a certain location as users interact with the page. React is doing so by means of components and browser router.*

2. If we wanted a component to show up on every page, where would we put it and why?
   a) Outside the ```<BrowserRouter/>```
   b) Inside the ```<BrowserRouter />```, outside a ```<Route />```
   c) Inside a ```<Route />```

    *Answer is a and b. If it was placed inside ```<Route />```, it would only be rendered for a specific route.*

3. What does routing do with the components that were rendered when a new route is requested?
   *React will unmount them*
4. What does props.children contain?
  *Whatever was included between an opening and a closing tag of a component as being used in a parent component.*
5. How do useState() and this.setState() differ?
   - useState() is a hook used in functional component to manipulate the State.
   - this.setState() is a function used with class components to manipualte the State object.


## Vocabulary

- State Hook - Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class. [Ref](https://reactjs.org/docs/hooks-state.html)
- Mounting and Un-Mounting - Adding or removing nodes from teh DOM. [Ref](https://stackoverflow.com/questions/31556450/what-is-mounting-in-react-js)

## Resources

[effects hook](https://reactjs.org/docs/hooks-effect.html)



[**<== BACK**](401-toc.md)