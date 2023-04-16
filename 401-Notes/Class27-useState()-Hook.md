# useState() Hook

## Thinking in React

Summarize the five steps of thinking in react.

Break the UI into a component hierarchy: This involves breaking down the UI into smaller, reusable components.
Build a static version of the UI: Build a static version of the UI using the components identified in step 1.
Identify the minimal (but complete) representation of UI state: Determine the minimal amount of state that needs to be tracked for the UI to be interactive.
Identify where your state should live: Determine which component should own the state identified in step 3.
Add inverse data flow: Finally, add the ability for the data to flow back up from the child components to the parent component so that the UI can respond to user input.

## State: A Component’s Memory

What is one reason a local variable isn’t sufficient for managing a React component?

One reason a local variable isn't sufficient for managing a React component is that local variables do not automatically trigger a re-render of the component when their value changes. In order to update the UI with the new value of the variable, the component needs to be explicitly re-rendered. This can lead to bugs and inconsistencies in the UI if not properly handled. By using state or props to manage component data, React ensures that the UI is always up-to-date with the latest data.

What is the argument to the useState hook, and what are the two parts of its return array?

The useState hook in React takes an initial state value as its argument and returns an array with two elements.

The first element is the current state value, and the second element is a function that can be used to update the state value. When the update function is called with a new value, React will automatically re-render the component with the updated state value.

How can Component A access state from Component B?

To access state from Component B in Component A, you need to lift the state up to a common parent component of both Component A and Component B. This means that the parent component will hold the state, and pass it down to both Component A and Component B as props. Then, when the state is updated in Component B, it will trigger a re-render in the parent component, which will also update the state in Component A. This technique is known as "lifting state up" and is a common pattern in React.

[link-to-reading-notes](https://react.dev/learn/thinking-in-react).
[link-to-reading-notes](https://react.dev/learn/state-a-components-memory).

## Bookmark and Review

[link-to-reading-notes](https://react.dev/learn/passing-props-to-a-component).
[link-to-reading-notes](https://react.dev/learn/rendering-lists).
[link-to-reading-notes](https://react.dev/learn/state-as-a-snapshot).
[link-to-reading-notes](https://react.dev/reference/react/useState).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?