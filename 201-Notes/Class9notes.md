# Class 09 code-201d93

Why are forms so important in web development?
Forms are important for web development because it allows developers to collect data fromusers or they allow them to control a user interface.

When designing a form, what are some key things to keep in mind when it comes to user experience?
Before starting to code, it's always better to step back and take the time to think about your form. Designing a quick mockup will help you to define the right set of data you want to ask your user to enter. From a user experience (UX) point of view, it's important to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.

List 5 form elements and explain their importance.
-The form element defines a form, it's a cotainer element like a section or a footer element but sspecifically for containing forms.
-The input element is the input field for the name.
-The label element defines a label for several form elements.
-The select element defines a drop-down list.
-The textarea element defines a multi-line input field (a text area).

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/Forms).
[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form).
********************************************************************************************************************
How would you describe events to a non-technical friend?
Events are interractions that happen in a webpage wether that's by the actions of a user or occurrences that happen in the page that you're using.

When using the addEventListener() method, what 2 arguments will you need to provide?
The addEventlistener() needs the name of the event and a function to handle the event that is going to happen.

Describe the event object. Why is the target within the event object useful?
The event object provides extra features and useful information it is usually automatically passed to event handlers. The target property of the event object is always a reference to the element the event occurred upon.

What is the difference between event bubbling and event capturing?
Event bubbling describes how the browser handles events targeted at nested elements.
Event capture is like event bubbling but the order is reversed: so instead of the event firing first on the innermost element targeted, and then on successively less nested elements, the event fires first on the least nested element, and then on successively more nested elements, until the target is reached.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events).