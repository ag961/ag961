# Object-Oriented Programming, HTML Tables

## Domain Modeling

retrieved from  
> https://github.com/codefellows/domain_modeling#domain-modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

### Constructor  

A constructor function is used to define the same properties between many objects.  

``` markdown

var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```  

Here, the constructor function is defined using a function expression. After the constructor function definition, two objects are instantiated with the `new` keyword and their properties are `initialized` by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables.

This is object-oriented programming in JavaScript at its most fundamental level.


To generate random numbers use Math.random() function.

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

Methods can be added to a constructor function's prototype.

## Chapter 6: “Tables” (pp.126-145)

Source:
> Duckett, J. (2011). *HTML & CSS: Design and build websites.* Indianapolis, IN: Wiley

`<table>` element is used to create a table
`<tr>` starts each row
`<td>` (nested within `<tr>`) for each cell
`<th>` heading. Attribute `scope="col"` for column, `scope="row"` - row.
`<colspan="number">` - attribute within `<td>` or `<th>` to indicate how many cells to stretch horizontally
`<rowspan="number">` - attribute within `<td>` or `<th>` to indicate how many cells to stretch vertically


## Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

from:
> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

The **new** keyword and the object constructor create a blank object. You can then add properties and methods to the object.

```
let hotel = new Object();
hote.name = 'Quay';
```

To create an emot object using literal notation use: `var hotel = {}`

To update the value of properties use dot notation or square brackets: 
`hotel.name='Park';`

To delete porperty `delete hotel.name;`. To clear, set it to blank.

### Constructor function

A constructor function creates a template for creating new objects with same properties, but different values. The name of a constructor function usually begins with a capital letter. Each property or method created ends in a semicolon.

``` js
function Hotel (name, rooms, booked) {
  this.name = name;
  this.rooms = rooms;
  this.booked = booked;
  this.checkAvailability = function() {
    return this.rooms - this.booked;
  }
}
```

To create instances use **new** keyword followed by a call to the function.



-----

[**<== BACK**](201-toc.md)