## Problem Domain

* Problem domian is hard if you do not have all information about problem domain, and easy if you have it all.

* understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:
    1. Make the problem domain easier.

    2. Get better at understanding the problem domain.

* You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

## Object

* Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

* In the object variables become known as a properties.

* In object functions become methods.

* In object name of methods and properties called key.

* the name can not have two keys.

* You access the properties or methods of an object using dot notation. You can access the properties using square brackets.

## The Document Object Model (DOM)

* The Document Object Model specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

* The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers.

* The DOM specifies the way in which the browser should structure this model using a DOM tree. and it is stored in the browsers' memory. It consists of four main types of nodes.

![DOM TREE](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)

* Each node is an object with methods and properties. 
Scripts access and update this DOM tree (not the source HTML file). 
Any changes made to the DOM tree are reflected in the browser. 

* Accessing and updating the DOM tree involves two steps: 

    1. Locate the node that represents the element you want to work with. 
    2. Use its text content, child elements, and attributes. 

* Access the elements
    * Select an individual element node : ```getElementById()``` , ```querySelector()```
    
    * Select multiple elements (Nodelists) : ```getElementsByClassName()``` , ```getElementsByClassName()``` , ```querySelectorAll()``` .

    * Traversing between element nodes: ```parentNode``` , ```previousSibling```/```nextSibling``` , ```firstChild```/```lastChild```

* There are two ways of electing an element from nodelist, the ```item()``` method and array sytax.

* When you have a Nodelist, you can loop through each node in the collection and apply the same statements to each.

* Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements.

* When you select a text node, you can retrieve or amend the content of it using the node Value property.

* You can also use the node Value property to update the content of a text node.

* The ```textContent``` property allows you to collect or update just the text that is in the containing element (and its children).

* There are two very different approaches to adding and reoving content from a DOM tree : the ```innerHTML``` property and DOM manipulation.

* ```innerHTML``` can be used on any element node. It is used both to retrieve and replace content.

* DOM manipulation easily targets individual nodes in DOM tree, whereas ```innerHTML``` is better suited to updating entire fragments.

* DOM manipulation refers to a set of DOM methods that allow you to create element and text nodes, and then attach them to the DOM tree or remove them from DOM tree.

* DOM manipulation offers another technique to add new content to a page (rather than i nnerHTML). It involves three steps:

    1. Create the element using ```createElement()```

    2. Give it content using ```createTextNode()```

    3. Add it to the DOM using ```appendChild()```

* DOM manipulation can be used to remove elements from the DOM tree, in three steps :

    1. Store the element to be removed in a variable.

    2. Store the parent of that element in a variable.

    3. Remove the element from its containing element.

* ```element.innerHTML``` 

    * advantages

        * You can use it to add a lot of new markup using less code than DOM manipulation methods. 
        * It can be faster than DOM manipulation when adding a lot of new elements to a web page. 
        * It is a simple way to remove all of the content from one element (by assigning it a blank string).
    
    * Disadvantages

       *  It should not be used to add content that has come from a user (such as a username or blog comment), as it can pose a significant security risk which is discussed over the next four pages.
       *  It can be difficult to isolate single elements that you want to update within a larger DOM fragment.
       *  Event handlers may no longer work as intended.

* DOM manipulation

    * Advantages

        * It is suited to changing one element from a DOM fragment where there are many siblings. 
        * It does not affect event handlers. 
        * It easily allows a script to add elements incrementally (when you do not want to alter a lot of code at once).

    * Disadvantages

      * If you have to make a lot of changes to the content of a page, it is slower than ```innerHTML```. 
      * You need to write more code to achieve the same thing compared with ```innerHTML```.  

* If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of ```Cross-Site Scripting Attack```s or ```XSS```; otherwise, an attacker could gain access to your users' accounts.

* Validate input going to the server

    1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation. Do not allow untrusted users to submit HTML markup or JavaScript.

    2. Double-check validation on the server before displaying user content/storing it in a database. This is important because users could bypass validation in the browser by turning JavaScript off.

    3. The database may safely contain markup and script from trusted sources (e.g., your content management system). This is because it does not try to process the code; it just stores it.

    4. As your data leaves the database, all potentially dangerous characters should be escaped.

    5. Make sure that you are only inserting content generated by users into certain parts of the template files.

    6. Do not create DOM fragments containing HTML from untrusted sources. It should only be added as text once it has been escaped.

* Once you have an element node, you can use other properties and methods on that element node to access and change its attributes.

* There are two steps to accessing and updating attributes:

    1. Select the element node that carries the attribute and follow it with a period symbol.

    2. Use one of the methods or properties to work with that element's attributes.

* To remove an attribute from an element, first select the element, then call ```removeAttribute()```.

* Modern browsers come with tools that help you inspect the page loaded in the browser and understand the structure of the DOM tree.

[Back to Home](README.md)