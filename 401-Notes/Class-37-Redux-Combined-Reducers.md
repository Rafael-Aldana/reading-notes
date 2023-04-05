# Redux - Combined Reducers

## Multiple Reducers Example

1. Why create multiple reducers?

We create multiple reduceers to minimize the trouble we would go through if we had a gigantic complex reducer.

2. How would you combine multiple reducers?

The way to combine reducers is to create a reducers fucntion and pass the object that you're modifying and which reducer is going to be modifying that data. 

3. How will you manage state as an immutable object? why?

You set the default values in the initial state and return a new state by spreading through the state and settig the state and overwritting it.

## Redux Docs: Using Combined Reducers

1. combineReducers is a utility function to simplify the most common use case when writing ___ _____ .

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state.

2. Explain how combineReducers assembles the new state tree.

combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.

3. How would you define initial state in an app using combineReducers?

There are two ways to define the initial shape and contents of your store's state. First, the createStore function can take preloadedState as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser's localStorage. The other way is for the root reducer to return the initial state value when the state argument is undefined.

## Redux Docs: Combined Reducer Syntax

1. Why will you want to split your reducing functions as your app becomes more complex?

As a redux application grows and becomes more complex it is harder to manage the original reducer fucntion that handles all the actions. It is better to split the reducing funtions into smaller more focused reducers that each handle a specific part of the application state. Reasons may included scalability, reusability and testing.

2. The _____ helper function turns an object whose values are different reducing functions into a single reducing 
function you can pass to ____.
combineReducers -----> createStore.


3. What is a popular convention when naming reducers?

A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: combineReducers({ counter, todos }). This is equivalent to writing combineReducers({ counter: counter, todos: todos }).

[link-to-reding-notes](https://www.youtube.com/watch?v=gBER4Or86hE).
[link-to-reding-notes](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/).
[link-to-reding-notes](https://redux.js.org/api/combinereducers/).
*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?