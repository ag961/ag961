# Putting it all together - Thinking in React

Source:

> [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. How would you break a mock into a component heirarchy?

    - We identify and draw out the components. The component that end up within another component will become its child.

2. What is the single responsibility principle and how does it apply to components?

    - Each component should ideally do one thing.

3. What does it mean to build a ‘static’ version of your application?

    - It is a version that has same UI but without interactivity. Only props are used, no state.

4. Once you have a static application, what do you need to add?

    - Interactivity, which is done thorugh state.

5. What are the three questions you can ask to determine if something is state?

    1. Is it passed in from a parent via props?
    2. Does it remain unchanged over time?
    3. Can you compute it based on any other state or props in your component?

    If so, it isn't state.

6. How can you identify where state needs to live?

    - Identify every component that renders something based on that state.
    - Find a common owner component (a single component above all the components that need the state in the hierarchy).
    - Either the common owner or another component higher up in the hierarchy should own the state.
    - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.


[**<== BACK**](301-toc.md)