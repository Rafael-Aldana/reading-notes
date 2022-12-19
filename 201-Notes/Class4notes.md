# Class 04 code-201d93

To create a basic link, we wrap text or other content inside what element?
To create a a basic link we wrap text inside an anchor tag.

The href attribute contains what information?
The href attribute contains the web address to the website the link is refferring to.

What are some ways we can ensure links on our pages are accessible to all readers?
Using best practices for all users regardless of their current context and which tools they prefer. For example:

Screen reader users like jumping around from link to link on the page, and reading links out of context.
Search engines use link text to index target files, so it is a good idea to include keywords in your link text to effectively describe what is being linked to.
Visual readers skim over the page rather than reading every word, and their eyes will be drawn to page features that stand out, like links. They will find descriptive link text useful.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks).
********************************************************************************************************************
What is meant by “normal flow”?
The normal flow means the way that webpage elements lay themselves out if you haven't changed their layout.

What are a few differences between block-level and inline elements?
By default, block-level elements are laid out in the block flow direction, which is based on the parent's writing mode (initial: horizontal-tb). Each element will appear on a new line below the last one, with each one separated by whatever margin that's been specified. In English, for example, (or any other horizontal, top to bottom writing mode) block-level elements are laid out vertically.

Inline elements behave differently. They don't appear on new lines; instead, they all sit on the same line along with any adjacent (or wrapped) text content as long as there is space for them to do so inside the width of the parent block level element. If there isn't space, then the overflowing content will move down to a new line.

___ positioning is the default for every html element.
The static position is the default position for HTML elements.

Name a few advantages to using absolute positioning on an element.
First of all, note that the gap where the positioned element should be in the document flow is no longer there — the first and third elements have closed together like it no longer exists! Well, in a way, this is true. An absolutely positioned element no longer exists in the normal document flow. Instead, it sits on its own layer separate from everything else. This is very useful: it means that we can create isolated UI features that don't interfere with the layout of other elements on the page. For example, popup information boxes, control menus, rollover panels, UI features that can be dragged and dropped anywhere on the page, and so on.

Second, notice that the position of the element has changed. This is because top, bottom, left, and right behave in a different way with absolute positioning. Rather than positioning the element based on its relative position within the normal document flow, they specify the distance the element should be from each of the containing element's sides. So in this case, we are saying that the absolutely positioned element should sit 30px from the top of the "containing element" and 30px from the left. (In this case, the "containing element" is the initial containing block. See the section below for more information).

What is a key difference between fixed positioning and absolute positioning?
The absolute position is a computed position by the browser and a fixed position is a position that doen't change rewardless if the browser changes or scrolled through.

Describe the difference between a function declaration and a function invocation.
declare and define are the same, and they mean when you write all the code for your function. At that point the function just sits there doing nothing. call is when you tell the JavaScript interpreter to run the code in your function.

What is the difference between a parameter and an argument?
Argument Vs. Parameter : Explore the Major Difference between Argument and Parameter. The values that are declared within a function when the function is called are known as an argument. Whereas, the variables that are defined when the function is declared are known as a parameter.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning).