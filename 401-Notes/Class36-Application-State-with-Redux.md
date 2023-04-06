# Application State with Redux

## Dan Abramov Redux Tutorials

1. What is the first principle of Redux?

The fisrt principle of redux is whether your app is really simple one or a complex app your're going to represent the state of the entire app in one object.

2. what is a store and what do we use our reducers for within that store?

The store holds the current application's state object, it lets you dispatch actions, and when we created we need to specify how state will be updated using a reducer actions.

3. Name three Redux store methods given to us by createStore and describe their use.

  1. get state
  2. dispatch
  3. subscribe

4. Explain to a non-technical recruiter what combineReducers() does and why it is useful.

The object contains key/value pairs where the key is the name of the reducer and the value is the reducer function. combineReducer() returns a function that takes the state and action as arguments. The function will call the reducer function that matches the key in the object and return the new state.

[link-to-reding-notes](https://egghead.io/courses/getting-started-with-redux).

### Bookmark and Review

[link-to-reading-notes](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)
[link-to-reading-notes](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)
[link-to-reading-notes](https://redux.js.org/)
*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
When do I use Redux?