#  Passing Functions as Props 

## lists and keys
### 1- What does .map() return?
#### - `.map()` return a new array with each element being the result of the callback function.

### 2- If I want to loop through an array and display each value in JSX, how do I do that in React?
#### we loop through the numbers array using the JavaScript `map()` function. We return a `<li>` element for each item. Finally, we assign the resulting array of elements to listItems.
#### We include the entire listItems array inside a `<ul> ` element, and render it to the DOM

#### Example : 

``` javascript 
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((numbers) =>
  <li>{numbers}</li>
);

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
``` 

### 3- Each list item needs a unique "key".

### 4- What is the purpose of a key?
#### Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

## The Spread Operator 

### 1- What is the spread operator? 
#### In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

### 2- List 4 things that the spread operator can do.
##### The `…` spread operator is useful for many different routine tasks in JavaScript, including the following:
 - The spread syntax “spreads” the array into separate arguments.
 - Copying an array
 - Using Math functions
 - Adding an item to a list
 - Adding to state in React
 - Combining objects
 - Converting NodeList to an array


### 3- Give an example of using the spread operator to combine two arrays. 
####  Here are a  basic example of using `… ` in JavaScript, where I demonstrate copying an array, splitting a string into characters, and combining the properties of two JavaScript objects:

``` javascript

[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
```


### 4- Give an example of using the spread operator to add a new item to an array.
### 5- Give an example of using the spread operator to combine two objects into one.

#### Using the `… ` spread operator is a convenient way to copy an array or combine arrays, and it can even add new items:  
``` javascript

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍
```

## How to Pass Functions Between Components

### 1- In the video, what is the first step that the developer does to pass functions between components?

#### The developer made a method and used it in render count

### 2- In your own words, what does the increment function do?

#### The increment function change the count for the chosen name 

### 3- How can you pass a method from a parent component into a child component? 
#### In the parent -inside render function : `increment = {this.increment} ` and in the child `this.props.increment()`
##### *** increment is the method name we pass from a parent component into a child component

### 4- How does the child component invoke a method that was passed to it from a parent component? 

#### `this.props.increment(this.props.name)` and that caused change the state and count and rerender 