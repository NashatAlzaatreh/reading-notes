# HTML & CSS 
## Design and Build Websites 

## ***Links** 
#### Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

### Writing Links
#### Links are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute.

```
<a href="http://www.imdb.com">IMDB</a>
```

#### The text between the opening `<a>` tag and closing `</a>` tag is known as link text. Where possible, your link text should explain where visitors will be taken if they click on it (rather than just saying "click here"). Below you can see the link to IMDB that was created on the previous page.

### Directory Structure
#### On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

### Rela tive URLs
#### Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

### Email Links
#### To create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>` element. However, this time the value of the href attribute starts with `mailto:` and is followed by the email address you want the email to be sent to.

#### You can use the id attribute to target elements within a page that can be linked to.

## ***Layout**

### Key Concepts in Positioning Elements
#### Building Block: CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
#### Block-level elements: start on a new line
#### Examples include: `<h1>` ` <p>` ` <ul> ` `<li>`
#### Inline elements flow in between surrounding text 
#### Examples include: `<img> <b> <i>`

### Containing Elements
#### If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

### Controll ing the Position of Elements
#### CSS has the following positioning schemes that allow  you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the `float` property.

- #### Normal flow
- #### Relative Positioning
- #### Absolute positioning
#### To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.
- #### Fixed Positioning
- #### Floating Elements


# JAVASCRIPT

## ***Functions, Methods, and Objects**
#### Browsers require very detailed instructions about what we want them to do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code.

### WHAT IS A FUNCTION?
#### Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements).

### Why Functions?
#### You can reuse code: Define the code once, and use it many times.

#### You can use the same code many times with different arguments, to produce different results.
###  Function Syntax
#### A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

#### The parentheses may include parameter names separated by commas: (parameter1, parameter2, ...)
#### The code to be executed, by the function, is placed inside curly brackets: {}

```
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```
#### Function parameters are listed inside the parentheses () in the function definition.

#### Function arguments are the values received by the function when it is invoked.

#### Inside the function, the arguments (the parameters) behave as local variables.
### Function Invocation
#### The code inside the function will execute when "something" invokes (calls) the function

### ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS 
#### Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression.

## ***6 Reasons for Pair Programming**
#### More “two heads are better than one” than “stop reading over my shoulder,” pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together. At Code Fellows, pair programing is one way we foster a collaborative environment while developing key industry skill.
1. #### Greater efficiency.
2. #### Engaged collaboration.
3. #### Learning from fellow students.
4. #### Social skills.
5. #### Job interview readiness.
6. #### Work environment readiness.
