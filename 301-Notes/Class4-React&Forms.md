# React and Forms

This reading topic is important because we will be using forms in our labs and they come in handy.

## React Docs- Forms 

What is a ‘Controlled Component’?

React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
The state is automatically merged witha a partial state into the current state when the setState() method is called.
It can sometimes be tedious to use controlled components, because you need to write an event handler for every way your data can change and pipe all of the input state through a React component. This can become particularly annoying when you are converting a preexisting codebase to React, or integrating a React application with a non-React library. In these situations, you might want to check out uncontrolled components, an alternative technique for implementing input forms.

How do we target what the user is entering if we have an event handler on an input field?
You use the tartget .value property of the event which is passed by the onchange handler whenever the user types on the input tag.

[link-to-reading-notes](https://reactjs.org/docs/forms.html).

********************************************************************************************************************

## The Conditional (Ternary) Operator Explained

Why would we use a ternary operator?
We use a ternary operator to shorten the lines of code.

Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}
result = x === y ? console.log(true) : console.log(false);

[link-to-reading-notes](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff).

### Things I want to know more about: 
W?TF
Can a ternary operator be used on multi line if statements?