# HTML & CSS & JAVASCRIPT
## Design and Build Websites

### Building Blocks
#### CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
#### Block-level elements: start on a new line Examples include:
`<h1> <p> <ul> <li>`
#### Inline elements: flow in between surrounding text Examples include: `<img> <b> <i>`

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

### Overlapping El ements
#### When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.
#### If you want to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front. For example, an element with a z-index of 10 will appear over the top of one with a z-index of 5.

### Clearing Floats
#### The clear property allows you to say that no element (within the same containing element) should touch the left or right hand sides of a box. It can take the following values:

- #### `left` The left-hand side of the box should not touch any other elements appearing in the same containing element.
- #### `right` The right-hand side of the box will not touch elements appearing in the same containing element.
- #### `both` Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.
- #### `none` Elements can touch either side.
### Creating Multi-Column Layouts with Floats

#### Many web pages use multiple columns in their design. This is achieved by using a `<div>`element to represent each column. The following three CSS properties are used to position the columns next to each other:


- #### width: This sets the width of the columns.
- #### float: This positions the columns next to each other.
- #### margin: This creates a gap between the columns. 

### Screen Resolution
#### Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

### Page Sizes
#### Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).

### Fixed Width Layouts
#### Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

### Liquid Layouts
#### Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.


