## Links

* Links are created using the ```<a>``` element. Users can click on anything between the opening ```<a>``` tag and the closing ```</a>```tag. You specify which page you want to link to using the href attribute.

* The text between the opening ```<a>``` tag and closing ```</a>``` tag is known as link text.

* Links are created using the ```<a>``` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.

* Absolute URL starts with the domain name for that site, and can be followed by the path to a specific page.

* Relative URL is shorthand of the domian.can be used when linking to pages within your own 
website.

* Relative link types
    * Same Folder
    * Child Folder
    * Grandchild Folder
    * Parent Folder
    * Grandparent Folder

* To create a link that starts up the user's email program and addresses an email to a specified email address, you use the ```<a>``` element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

* If you want a link to open in a new window, you can use the target attribute on the opening ```<a>``` tag. The value of this attribute should be ```_blank``` .

## Layout

* CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

* Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes.

* If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

* CSS has the positioning schemes that allow you to control the layout of a page:   

    * Normal flow: every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.
    
    * Relative positioning: this moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. 
    
    * Absolute positioning: this positions the element in relation to its containing element.
    
    
* You specify the positioning scheme using the position property in CSS. You can also float elements using the ```float``` property.

* To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.

* ```position: static;``` its for Normal Flow.

* ```position:relative;``` Relative positioning moves an 
element in relation to where it 
would have been in normal flow.

* ```position:absolute;``` When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page.

* ```position:fixed;``` is a type 
of absolute positioning that 
requires the position property 
to have a value of fixed. It positions the element in 
relation to the browser window.

* ```z-index``` When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page.

* ```float``` this property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.Anything else that sits inside the containing element will flow around the element that is floated.

* ```clear``` property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

    * ```left``` The left-hand side of the box should not touch any other elements appearing in the same containing element.

    * ```right``` The right-hand side of the box will not touch elements appearing in the same containing element.

    * ```both``` Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.

    * ```none``` Elements can touch either side.

* Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

* Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.

* Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

    * Advantages

        *  Pixel values are accurate at controlling size and positioning of elements.

        * The designer has far greater control over the appearance and position of   items on the page than with liquid layouts. 

        * You can control the lengths of lines of text regardless of the size of the user's window.

        * The size of an image will always remain the same relative to the rest of the page.

    * Disadvantages
        
        * ● You can end up with big gaps around the edge of a page. 
        
        * If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read. 
        
        * If a user increases font sizes, text might not fit into the allotted spaces. 
        
        * The design works best on devices that have a site or resolution similar to that of desktop or laptop computers. 
        * The page will often take up more vertical space than a liquid layout with the same content.

* Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

    * Advantages
        
        * Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.
        * If the user has a small window, the page can contract to fit it without the user having to scroll to the side.
        * The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).

    * Disadvantages

        * If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.

        * If the user has a wide window, lines of text can become very long, which makes them harder to read.

        * If the user has a very narrow window, words may be squashed and you can end up with few words on each line. 

        * If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text.

* CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

* Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on. Some authors take an even more modular approach to stylesheets, creating separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site.

## Function

* Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

* Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function, rather than repeating the same set of statements.

* Declaring a function
    * To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces.

* Calling function
    * Having declared the function, you can then execute all of the statements between its curly braces with just oneline of code.

* Declaring functions that need information
    * Sometimes function needs a specific information to perform its task. In such cases, when declare the function you give it a parameters. Inside the function the parameters act like variables.

* Getting a single value out of a function
    * Some functions return information to the code that called them. For example, when they perform a calculation, they return the result.

* Getting multiple values out of a function
    * Functions can return more than one value using an array.

* Anonymous Functions and Function Expressions
    * Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, then it gets treated as an expression.

* Immediately Invoked Function Expressions
    * ```
        var area = (function() 
        var wi dth = 3; 
        var height = 2; 
        return widt h * height; 
        }()); 
    final parentheses after the closing curly brace of the code block tell the interpreter to call the function immediately.

* Variable Scope
    * The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.

* How Memory and Variables Work
    * Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.

## Six Reasons for Pair Programming

1. Greater efficiency

    pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging. it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own.

2. Engaged collaboration

    When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone.

3. Learning from fellow students

   beacuase developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. 

4. Social skills

   working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. 
    

5. Job interview readiness

    A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.


6. Work environment readiness

    Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.


[Back to Home](README.md)