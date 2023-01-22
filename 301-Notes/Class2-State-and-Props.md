# State and Props

This reading topic is important because these are two different concepts we will be utilizing in the next few weeks of the course.

## React lifecycle

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
Based of the diagram, the first thing that happens is render and then componentDidMount.

What is the very first thing to happen in the lifecycle of React?
The very first thing that happens in the lifecycle of React is the mounting an instance.

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.
React updates, constructor, render, componentDidMount, componentWillUnmount

What does componentDidMount do?
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

Here we use componentDidMount() to connect to the YouTube API and get videos when the components is rendered.

[link-to-reding-notes](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093).

********************************************************************************************************************

## React State vs Props

What types of things can you pass in the props?
In props you can pass arguements.

What is the big difference between props and state?
State is handled inside of a component and updates inside as well and props are handled outside of it and updated outside.

When do we re-render our application?
The appication is re-rendered when state is updated based on something that the user has done.

What are some examples of things that we could store in state?
Things that can be stored in state should be things like a counter or things that are going to re-render or update the application based on something that the user has done.

[link-to-reding-notes](https://www.youtube.com/watch?v=IYvD9oBCuJI).

### Things I want to know more about: 

How we will use state as opposed to props?


