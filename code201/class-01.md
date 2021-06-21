# HTML & CSS 
## Design and Build Websites

## ***Introduction**



- #### How People Access the Web
- #### How Websites Are Created
- #### How the Web Works

### How People Access the Web
#### Before we look at the code used to build websites it is important to consider the different ways in which people access the web and clarify some terminology.

##### 1- People access websites using software called a **web browser**.
##### 2- In order to view a web page, users might type a **web address** into their browser
##### 3- The request is sent across the Internet to a special computer known as a **web server** which hosts the website
##### 4- The web server connect the requester to the wep page 
![How People Access the Web](https://media.vlpt.us/images/wonseok2877/post/ceb59090-5afc-4a5a-b67a-50d93fb96a3c/image.png)



### How Websites Are Created

#### All websites use HTML and CSS, but content management systems, blogging software, and e-commerce platforms often add a few more technologies into the mix.

### How the Web Works
#### When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

##### 1- When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site
##### 2- Your computer contacts a network of servers called Domain Name System (DNS) servers. These act like phone books; they tell your computer the IP address associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer.

##### 3- The unique number that the DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users.
##### 4- The web server then sends the page you requested back to your web browser.


## ***Structure** 

- #### Understanding structure
- #### Tags and elements
### HTML Uses Elements to Describe the Structure of Pages

### what is HTML?
#### ***HTML*** is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.

### Anatomy of an HTML element
![Anatomy of an HTML element](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics/grumpy-cat-small.png)


#### The main parts of our element are as follows:
 
- ***The opening tag***: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
- ***The closing tag***: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
- ***The content***: This is the content of the element, which in this case, is just text.
- ***The element***: The opening tag, the closing tag, and the content together comprise the element.

### Anatomy of an HTML document
#### That wraps up the basics of individual HTML elements, but they aren't handy on their own. Now we'll look at how individual elements are combined to form an entire HTML page. Let's revisit the code we put into our index.html example (which we first met in the Dealing with files article):

```md
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="My test image">
  </body>
</html>
```

#### The opening `<html>` tag indicates that anything between it and a closing `</html>` tag is HTML code.
#### The `<body>` tag indicates that anything between it and the closing `</body>` tag should be shown inside the main browser window.

### Attributes 
#### Attributes Tell Us More About Elements
##### Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a `name` and a `value`, separated by an `equals sign`.

![Attributes](https://i.dlpng.com/static/png/7183819_preview.png)

- The ***attribute name*** indicates what kind of extra information you are supplying about the element's content. It should be written in lowercase.
- The ***value*** is the information or setting for the attribute. It should be placed in double quotes. Different attributes can have different values.

## ***Extra Markup**

### How to add **comments** to your code?
#### To add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
`<!-- comment goes here -->`
#### On a long page you will often see comments used to indicate where sections of the page start or end, and to pass on notes to help anyone who is looking at the code understand it.

### **ID Attribute**

#### Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character). It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique).

### **Class Attribute**

#### Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other pages on your own site and links that point to external sites.

### **Block Elements**
#### Some elements will always appear to start on a new line in the browser window. These are known as block level elements.
#### Examples of block elements are `<h1>, <p>, <ul>, and <li>`.

### **Inline Elements**
#### Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements
#### Examples of inline elements are `<a>, <b>, <em>, and <img>`.

### **Grouping Text & Elements In a Block**
#### The `<div>` element allows you to group a set of elements together in one block-level box.

#### For example, you might create a `<div>` element to contain all of the elements for the header of your site (the logo and the navigation), or you might create a `<div>` element to contain comments from visitors

### **Grouping Text & Elements Inline**
#### The `<span>` element acts like an inline equivalent of the `<div>` element. It is used to either:
#### 1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text
#### 2. Contain a number of inline elements

### **IFrames**
#### An `<iframe>` is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.
#### One common use of iframes (that you may have seen on various websites) is to embed a Google Map into a page. The content of the iframe can be any html page (either located on the same server or anywhere else on the web).
#### An iframe is created using the `<iframe>` element. There are a few attributes that you will need to know to use it:
- #### **src**: The src attribute specifies the URL of the page to show in the frame.
- #### **height**:The height attribute specifies the height of the iframe in pixels.
- #### **width**: The width attribute specifies the width of the iframe in pixels.
- #### **scrolling**: The scrolling attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the iframe should have scrollbars or not. This is important if the page inside the iframe is larger than the space you have allowed for it (using the height and width attributes). Scrollbars allow the user to move around the frame to see more content. It can take one of three values: yes (to show scrollbars), no (to hide scrollbars) and auto (to show them only if needed).
- #### **frameborder**: The frameborder attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the frame should have a border or not. A value of 0 indicates that no border should be shown. A value of 1 indicates that a border should be shown.
- #### **seamless**: In HTML5, a new attribute called seamless can be applied to an iframe where scrollbars are not desired. The seamless attribute (like some other new HTML5 attributes) does not need a value, but you will often see authors give it a value of seamless. Older browsers do not support the seamless attribute.

### **Information About Your Pages**
#### The `<meta>` element lives inside the `<head>` element and contains information about that web page.

#### It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire.)
#### The `<meta>` element is an empty element so it does not have a closing tag. It uses attributes to carry the information.


### **Escape Characters** 
#### There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.)
#### Therefore, if you want these characters to appear on your page you need to use what are termed "escape" characters (also known as escape codes or entity references). For example, to write a left angled bracket, you can use either `&lt;` or `&#60;`. For an ampersand, you can use either `&amp;` or `&#38;`.


## ***HTML5 Layout**
### HTML5 is introducing a new set of elements that help define the structure of a page
### **Headers & Footers**
### The `<header>` and `<footer>` elements can be used for:
#### The main header or footer that appears at the top or bottom of every page on the site.
#### A header or footer for an individual `<article>` or `<section> `  within the page.

### **Navigation** 
#### The `<nav>` element is used to contain the major navigational blocks on the site such as the primary site navigation.

### **Articles** 
#### The `<article>` element acts as a container for any section of a page that could stand alone and potentially be syndicated

### **Article**
#### The `<aside>` element has two purposes, depending on whether it is inside an <article> element or not.

### **Sections**
#### The `<section>` element groups related content together, and typically each section would have its own heading



## ***Process  & Design**
### This section discusses a process that you can use when you are creating a new website

### Who is the Site For?
#### Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is.

### Why People Visit YOUR Website?
#### Now that you know who your visitors are, you need to consider why they are coming. While some people will simply chance across your website, most will visit for a specific reason.

### What Your Visitors are Trying to Achieve?
#### First you want to create a list of reasons why people would be coming to your site

### What Information Your Visitors Need?
#### You know who is coming to your site and why they are coming, so now you need to work out what information they need in order to achieve their goals quickly and effectively.

### Site Maps
#### Now that you know what needs to appear on your site, you can start to organize the information into sections or pages.
![Example Site Map](https://blog.hubspot.com/hs-fs/hubfs/dyno-mapper-sitemap-generator.png?width=566&name=dyno-mapper-sitemap-generator.png)


### WireFrames
#### A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

![Example wireframes](https://cdn-images.visual-paradigm.com/handbooks/agile-handbook/wireframe/02-newspaper-site-wireframe-example.png)

##### ...........................................................................................................................
# JAVASCRIPT
## ***Introduction**
## What is JavaScript?
#### ***JavaScript*** (often shortened to ***JS***) is a lightweight, interpreted, object-oriented language with first-class functions, and is best known as the scripting language for Web pages, but it's used in many non-browser environments as well. It is a prototype-based, multi-paradigm scripting language that is dynamic, and supports object-oriented, imperative, and functional programming styles.

## How JavaScript makes web pages more interactive? 
#### 1- ACCESS CONTENT: You can use JavaScript to select any element, attribute, or text from an HTML page.
#### 2- MODIFY CONTENT: You can use JavaScript to add elements, attributes, and text to the page, or remove them.
#### 3- PROGRAM RULES: You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page.
#### 4- REACT TO EVENTS: You can specify that a script should run when a specific event has occurred.


## ***The ABC of Programming**
### Before you learn how to read and write the JavaScript language itself, you need to become familiar with some key concepts in computer programming. They will be covered in three sections:
- #### A: What is a script and how do I creat one?
- #### B: How do computers fit in with the world around them?
- #### C: How do I write a script for a web page?


### What is a script and how do I creat one?
#### A script is a series of instructions that a computer can follow to achieve a goal.

### WRITING A SCRIPT
#### To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it
#### Start with the big picture of what you want to achieve, and break that down into smaller steps.

### DEFINING A GOAL & DESIGNING THE SCRIPT
#### Consider how you might approach a different type of script. 
### SKETCHING OUT THE TASKS IN A FLOWCHART 
#### Often scripts will need to perform different tasks in different situations. You can use flowcharts to work out how the tasks fit together. The flowcharts show the paths between each step.

![flowchart](https://i.stack.imgur.com/FvcwZ.jpg)
### How do computers fit in with the world around them?
#### COMPUTERS CREATE MODELS OF THE WORLD USING DATA

### HOW A BROWSER SEES A WEB PAGE? 
#### 1- RECEIVE A PAGE AS HTML CODE
#### 2- CREATE A MODEL OF THE PAGE AND STORE IT IN MEMORY
#### 3- USE A RENDERING ENGINE TO SHOW THE PAGE ON SCREEN

### HOW HTML, CSS, & JAVASCRIPT FIT TOGETHER?
#### Web developers usually talk about three languages that are used to create web pages: HTML, CSS, and JavaScript.
#### Where possible, aim to keep the three languages in separate files, with the HTML page linking to CSS and JavaScript files.
#### Each language forms a separate layer with a different purpose. Each layer, from left to right. builds on the previous one.

