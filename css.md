# CSS 

## CSS 

* Is used to design your web page.
* CSS works by associating rules with HTML elements.
* CSS rule contains two parts: a **selector** and a **declaration**.
    * Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

    * Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.

* CSS declarations sit inside curly brackets and each is made up of two parts: a **property** and a **value**, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon

* There is three types of using **CSS**
    * Inline
    * Internal
    * External

------------------------

## Selectors

* ``` * {} ``` Targets all elements on the page.
* ``` h1, h2, h3 {}``` Targets the ```<h1>```, ```<h2>``` and ```<h3>``` elements.
* ```.note {}``` Targets any element whose class attribute has a value of note.
* ```p.note {}``` Targets only ```<p>``` elements whose class attribute has a value of note.

* ```#introduction {}``` Targets the element whose id attribute has a value of introduction.

* ```li>a {}``` Targets any ```<a>``` elements that are children of an ```<li> ```element (but not other ```<a>``` elements in the page).

* ```p a {}``` Targets any ```<a>``` elements that sit inside a ```<p>``` element, even if there are other elements nested between them.

* ```h1+p {}``` Targets the first ```<p>``` element after any ```<h1>``` element (but not other ```<p>``` elements).

* ```h1~p {}``` If you had two ```<p>``` elements that are siblings of an ```<h1>``` element, this rule would apply to both.

-----------------------

## Colors

* The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
    * **rgb** values These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).

    * **hex** codes These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.

    * **color names** There are 147 predefined color names that are recognized by browsers. For example: DarkCyan.

     [Back to Home](README.md)