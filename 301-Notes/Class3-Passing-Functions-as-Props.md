# Intro to React and Components

This reading topic is important because we will be exploring different types of operators and method types in 301.

## React Docs- lists and keys

What does .map() return?
The .map() method returns a new array populated with the results of calling a provided function on every element in the calling array.

If I want to loop through an array and display each value in JSX, how do I do that in React?
To do that in React, you need to use the .map() method then return a list item element for each item, finally then you need to assign the resulting arry of elements to a listItmes using the curly braces syntax.

Each list item needs a unique ____.
Each item needs a unique key special string attribute.

What is the purpose of a key?
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

[link-to-reding-notes](https://reactjs.org/docs/lists-and-keys.html).

********************************************************************************************************************

## The Spread Operator

What is the spread operator?
The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

List 4 things that the spread operator can do.
Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments
Adding an item to a list
Adding to state in React
Combining objects
Converting NodeList to an array

Give an example of using the spread operator to combine two arrays.
const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

Give an example of using the spread operator to add a new item to an array.
const fruitStand = ['🍏','🍊','🍌']
const sellFruit = (f1, f2, f3) => { console.log(`Fruits for sale: ${f1}, ${f2}, ${f3}`) }
sellFruit(...fruitStand) // Fruits for sale: 🍏, 🍊, 🍌
fruitStand.pop()
fruitStand.pop()
fruitStand.push('🍉')
fruitStand.push('🍍')
sellFruit(...fruitStand) // Fruits for sale: 🍏, 🍉, 🍍
fruitStand.pop()
fruitStand.pop()
sellFruit(...fruitStand,'🍋') // Fruits for sale: 🍏, 🍋, undefined

Give an example of using the spread operator to combine two objects into one.

const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

[link-to-reding-notes](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab).

********************************************************************************************************************
## How to pass Functions between Components

In the video, what is the first step that the developer does to pass functions between components?
You create a function where ever the state is that you want to change.

In your own words, what does the increment function do?
It is recieving a name then looping through the array to find the matching name and changing the state.

How can you pass a method from a parent component into a child component?
You use the props.

How does the child component invoke a method that was passed to it from a parent component?
The child element uses this.props to invoke the method.

[link-to-reding-notes](https://www.youtube.com/watch?v=c05OL7XbwXU)

### Things I want to know more about: 

Are there any other ways to pass information other than props between parent components to child components.