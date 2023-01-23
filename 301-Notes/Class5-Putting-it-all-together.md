# Putting it all together

This reading topic is important because going into the rest of the course we will be using everything we have learned this week on the upcoming days of 301.

## React Docs- Thinking in React

What is the single responsibility principle and how does it apply to components?
The responsibility principle is that a component should ideally do one thing.

What does it mean to build a ‘static’ version of your application?
A static version of your app that renders your data model.

Once you have a static application, what do you need to add?
You’ll want to build components that reuse other components and pass data using props.

What are the three questions you can ask to determine if something is state?

  1. Is it passed in from a parent via props? If so, it probably isn’t state.
  2. Does it remain unchanged over time? If so, it probably isn’t state.
  3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

How can you identify where state needs to live?

Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

[link-to-reding-notes](https://reactjs.org/docs/thinking-in-react.html).

********************************************************************************************************************

## Higher-Order Functions

What is a “higher-order function”?
Functions that operate on other functions, either by taking them as arguments or by returning them

Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
Line two is returning an arrow function that returns m greater than n.

Explain how either map or reduce operates, with regards to higher-order functions.
map takes in an array and a set of arguments and returns a new array with those new arguments.

[link-to-reding-notes](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK).

### Things I want to know more about: 

Out in the industry will we be buiding the layout and the first look of the application.
In how does state change from one component to another.
