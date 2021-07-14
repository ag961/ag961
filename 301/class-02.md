# State and Props

## Reading

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

    * Render happens first.

2. What is the very first thing to happen in the lifecycle of React?

    * Constructor

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
    * constructor
    * render
    * React Updates
    * componentDidMount
    * componentWillUnmount

4. What does componentDidMount do?
    * this method can be sed to fetch data from external API after everything is rendered on the page.

## Videos

1. What types of things can you pass in the props?

    * any values: string, numbers, objects, arrays, etc.

2. What is the big difference between props and state?

    * Props is data that is handled/changed outside of a component and passed down into the component
    * State is changed/updated inside the component and is not passed in from the outside.

3. When do we re-render our application?
    * After the state changes
4. What are some examples of things that we could store in state?
    * objects, numbers, string


## Things I want to know more about

- Why components have to be mounted and unmounted.

- Lifecycle of a component.

[**<== BACK**](301-toc.md)