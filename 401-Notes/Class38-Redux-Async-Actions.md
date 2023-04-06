# Redux - Asynchronous Actions

## async actions

1. Why use Redux middleware?

Redux middleware were designed to enable writing logic that has side effects.

2. Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

An action is dispatched by the UI handled by the event handler and it gets intercepted by the middle ware and its sends a request to the api, the api sends a response to the reducer/store and updates the new state and then the new state is sent to the UI to be rendered on screen.

3. How are we accommodating async in our Redux app?

We use redux-thunk to handle any async action in the app.

## thunk middleware


1. Why would you need redux-thunk middleware?

Thunk middleware for Redux. It allows writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.

2. Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.

3. Describe how any return value from the inner thunk function will be made available.

Any return value from the inner function will be available as the return value of dispatch itself.

[link-to-reading-notes](https://redux.js.org/advanced/asyncactions).
[link-to-reading-notes](https://github.com/reduxjs/redux-thunk).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?