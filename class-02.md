# Basics of HTML, CSS & JS

## Headings

* There is six levels of headings ```<h1>``` ,```<h2>```,```<h3>```,```<h4>```,```<h5>```, and```<h6>```.

* ```<h1>```used for main headings.

## Paragraphs

* to create paragraph surrounds the words with ```<p>``` and ```</p>```.

## Bold and Italic

* Characters appear bold if you put them between ```<b>``` and ```</b>```.

* Characters will appear italic if you surround it with ```<i>``` and ```</i>```.

## Superscript and Subscript

* Use ```<sup>``` and ```<sub>```.

## Line Breaks and Horizontal Rules

* ```<br/>``` used to add a line break to paragraph.

* ```<hr/>``` used to add horizontal rule between sections.

## Visual Editor and Their code Views

* Visual editor used for resemble word processors.

* Code views used to show the code that are created by visual editor.

## Semantic Markup

* Semantic markup are text elements that does not affect the page structure, but add extra information.

## Strong and Emphasis

* ```<strong>``` used to indicate that the content has strong importance.

* ```<em>``` used to indicate emphasis that subtly changes the meaning of the sentence.

## Quotations

* ```<blockquote>``` used for long quotes that take up to entire paragraph.

* ```<q>``` use for short quotes.

## Abbreviations and Acronyms

* ```<abbr>``` used for abbreviations and acronyms.

## Citations and Definitions

* ```<cite>``` used to indicate where the citation is from.

* ```<dfn>``` used to indicate the defining instance of a new term.

## Author Details

* ```<address>``` used to contain contacts details for author of the page.

## Changes to content

* The ```<ins>``` element can be used to show content that has been inserted into a document, while the ```<del>``` element can show text that has been deleted from it.

* The ```<s>``` element indicates something that is no longer accurate or relevant.

## CSS

* ```CSS``` allows you to create rules that control the way the content is presented.

* ```CSS``` rule contains two parts : a ```Selector``` and a ```Declaration```.

* ```Selectors``` indicate which element the rule applies to, and ```Declarations``` indicate how the elements referred to in the selector should be styled.

* ```CSS Declarations``` sit inside curly brackets and each is made up of two parts: a ```property``` and a ```value```, separated by a colon.

* The ```<link>``` element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

    * ```href``` specifies the path to the CSS file.

    * ```type``` attribute specifies the type of document being linked to.

    * ```rel``` specifies the relationship between the HTML page and the file it is linked to.

* For internal CSS using ```<style>``` inside the ```<head>``` .

* types of css selectors
    ![css selectors](https://i.pinimg.com/originals/bc/97/96/bc97965579512f8a6d2303934f599c65.png)

* CSS rules cascade in four ways
    1. Last rule: If the two selectors are identical, the latter of the two will take precedence.

    1. Specificity: If one selector is more specific than the others, the more specific rule will take precedence over more general ones.

    1. Important: You can add ```!important``` after any property value to indicate that it should be considered more important than other rules that apply to the same element.

    1. Inheritance: some properties on a tag element can be inherited by child elements.

## Statement
 
 * Statement is a script is a series of instructions that a computer can follow one-by-one. 

 * Comments used to explain the code, and make the code easier to understand.

 ## Variable

 * Variables are temporarily store for data.

 * Stored data in variables can be changed.

 * Before using variable you have to announce that you want to use it, by creating the variable and it a name, also called declaring a variable.

 * After declaring a variable you can assign a value to it.

 * Types of data are : numeric, string, and boolean.

 * Rules for naming variables 
    1. The name must begin with a letter, dollar sign, or an underscore.
    
    1. The name can contain letters, numbers, dollar sign, or an underscore.

    1. Can not use **Keywords** or **Reserved** words.

    1. All variables are case sensitive.

    1. Use a name that describe kind of information that the variable stores.

    1. If your variable name is made up of more that onw word, use a capital letter for first letter of every word *after* the first word.

* Array is a special type of variable. It doesn't just store one value; it stores a list of values.

## Decisions and Loops

* There are two components to decision:
    1. An Expresion is evaluated, which returns a value.

    1. A conditional statement says what to do in a given situation.

* Comparison Operators
    * ```==``` Compares two values to see if they are the same.
    * ```!=``` compares two values to see if they are NOT the same.
    * ```===``` compares two vales to check if both data type and value are the same.
    * ```!==``` compares two vales to check if both data type and value are NOT the same.
    * ```>``` checks if the number on the left is greater than the number on the right.
    * ```<``` checks if the number on the right is greater than the number on the left.
    * ```>=``` checks if the number on the left is greater than or equal to the number on the right.
    * ```<``` checks if the number on the right is greater than or equal to the number on the left.
   

* Logical Operator

    * ```&&``` 
        * ```T && T``` returns ```T```
        * ```T && F``` returns ```F```
        * ```F && T``` returns ```F```
        * ```F && F``` returns ```F```

    * ```||```
        * ```T || T``` returns ```T```
        * ```T || F``` returns ```T```
        * ```F || T``` returns ```T```
        * ```F || F``` returns ```F```

    * ```!```
        * ```!```True returns Fales
        * ```!```Fales returns True

* IF Statement
    * The ```if``` statement evaluates a condition. if the condition evaluates ```true```, any statements in subsequent code block are executed.

* IF .. ELSE Statement
    * The ```if .. else``` statement checks a codition, if it resolves to ```true``` the first code block is executed, if the condition resolves to ```false``` the second code block is run instead.

[Back to Home](README.md) 