## Domain Modeling 

* Domain modeling is the process of creating a conceptual model in code for a specific problem.

* A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain.

* An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an ```object-oriented ```model.

* A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

*  constructor function is defined using a function expression. In other words, the variable is declared and then assigned a function with two parameters called.

*  building your own domain models.

    1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
    2. Model its attributes with a constructor function that defines and initializes properties.
    3. Model its behaviors with small methods that focus on doing one job well.
    4. Create instances using the new keyword followed by a call to a constructor function.
    5. Store the newly created object in a variable so you can access its properties and methods from outside.
    6. Use the this variable within methods so you can access the object's properties and methods from inside.

## Tables

* A table represents information in a grid format. 

* The ```<table>``` element is used to create a table. The contents of the table are written out row by row.

* ```<tr>``` used to start of each row.

* ```<td>``` used to represent each tabel's cell.

* The ```<th>``` element is used just like the ```<td>``` element but its purpose is to represent the heading for either a column or a row.

* To stretch across more than one colomn use inside the ```<td>``` ```colspan="rows number"```.

* To stretch across more than one row use inside the ```<td>``` ```rowspan="rows number"```.

* The headings of the table should 
sit inside the ```<thead>``` element. 

* The body should sit inside the 
```<tbody>``` element. 

* The footer belongs inside the 
```<tfoot>``` element.

## Objects

* The ```new``` keyword and the object constructor create a blank object, you can then add properties and methods to the object.

* To update the value of peoperties, use dot notation or square brackets, they work on objects created using literal or constroctor notation. To delete a property, use the ```delete``` keyword.

* Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods.

* When you create ```instances``` of the object using the constroctor function, the ```new``` keyword followed by call to function creates a new object, the properties of each object are given as arguments to the function.

* The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

* In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

* Arrays are actually a special type of object. They hold a related set of key/value pairs, but the key for each value is its index number.

* You can combine arrays and objects to create complex data structures, arrays can sore a series of objects, objects also can hold arrays.

* Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

* Three groups of built-in objects

    * Browser object model
    * Document object model
    * Global JavaScript objects

* In JavaScript there are six data types: 
    1. Strin
    2. Number
    3. Boolean
    4. Undefined
    5. Null
    6. Object

* In order to work with dates, you create an intance of ```Date``` object, you can then specify the time and date that you want it to represent.

[Back to Home](README.md)
