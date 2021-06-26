# HTML & CSS & JAVASCRIPT
## Design and Build Websites

### Understanding The Problem Domain Is The Hardest Part Of Programming

#### what is the problem domain?
#### Problem domain  is an engineering term referring to all information that defines the problem and constrains the solution (the constraints being part of the problem).

#### The problem domain is the software that solves problem of some users where larger systems or businesses may depend on the software, and where problems in the software can lead to indirect loss and this software is termed as industrial strength software.

### What can you do about it?
#### If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

- #### Make the problem domain easier
- #### Get better at understanding the problem domain

#### You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
#### The other choice is to become better at understanding problem domains.  As developers, we tend to think that sitting down and talking to customers or business people who know about the problem domain is a waste of time. It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.  


### ***WHAT IS AN OBJECT?**
#### Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

- #### IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES
- #### IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS


###  Creating an Object 

#### CREATING· OBJECTS USING LITERAL NOTATION

#### This example starts by creating an object using literal notation.
#### This object is called hotel which represents a hotel called Quay with 40 rooms (25 of which have been booked).
#### Next, the content of the page is updated with data from this object. It shows the name of the hotel by accessing the object's name property and the number of vacant rooms using the checkAvail ability() method.
#### To access a property of this object, the object name is followed by a dot (the period symbol) and the name of the property that you want. 
#### Similarly, to use the method, you can use the object name followed by the method name. hotel .checkAvailability()
#### If the method needs parameters, you can supply them in the parentheses (just like you can pass arguments to a funct ion).

```
var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var elName = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms .textContent = hotel .checkAvailability();
```

### ***Document Object Model**
#### The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

#### THE DOM TREE IS A MODEL OF A WEB PAGE
#### As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.
- #### THE DOCUMENT NODE
- #### ELEMENT NODES
- #### ATTRIBUTE NODES
- #### TEXT NODES

### WORKING WITH THE DOM TREE
#### Accessing and updating the DOM tree involves two steps:
#### 1- Locate the node that represents the element you want to work with.
#### 2- Use its text content, child elements, and attributes.

### NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT

#### When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).

#### A Nodelist is a collection of element nodes. Each node is given an index number (a number that starts at zero, just like an array).
#### The order in which the element nodes are stored in a Node List is the same order that they appeared in the HTML page.

### SELECTING AN ELEMENT FROM A NODELIST
#### There are two ways to select an element from a Nodelist: The item() method and array syntax.Both require the index number of the element you want.

### LOOPING THROUGH A NODELIST
#### If you want to apply the same code to numerous elements, looping through a Nodelist is a powerful technique.
#### It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one.
#### Each time the loop runs, the script checks that the counter is less than the total number of items in the Nodelist.

### notes:
#### You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
#### Whenever a DOM query can return more than one node, it will always return a Nadel i st.
#### From an element node, you can access and update its content using properties such as textContent and i nnerHTML or using DOM manipulation techniques.
#### An element node can contain multiple text nodes and child elements that are siblings of each other.
#### In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
#### Browsers offer tools for viewing the DOM tree .

