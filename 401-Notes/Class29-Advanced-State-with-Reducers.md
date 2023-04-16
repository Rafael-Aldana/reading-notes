# Advanced State with Reducers

## Extracting State Logic into a Reducer

What is the motivation for adding a reducer?

Adding a reducer to a React component can help manage complex state by providing a more organized and scalable way of updating state in response to different actions or events. Instead of directly updating state with setters or other methods, a reducer allows state updates to be defined in a centralized location and dispatched through a simple action dispatch. This can make it easier to reason about state changes and reduce the likelihood of bugs or inconsistencies. Additionally, using a reducer can make it easier to share state logic between different components or even across the entire application.

What are actions in the context of a reducer? How are they different than setting state directly?
In the context of a reducer, actions are plain JavaScript objects that describe the changes that need to be made to the state. They typically include a type property, which is a string that describes the type of action being performed, as well as any additional data needed to update the state.

When using a reducer, state is updated by dispatching actions to the reducer, rather than setting the state directly. This is because the reducer is designed to handle complex state updates that may depend on the current state or other factors, while also providing a clear and consistent way to manage state changes. By using actions and a reducer, state management becomes more predictable, testable, and maintainable.

What common list operation is useReduce named for, and why?

useReduce is named after the common list operation "reduce", also known as "fold", where an array is iterated over and its values are combined into a single value using a specified function. The reducer function passed to useReduce takes the current state and an action as input and returns the new state. The action is typically an object with a type property that describes what action to perform on the state. The reducer function is called for each action dispatched to the reducer, and it updates the state accordingly. This is similar to how reduce is used to update an accumulator with each element of an array. By using a reducer with useReduce, a React component can manage more complex state and state updates in a more predictable and maintainable way.

When should you switch from useState to useReducer?

The main difference between the two hooks is that useState is simpler and generally easier to use for most state updates. On the other hand, useReducer is more powerful and useful for managing complex state and state transitions.

So, if you have a simple state that only needs to be updated occasionally, useState is probably the best choice. However, if your state has complex interactions and needs to be updated frequently, or if you have a large number of state variables, useReducer may be a better choice. Additionally, if you find yourself using the same logic for updating state in multiple places, useReducer can help to simplify your code and reduce duplication.

[link-to-reading-notes](https://react.dev/learn/extracting-state-logic-into-a-reducer).

## Bookmark and Review

[link-to-reading-notes](https://react.dev/reference/react/useReducer).
[link-to-reading-notes](https://react.dev/learn/keeping-components-pure).
[link-to-reading-notes](https://react.dev/learn/queueing-a-series-of-state-updates).


*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?