# Component Lifecycle / useEffect Hook

## useEffect hook

What is the main intended use case for the useEffect hook?

The main intended use case for the useEffect hook is to perform side effects that need to be cleaned up when the component unmounts, or before the next render. For example, you may want to add an event listener to the window object, and remove it when the component unmounts. You can do this by returning a function from the useEffect hook that removes the event listener.

How does the effect’s logic interact with the component?

The effect function is called after the initial render of the component and then after every re-render if the dependency array provided to the useEffect hook has changed. The dependency array is an optional second argument to the useEffect hook that specifies the variables that the effect depends on. If a dependency is included in the array, the effect will be re-run whenever the value of that dependency changes.

What is the importance of the return value from the effect’s logic function?

The return value from the effect's logic function is important because it defines how the effect will be cleaned up or undone. It allows for the removal of event listeners, timers, or other subscriptions that were set up within the effect's logic function, preventing memory leaks or unexpected behavior.

If the return value is undefined or not provided, the effect will simply run each time the component rerenders. If the return value is a function, it is considered a cleanup function and will be run before the next execution of the effect, allowing for the removal of any resources that were set up in the previous execution of the effect.

[link-to-reading-notes](https://react.dev/reference/react/useEffect#reference).

## Bookmark and Review

[link-to-reading-notes](https://react.dev/learn/responding-to-events).
[link-to-reading-notes](https://react.dev/learn/conditional-rendering).
[link-to-reading-notes](https://react.dev/learn/updating-arrays-in-state).
[link-to-reading-notes](https://react.dev/learn/updating-objects-in-state).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?