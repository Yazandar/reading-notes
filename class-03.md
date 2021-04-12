## Lists

* ```<ol>``` used for creating ordered list.

* ```<ul>``` used for creating unordered list.

* items of the list should be between these tags ```<li>```here ```</li>```.

* ```<dl>``` usually consists of a series of terms and their definitions. And inside it usually you will see ```<dt>``` and ```<dd>```.

* ```<dt>``` used to contain the term being defined.

* ```<dd>``` used to contain the 
definition.

* Nested lists are lists inside lists.

## Box Dimensions

* Box size by defualt is big enough to hold its content. To set your own dimensions for a box you can use the height and width properties.

* Yo specify the size you can use pixels, percentages, or ems.

* The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values: 
    * hidden
    * scroll

## Border, Margin, and Padding

* Border seperates the edge of one box from another.

* Margin sits outside the edge of the border. 

* Padding is the space between the border of a box and any content contained within it.

* The border-width property is used to control the width of a border.

* Border styl peroperty used to control the style of the border.
    * ```solid```
    * ```dotted```
    * ```dashed```
    * ```double```
    * ```groove```
    * ```ridge```
    * ```inset```
    * ```outset```
    * ```hidden / none```

* you can specigy the border color.

## Centering Content

* to center a box you can set left-margin and right-margin to auto.

* The text-align property is inherited by child elements. You therefore also need to specify the text-align property on the centered box if you do not want the text inside it to be centered.

## Change Inline/Block Display

* The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. the values of this property can take:
    * Inline : causes a block-level element to act like an inline element.

    * block : causes an inline element to act like a block-level element.

    * inline-block : causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

    * none : hides an element from the page.

##  Hiding Boxes Visibility

* hidden

* visible

## Border Images

* The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

## Box Shadows

* The box-shadow property allows you to add a drop shadow around a box.

## Rounded Corners

* Using ```broder-radius``` you can create rounded corners on any box.

## Arrays

* An array is a special type of variable. It doesn't just store one value; it stores a list of values. its useful when you are working with a set of values.

## Creating Array

* Create array and give it a name , assign values inside square brackets, and each value is sperated by comma.
    * Example 

    ``` 
    colors= ['white', 
            'black', 
            'custom'];

## Values in Arrays

* Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero **(not one).**

## If .. Else Statements

* The if .. else statement checks a codition, if it resolves to true the first code block is executed, if the condition resolves to false the second code block is run instead.

## Switch Statements

* A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

## Type Coercion

* Is convering data type behinde the scences to complete an operation.

## Truthy and Falsy Values

* Falsy

|Value|Type|
|-----|----|
|False;|Bloean|
|0;|Number|
|' '; |NaN|
|var x; | variable with no value|
----

* Truthy

|Value|Type|
|-----|----|
|true;|Bloean|
|1;|Number|
|'Word'; |String|
|var 10/5;|Number|
|'true';|String|
|'0'|string|
|'false'|string|
-----

## Checking Equality and Existence

* Because the presence of an object or array can be considered truthy, it is often used to check for the existence of an element within a page.

## Short Circuit Values

* Logical operators are processed left to right. They short-circuit (stop) as soon as they have a result - but they return the value that stopped the processing (not necessarily true or false).

## Loops 

* loops check the coditions, if condition return true it will run the code block, and check it again till it returns false.

* Types of loops 

    * ```for``` it runs the code specific number of times.

    * ```while``` runs the code NOT specific times, the code will continue loop again and again as long as the condition is true.

    * ```do while``` same as while loop but has one difference , that while do will run the code between the curly braces at least once.

## Loop Counters

* A ```for``` loop uses a counter ass a condition. This instructs the code to run a specified number of times.

## Key Loop concepts

* Consider these three points when working with loops

    * Keywords : commonly will se two keywords, break and continue. break causes termination of the loop, continue tells the interpreter to continue with the current iteration.

    * Loops and arrays : loops are very helpful when dealing with arrays if you want to run the same codefor each item in array.

    * Performance issues : its important to remember that a browser comes across JavaScript, it will stop doing anything else until it has processed that script.


[Back to Home](README.md)