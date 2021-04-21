## Forms

* There are several types of form controls that you can use to collect information from visitors to your site.

  * Adding Text
  * Making choices
  * Submitting forms
  * Uploading files

* A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element.

* Form controls live inside a ```<form>``` element. This element should always carry the action attribute and will usually have a method and id attribute too.

* Every ```<form>``` element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.

* Forms can be sent using one of two methods: get or post.

* The ```<input>``` element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.

* When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.

* The ```<textarea>``` element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. Any text that appears between the opening ```<textarea>``` and closing ```</textarea>``` tags will appear in the text box when the page loads.

* ```type="radio"``` radio buttons allow users to pick just one of a number of options.

* ```type="checkbox"``` checkboxes allow users to select (and unselect) one or more options in answer to a question.

* The ```<select>``` element is used to create a drop down list box. It contains two or more ```<option>``` elements.

* The ```<option>``` element is used to specify the options that the user can select from. The words between the opening ```<option>``` and closing ```</option>``` tags will be shown to the user in the drop down box.

* The ```<button>``` element was introduced to allow users more control over how their buttons appear, and to allow other elements to appear inside the button. This means that you can combine text and images between the opening ```<button>``` tag and closing ```</button>``` tag.

* The ```<label>``` element can be used in two ways. It can:
    1. Wrap around both the text description and the form input.
    2. Be kept separate from the form control and use the for attribute to indicate which form control it is a label for.

* You can group related form controls together inside the ```<fieldset>``` element. This is particularly helpful for longer forms.

* The ```<legend>``` element can come directly after the opening ```<fieldset>``` tag and contains a caption which helps identify the purpose of that group of form controls.

* Form validation helps ensure the user enters information in a form that the server will be able to understand when the form is submitted.

* If you are asking the user for a date, you can use an ```<input>``` element and give the type attribute a value of date. This will create a date input in browsers that support the new HMTL5 input types.

* ```type="email"``` used for the email input. Browsers that support HTML5 validation will check that the user has provided information in the correct format of an email address.

* ```type="url"``` used when you are asking a user for a web page address. Browsers that support HTML5 validation will check that the user has provided information in the format of a URL.

* ```type="search"``` used for create a single line text box for search queries, HTML5 provides a special search input.

## Lists, Tabels And Forms

* The ```list-style-type``` property allows you to control the shape or style of a bullet point (also known as a marker). It can be used on rules that apply to the ```<ol>```, ```<ul>```, and ```<li>``` elements.

* ```list-style-image``` property used to specify an image to act as a bullet point.

* Lists are indented into the page by default and the ```list-style-position``` property indicates whether the marker should appear on the inside or the outside of the box containing the main points.

* Table properties are :
  * ```width``` to set the width of the table

  * ```padding``` to set the space between the border of each table cell and its content

  * ```text-transform``` to convert the content of the table headers to uppercase

  * ```letter-spacing```, font-size to add additional styling to the content of the table headers

  * ```border-top```, border-bottom to set borders above and below the table headers
  
  * ```text-align``` to align the writing to the left of some table cells and to the right of the others
  
  * ```background-color``` to change the background color of the alternating table rows
  
  * ```:hover```to highlight a table row when a user's mouse goes over it

* The ```empty-cells``` property to specify whether or not their borders should be shown.

* The ```cursor``` property allows you to control the type of mouse cursor that should be displayed to users.

## Events

* EVENTS
  * load: Web page has finished loading

  * unload: Web page is unloading (usually because a new page was requested)

  * error: Browser encounters a JavaScript error or an asset doesn't exist

  * resize: Browser window has been resized

  * scroll: User has scrolled up or down the page

  * keydown: User first presses a key (repeats while key is depressed)

  * keyup: User releases a key

  * keypress: Character is being inserted (repeats while key is depressed)

  * click: User presses and releases a button over the same element

  * dblclick: User presses and releases a button twice over the same element

  * mousedown: User presses a mouse button while over an element

  * mouseup: User releases a mouse button while over an element

  * mousemove: User moves the mouse (not on a touchscreen)

  * mouseover: User moves the mouse over an element (not on a touchscreen)

  * mouseout: User moves the mouse off an element (not on a touchscreen)

    *focus / focusin: Element gains focus

  * blur / focusout: Element loses focus  

  * input: Value in any ```<input>``` or ```<textarea>``` element has changed (IE9+) or any element with the contented i table attribute

  * change: Value in select box, checkbox, or radio button changes (IE9+)

  * submit: User submits a form (using a button or a key)

  *reset: User clicks on a form's res~t button (rarely used these days)

  * cut: User cuts content from a form field

  * copy: User copies content from a form field

  * paste: User pastes content into a form field

  * select: User selects some text in a form field

  * DOMSubtreeModified: Change has been made to document

  * DOMNodeInserted: Node has been inserted as a direct child of another node

  * DOMNodeRemoved: Node has been removed from another node

  * DOMNodelnsertedlntoDocument: Node has been inserted as a descendant of another node

  * DOMNodeRemovedFromOocument: Node has been removed as a descendant of another node

* When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.
  1. Select the element node(s) you want the script to respond to.

  2. Indicate which event on the selected node(s) will trigger the response.

  3. State the code you want to run when the event occurs.

* All modern browsers understand this way of creating an event handler, but you can only attach one function to each event handler.

* Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.

* Because you cannot have parentheses after the function names in event handlers or listeners, passing arguments requires a workaround.

* IES-8 had a different event model and did not support addEventL i stener() but you can provide fallback code to make event listeners work with older versions of IE.

* HTML elements nest inside other elements. If you hover or click on a link, you will be also hovering or clicking on its parent elements.

* When an event occurs, the event object tells you information about the event, and the element it happened upon.

* Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.

* When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see the approach below used; it relies on the this keyword.

[Back to Home](README.md)
