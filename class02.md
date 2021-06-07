# React: Component Lifecycle Events 

**1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

The answer is render

**2. What is the very first thing to happen in the lifecycle of React?**

* Mounting 

When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting. 


**3. Put the following things in the order that they happen:**

constructor, render, componentDidMount, React Updates, componentWillUnmount.

**4. What does componentDidMount do?**

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().


# React State Vs Props (video)

**1. What types of things can you pass in the props?**

 props in React allows us to pass values from a parent component down to a child component. The values can be any data type, from strings to functions, objects, etc.

**2. What is the big difference between props and state?**

"Props" handled outside of a component, "State" is handled and update it inside of a component.

**3. When do we re-render our application?**

when we change the state inside of our application.

**4. What are some examples of things that we could store in state?**

 date that are inside of a form like checkbox, textbox, or an input element that are being updated by the user.

