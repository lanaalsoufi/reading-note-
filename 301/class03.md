# Passing Functions as Props

## Lists and Keys

**1. What does .map() return?**

we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it.

**2. If I want to loop through an array and display each value in JSX, how do I do that in React?**

In React, transforming arrays into lists of elements is nearly identical.

we loop through the numbers array using the JavaScript map() function. We return a li element for each item. Finally, we assign the resulting array of elements to listItems.

**3. Each list item needs a unique ____.**

string

**What is the purpose of a key?**

Keys help React identify which items have changed, are added, or are removed. 

## The Spread Operator

**1. What is the spread operator?**

In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

**2. List 4 things that the spread operator can do.**

The … spread operator is useful for many different routine tasks in JavaScript, including the following:

1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Using an array as arguments
5. Adding an item to a list
6. Adding to state in React
7. Combining objects
8. Converting NodeList to an array

In each case, the spread syntax expands an iterable object, usually an array, though it can be used on any interable, including a string.

**3. Give an example of using the spread operator to combine two arrays.**

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

**4. Give an example of using the spread operator to add a new item to an array.**

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

**5. Give an example of using the spread operator to combine two objects into one.**

[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }


## How to Pass Functions Between Components

**1. In the video, what is the first step that the developer does to pass functions between components?**

create the function wherever the state is that we’re going to change.

**2. In your own words, what does the increment function do?**
effect a change in one component state from within another component.

**3. How can you pass a method from a parent component into a child component?**

Just like any other props by add it to the object, then write it in the child class.

**4.How does the child component invoke a method that was passed to it from a parent component?**

call it like other regulars functions by adding parentheses.

# THE END