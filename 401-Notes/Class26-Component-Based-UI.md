# Component Based UI

## React Quick Start

What are the building blocks of a React app?

Reusable components: Components are the building blocks of any React application, and a single app usually consists of multiple components. These components have their logic and controls, and they can be reused throughout the application, which in turn dramatically reduces the application's development time.

What is the difference between an HTML element and a React component?

In HTML, an element is a fundamental building block of a web page. It consists of a start tag, content, and an end tag. For example, <p> is an HTML element used to define a paragraph, and it has a corresponding closing </p> tag.

In React, a component is a reusable piece of UI that can be composed of other components. It can be a simple component like a button or a complex one like a form. Components in React are written in JavaScript and can be thought of as functions that accept props (short for properties) and return React elements. React components allow for modular and reusable code, making it easier to manage complex user interfaces.

What is JSX and why do we use it?

What Is JSX? JSX stands for JavaScript syntax extension. It is a JavaScript extension that allows us to describe React's object tree using a syntax that resembles that of an HTML template. It is just an XML-like extension that allows us to write JavaScript that looks like markup and have it returned from a component.

Describe the process of embedding JavaScript expressions in JSX.

Embedding Expressions in JSX

You can put any valid JavaScript expression inside the curly braces in JSX. For example, 2 + 2 , user. firstName , or formatName(user) are all valid JavaScript expressions. In the example below, we embed the result of calling a JavaScript function, formatName(user) , into an <h1> element.

Does React or JSX have any special features for iteration or conditional logic?

React has special features for iteration and conditional logic. For iteration, you can use the map() method of an array to create a new array of React components. For example, suppose you have an array of names that you want to display as a list of li elements
This creates a new array of li elements, with each element containing a name from the original names array.

For conditional logic, you can use the ternary operator (? :) or the && operator to conditionally render components. For example, suppose you have a showName boolean that determines whether to show a name

How does React know to respond to a user’s inputs?

React responds to a user's inputs through the use of event handlers. In React, an event is a user action such as clicking a button, typing in a form, or scrolling a page. When an event occurs, React uses an event handler to execute some code in response.

To use an event handler in React, you first need to define a function that will be executed when the event occurs. This function is then passed as a prop to the relevant element in the JSX code. For example, to handle a button click event, you can define a function and pass it as the onClick prop of the button element.When the user clicks the button, the handleClick function will be executed and "Button clicked" will be logged to the console.

What word indicates that a React component manages data with a Hook?

The word that indicates that a React component manages data with a Hook is "useState".

How can two react components share data?

There are four ways to share data between React components:
Parent to child component.
Child to parent component.
Sharing data between sibling.
Sharing data between not related components.

## Render and Commit

What are the three steps of refreshing a React UI?

Props or State Update: The first step is to update the props or state of a React component.

Re-rendering: Once the props or state of a component has been updated, React will automatically re-render the component and its child components.

Virtual DOM Update: Finally, React will update the virtual DOM, which is a lightweight representation of the actual DOM. This is done by comparing the new virtual DOM with the previous one, and updating only the parts that have changed. The result is a fast and efficient update of the UI, without having to re-render the entire page.

How do you trigger updates to a component after the initial render?

State Changes: You can update a component's state by calling the setState() method. This will re-render the component and any child components that depend on its state.

Props Changes: When a parent component updates its props, React will automatically trigger a re-render of any child components that depend on those props.

In both cases, React's Virtual DOM algorithm compares the previous state or props with the new state or props, and then only updates the parts of the DOM that need to change, rather than re-rendering the entire page. This makes updates in React very fast and efficient.

Does React recreate DOM nodes on every rerender?

No, React does not recreate DOM nodes on every rerender. Instead, React uses a virtual DOM to keep track of changes in the UI and to update the real DOM only when necessary. When a component is updated, React will compare the new virtual DOM tree with the previous one, and then update the real DOM only with the necessary changes. This makes the process of updating the UI more efficient and faster than directly manipulating the real DOM.

After React has updated the DOM, what still needs to happen before the user sees the change?
After React has updated the DOM, the browser needs to repaint the screen before the user can see the change. This is done by the browser's rendering engine, which traverses the DOM tree and generates the layout and visual styles for each element on the page. The rendering engine then paints each pixel of the layout on the screen. This process is called reflow and repaint, and it can take some time depending on the complexity of the page and the performance of the user's device.

It's important to note that React tries to optimize this process by minimizing the number of DOM updates and batching them together whenever possible. This helps to reduce the amount of work the rendering engine needs to do and can improve the perceived performance of the application.


[link-to-reading-notes](https://react.dev/learn).
[link-to-reading-notes](https://react.dev/learn/render-and-commit).

## Bookmark and Review

[link-to-reading-notes](https://react.dev/learn/your-first-component).
[link-to-reading-notes](https://react.dev/learn/importing-and-exporting-components).
[link-to-reading-notes](https://react.dev/learn/writing-markup-with-jsx).
[link-to-reading-notes](https://devhints.io/sass).
[link-to-reading-notes](https://devhints.io/react).
[link-to-reading-notes](https://airbnb.io/javascript/react/#naming).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?