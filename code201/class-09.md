# HTML & CSS & JAVASCRIPT
## Design and Build Websites 

## ***Forms**
### Why Forms?
#### Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information.
#### HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.

### Form Controls
#### There are several types of form controls that you can use to collect information from visitors to your site.

- #### ADDING TEXT
- #### Ma king Choices
- #### Submitting Forms
- #### Uploading Files

### How Forms Work
#### 1- A user fills in a form and then presses a button to submit the information to the server.
#### 2- The name of each form control is sent to the server along with the value the user enters or selects.
#### 3- The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database..
#### 4- The server creates a new page to send back to the browser based on the information received.

### Form Structure
#### Form controls live inside a `<form>` element. This element should always carry the action attribute and will usually have  method and id attribute too.

#### Every `<form>` element requires an `action` attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

#### Forms can be sent using one of two methods: `get` or `post`.

### Text Input
#### The `<input>` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating. 
#### `type="text"`  When the type attribute has a value of text, it creates a singleline text input.


## ***Lists, Tables & Forms**
### Bullet Point Styles
#### The `list-style-type` property allows you to control the shape or style of a bullet point (also known as a marker). It can be used on rules that apply to the `<ol>, <ul>, and <li>` elements.

```
Unordered Lists
For an unordered list you can use
the following values:
none
disc
circle
square
Ordered Lists
For an ordered (numbered) list
you can use the following values:
decimal
1 2 3
decimal-leading-zero
01 02 03
lower-alpha
a b c
upper-alpha
A B C
lower-roman
i. ii. iii.
upper-roman
I II III
```

### Images for Bullets
``` 
You can specify an image to act
as a bullet point using the
list-style-image property.
The value starts with the letters
url and is followed by a pair
of parentheses. Inside the
parentheses, the path to the
image is given inside double
quotes.
This property can be used on
rules that apply to the <ul> and
<li> elements.
The example on this page also
shows the use of the margin
property to increase the vertical
gap between each item in the
list.
```
### Table Properties 

```css
You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:
width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it
```

## ***Events**
#### When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events.

### HOW EVENTS TRIGGER JAVASCRIPT CODE
##### When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
#### 1- Select t he element node(s) you want the script to respond to.
#### 2- Indicate which event on the selected node(s) will trigger the response.
#### 3- State the code you want to run when the event occurs.