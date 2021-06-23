# HTML & CSS & JAVASCRIPT
## Design and Build Websites


## ***Images**

#### There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart.

### Adding Images 
#### To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:
- #### `src` tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site.
- #### `alt`  provides a text description of the image which describes the image if you cannot see it.
- #### `title` You can also use the title attribute with the `<img>` element to provide additional information about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

## Height & Width of Images

#### `height`  specifies the height of the image in pixels.
#### `width`  specifies the width of the image in pixels.

### Where to Place Images in Your Code
#### Where an image is placed in the code will affect how it is displayed.

#### HTML5: Figure and Figure Caption
#### Images often come with captions. HTML5 has introduced a new  `<figure>`  element to contain images and their caption so that the two are associated. You can have more than one image inside the  `<figure>`  element as long as they all share the same caption.

#### The `<figcaption>` element has been added to HTML5 in order to allow web page authors to add a caption to an image.


## ***Color**
### Foreground Color 
#### color: The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

- #### rgb values: These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
- #### hex codes: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
- #### color names: There are 147 predefined color names that are recognized  by browsers. For example: DarkCyan

### Background Color:
#### CSS treats each HTML element as if it appears in a box, and the `background-color` property sets the color of the background for that box.

### CSS3: Opacity
#### CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

## ***Text**
### Typeface Terminology
#### Serif: Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
#### Sans-Serif: Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

#### Monospace: Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

### Specifying Typefaces
#### The `font-family` property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies.

#### The value of this property is the name of the typeface you want to use. 


## ***JPEG vs PNG vs GIF**
### which image format to use and when?
#### There are hundreds of image formats available each with a specific use case.
#### Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

![JPEG vs PNG vs GIF](https://2.bp.blogspot.com/-YMnp4TGhkxI/V8V93Z76nCI/AAAAAAAAP_c/IjZDrss0xKIXFh9w6QU1QRBq8Ma9VfA8QCLcB/s640/1.gif)

- #### JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.

- ####  PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

- #### PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.

### Transparency

- #### JPEG images don’t support transparency and are hence not usable for such cases.

- #### PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparen

- #### GIF images support transparency by declaring a single colour in the colour palette as transparent