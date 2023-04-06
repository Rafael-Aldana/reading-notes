# Redux - Additional Topics

## Redux Toolkit (RTK)

What concerns are addressed by Redux Toolkit?

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code"

What does configureStore() do?

wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

How would I use createSlice()?

Createslice accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

## MobX

What is Mobx?

State is the heart of each application and there is no quicker way to create buggy, unmanageable applications than by producing an inconsistent state or state that is out-of-sync with local variables that linger around. Hence many state management solutions try to restrict the ways in which you can modify state, for example by making state immutable. But this introduces new problems; data needs to be normalized, referential integrity can no longer be guaranteed and it becomes next to impossible to use powerful concepts like classes in case you fancy those.

MobX makes state management simple again by addressing the root issue: it makes it impossible to produce an inconsistent state. The strategy to achieve that is simple: Make sure that everything that can be derived from the application state, will be derived. Automatically.

How does MobX make it “impossible” to produce an inconsistent state?

By using observables, actions, and strict mode, MobX makes it very difficult to produce an inconsistent state in an application. The library helps to ensure that all changes to application state are predictable, controlled, and atomic, which makes it easier to write and maintain complex applications.

How would we build a reactive user interface?

The observer HoC wrapper from the mobx-react-lite package fixes that by basically wrapping the React component in autorun.

## Tutorial

What take-away(s) did this tutorial provide?

Redux helps you deal with shared state management, but like any tool, it has tradeoffs. There are more concepts to learn, and more code to write. It also adds some indirection to your code, and asks you to follow certain restrictions. It's a trade-off between short term and long term productivity.

Redux is more useful when:

You have large amounts of application state that are needed in many places in the app
The app state is updated frequently over time
The logic to update that state may be complex
The app has a medium or large-sized codebase, and might be worked on by many people

[link-to-reading-notes](https://redux-toolkit.js.org/introduction/getting-started).
[link-to-reading-notes](https://mobx.js.org/getting-started.html)
[link-to-reading-notes](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
createReducer(): that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements. In addition, it automatically uses the immer library to let you write simpler immutable updates with normal mutative code, like state.todos[3].completed = true.
createAction(): generates an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.
createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.
createAsyncThunk: accepts an action type string and a function that returns a promise, and generates a thunk that dispatches pending/fulfilled/rejected action types based on that promise
createEntityAdapter: generates a set of reusable reducers and selectors to manage normalized data in the store
The createSelector utility from the Reselect library, re-exported for ease of use.