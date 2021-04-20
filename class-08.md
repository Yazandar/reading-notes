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

    * Pixel values are accurate at controlling size and positioning of elements.

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

[Back to Home](README.md)