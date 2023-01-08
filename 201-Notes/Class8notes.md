# Class 08 code-201d93

Flexbox is designed for one-dimensional content. Explain what this means.
Flexbox is designed for one-dimesional content designed to provide greater control over alignment and space distribution between items within a container that means it only deals with layout in a single direction columns or rows at a time.

Explain the difference between the main axis and cross axis.
Since flexbox deals with one-dimensional layout ie. single direction columns or rows this means the main axis is going one direction -----> as opposed to the cross axis that is going in the other direction |
                                                                                             v
How can using certain properties of flexbox negatively impact accessibility?
You should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility. The row-reverse and column-reverse values are a good example of this. The reordering only happens for the visual order, not the logical order. This is important to understand as the logical order is the order that a screen reader will read out the content, and anyone navigating using the keyboard will follow.

[link-to-reading-notes](https://web.dev/learn/css/flexbox/).
********************************************************************************************************************
What are some advantages of using flexbox over float?
The advantages of using flexbox over float are that flexbox is more versatile for editing layouts. Before with float is was either difficult or impossible to achieve with such tools in any kind of convenient, flexible way:

Vertically centering a block of content inside its parent.
Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

How does this topic connect with your long term goals?
This topic just shows the ever changing world of technology we are all heading into things are evolving and getting easier but more complex.
[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox).