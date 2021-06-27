# HTML & CSS & JAVASCRIPT
## Design and Build Websites

### Domain Modeling
#### Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

#### A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

### Define a constructor and initialize properties

#### To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an `EpicFailVideo` object.

| Property     | Data              | Type    |
|--------------|-------------------|---------|
| `epicRating` | `1` to `10`       | Number  |
| `hasAnimals` | `true` or `false` | Boolean |

#### Here's an implementation of the `EpicFailVideo` constructor function.

```javascript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```



### Generate random numbers

#### To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a `Math.random()` function for just this sort of occasion.

```javascript
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));
```



### Calculate daily Likes

#### Popularity of a video is measured in Likes. And the formula for calculating Likes is the number of viewers times the percentage of viewers who'll Like a video. In other words, **viewers times percentage**.

#### To calculate the number of viewers per day, generate a random number between 10 and 30 and then multiply it by the epic rating of that video.

| Random number | Epic rating | Viewers per day |
|---------------|-------------|-----------------|
| 10            | 10          | 100             |
| 20            | 9           | 180             |
| 30            | 8           | 240             |

#### The percentage of viewers who'll Like a video depends on whether or not the video contains animals.

| Animals | Percentage |
|---------|------------|
| Yes     | 75%        |
| No      | 40%        |



### Summary

#### Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

#### Here's some tips to follow when building your own domain models.

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
1. Model its attributes with a constructor function that defines and initializes properties.
1. Model its behaviors with small methods that focus on doing one job well.
1. Create instances using the `new` keyword followed by a call to a constructor function.
1. Store the newly created object in a variable so you can access its properties and methods from **outside**.
1. Use the `this` variable within methods so you can access the object's properties and methods from **inside**.


## ***Tables**
### What's a Table?
#### A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

### Basic Table St ructure
- #### The `<table>` element is used to create a table. The contents of the table are written out row by row.
- #### You indicate the start of each row using the opening `<tr>` tag. (The tr stands for table row.) It is followed by one or more `<td>` elements (one for each cell in that row). At the end of the row you use a closing `</tr> ` tag.
- #### Each cell of a table is represented using a `<td>` element. (The td stands for table data.) At the end of each cell you use a closing `</td>` tag.

