# **Chapter 7**

<img src = "https://careerkarma.com/blog/wp-content/uploads/2020/03/html-forms.jpg">

# Forms

## Why Forms?

The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

## Form Controls

There are several types of form controls that you can use to collect information from visitors to your site.

* ADDING TEXT: **Text input (single-line)**

Used for a single line of text such as email addresses and names.

* Making Choices: **Radio buttons**

For use when a user must select one of a number of options.

* Submitting Forms: **Submit buttons**

To submit data from your form to another web page.

* **Password input**

Like a single line text box but it masks the characters entered.

* **Checkboxes**

When a user can select and unselect one or more options.

* **Image buttons**

Similar to submit buttons but they allow you to use an image.

* **Text area (multi-line)**

For longer areas of text, such as messages and comments.

* **Drop-down boxes**

When a user must pick one of a number of options from a list.

* Uploading Files: **File upload**

Allows users to upload files (e.g. images) to a websiteFile upload

## How Forms Work

A user fills in a form and then presses a button to submit the information to the server.

## Summary
 
* Whenever you want to collect information from visitors you will need a form, which lives inside a (form) element.

* Information from a form is sent in name/value pairs.

* Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.

* HTML5 introduces new form elements which make it easier for visitors to fill in forms.

# **Chapter 14**

# Lists, Tables & Forms

## Positioning the Marker
**list-style-position**

Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points.

This property can take one of two values:

* **outside**

The marker sits to the left of the block of text. (This is the default behaviour if this property is not used.)

* **inside**

The marker sits inside the box of
text (which is indented).

## Table Properties

You have already met several properties that are commonly used with tables.

* **width**  to set the width of the table

* **padding** to set the space between the border of each table cell and its content

* **text-transform** to convert the content of the table headers to uppercase

* **letter-spacing, font-size** to add additional styling to the content of the table headers

* **border-top, border-bottom** to set borders above and below the table headers

* **text-align** to align the writing to the left of some table cells and to the right of the others

* **background-color** to change the background color of the alternating table rows

* **:hover** to highlight a table row when a user's mouse goes over it

## Summary

* roperties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables, and forms.


* List markers can be given different appearances using the list-style-type and list-style image properties.

* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.

* Forms are easier to use if the form controls are vertically aligned using CSS.

* Forms benefit from styles that make them feel more interactive.

# **Chapter 6**

<img src = "https://www.edureka.co/blog/wp-content/uploads/2019/09/Events-in-JavaScript.jpg">

# Events

## HOW EVENTS TRIGGER JAVASCRIPT CODE

When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling.

1. Select t he element node(s) you want the script to respond to.

2. Indicate which event on the selected node(s) will trigger the response.

3. State the code you want to run when the event occurs.

## THREE WAYS TO BIND AN EVENT TO AN ELEMENT

Event handlers let you indicate which event you are waiting for on any particular element. There are three types of event handlers.

1. HTML EVENT HANDLERS

2. TRADITIONAL DOM EVENT HANDLERS

3. DOM LEVEL 2 EVENT LISTENERS

## EVENT LISTENERS

Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.


## Summary

* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).

* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.

* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.

* You can use event delegation to monitor for events that happen on all of the children of an element.

* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.

# THE END

