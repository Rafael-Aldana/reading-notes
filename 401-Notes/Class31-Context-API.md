# Context API

## Choosing the State Structure

Summarize the five principles for structuring state

  - Group related state. If you always update two or more state variables at the same time, consider merging them into a single state variable.

  - Avoid contradictions in state. When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this.

  - Avoid redundant state. If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.

  - Avoid duplication in state. When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.

  - Avoid deeply nested state. Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.

## Passing State Deeply with Context

What problem do Contexts aim to solve?

Context lets the parent component make some information available to any component in the tree below it—no matter how deep—without passing it explicitly through props.

What is one technique to try before useContext?

Start by passing props. If your components are not trivial, it’s not unusual to pass a dozen props down through a dozen components. It may feel like a slog, but it makes it very clear which components use which data! The person maintaining your code will be glad you’ve made the data flow explicit with props.

What hook complements useContext for complex applications?

Managing state: As your app grows, you might end up with a lot of state closer to the top of your app. Many distant components below may want to change it. It is common to use a reducer together with context to manage complex state and pass it down to distant components without too much hassle.
  
[link-to-reading-notes](https://react.dev/learn/choosing-the-state-structure).
[link-to-reading-notes](https://react.dev/learn/passing-data-deeply-with-context).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?