# HTML & CSS 
## Design and Build Websites

## ***Text**

- #### Headings and paragraphs
- #### Bold, italic, emphasis
- #### Structural and semantic markup

### Headings
#### HTML has six "levels" of headings:
#### `<h1>` is used for main headings `<h2>` is used for subheadings If there are further sections under the subheadings then the `<h3>` element is used, and so on... . 

### Paragraphs 

#### To create a paragraph, surround the words that make up the paragraph with an opening `<p>` tag and closing `</p>` tag.

### Bold & It alic
#### By enclosing words in the tags `<b>` and `</b>` we can make characters appear bold.
#### By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic.

### Superscript & Subscript
#### The `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.
#### The `<sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

### White Space
#### When the browser comes across two or more spaces next to each other, it only displays one space. Similarly if it comes across a line break, it treats that as a single space too. This is known as **white space collapsing**.

### Line Breaks & Horizontal Rules
#### As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag `<br />`.
#### To create a break between themes such as a change of topic in a book or a new scene in a play you can add a horizontal rule between sections using the `<hr />` tag.

### Strong & Emphasis 
#### The use of the `<strong>` element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.
#### By default, browsers will show the contents of a `<strong>` element in bold.
#### The `<em>` element indicates emphasis that subtly changes the meaning of a sentence.
#### By default browsers will show the contents of an `<em>` element in italic.


## ***Introducing CSS**
### CSS Associates Style rules with HTML elements
#### CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a `selector` and a `declaration`.

![selector and a declaration pic](https://miro.medium.com/max/3840/1*naFDyXh9iGtmvNRhhFY-og.png)

- #### This rule indicates that all `<p>` elements should be shown in the font size 1.2.
- #### Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.
- #### Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.
- #### CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.


# JAVASCRIPT
## ***Basic JavaScript Instructions**
- ### A script is made up of a series of statements. Each statement is like a step in a recipe.
- ### Scripts contain very precise instructions. For example, you might specify that a value must be remembered before creating a calculation using that value.
- ### Variables are used to temporarily store pieces of information used in the script.
- ### Arrays are special types of variables that store more than one piece of related information.
- ### JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).
- ### Expressions evaluate into a single value.
- ### Expressions rely on operators to calculate a value.

## ***Decisions and Loops**

#### Looking at a flowchart (for all but the most basic scripts), the code can take more than one path, which means the browser runs different code in different situations. you will learn how to create and control the flow of data in your scripts to handle different situations.

#### Scripts often need to behave differently depending upon how the user interacts with the web page and/or the browser window itself. To determine which path to take, programmers often rely upon the following three concepts:

- ### EVALUATIONS: You can analyze values in your scripts to determine whether or note they match expected results.
- ### DECISIONS: Using the results of evaluations, you can decide which path your script should go down.
- ### LOOPS: There are also many occasions where you will want to perform the same set of steps repeatedly.