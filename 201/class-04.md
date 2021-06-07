# Links
## Writing Links

Links are created using the (a) element. Users can click on anything between the opening (a) tag and the closing (/a) tag. You specify which page you want to link to using the href attribute.

## Linking to Other Sites

(a)

Links are created using the (a)element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.

Users can click on anything that appears between the opening (a) tag and the closing (/a)tag and will be taken to the page specified in the href attribute.

When you link to a different website, the value of the hrefattribute will be the full web address for the site, which is known as an absolute URL.

## Relative URLs

When you are linking to a page on your own website, you do not need to specify the domain name. You can use relative URLs
which are a shorthand way to tell the browser where a page is in relation to the current page.

This is especially helpful when creating a new website or learning about HTML because you can create links between pages when they are only on your personal computer (before you have got a domain name and uploaded them to the web).

Because you do not need to repeat the domain name in each link, they are also quicker to write.

**Relative Link Type**

* Same Folder
* Child Folder
* Grandchild Folder
* Parent Folder
* GrandParent Folder

## Email Links

mailto:

To create a link that starts up the user's email program and addresses an email to a specified email address, you use the (a)element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

On the right you can see that an email link looks just like any other link but, when it is clicked on, the user's email program will open a new email message and address it to the person specified in the link.

## Summary

* Links are created using the (a) element.

* The (a) element uses the href attribute to indicate the page you are linking to.

* If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

* You can create links to open email programs with an email address in the "to" field.

* You can use the id attribute to target elements within a page that can be linked to.


# Layout

## Key Concepts in Positioning Elements

**Building Blocks**

CSS treats each HTML element as if it is in its own box. This box will either be a block-levelbox or an inline box.

Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors. 

* Block-level elements (start on a new line)
* Inline elements (flow in between surrounding text)

**Containing Elements**

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

It is common to group a number of elements together inside a (div) (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The (div)element that contains this group of elements is then referred to as the containing element.

## Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the positionproperty in CSS. You can also float elements using the float property.

* Normal flow

Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else).

* Relative Positioning

This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.

* Absolute positioning

This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page.


To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed. (You will meet these when we introduce the positioning schemes on the following pages.)

* Fixed Positioning 

This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.

* Floating Elements

Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.

## Summary

* (div) elements are often used as containing elements to group together sections of a page.

* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.

* The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)

* Pages can be fixed width or liquid (stretchy) layouts.

* Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).

* Grids help create professional and flexible designs.

* CSS Frameworks provide rules for common tasks.

* You can include multiple CSS files in one page.


# Functions, Methods, and Objects

## WHAT IS A FUNCTION? 

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

## DECLARING A FUNCTION

To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a function declaration.

## CALLING A FUNCTION

Having declared the function, you can then execute all of the statements between its curly braces with just one line of code. This is known as Calling the function.


## DECLARING FUNCTIONS THAT NEED INFORMATION

Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it parameters. Inside the function, the parameters act like variables .


## CALLING FUNCTIONS THAT NEED INFORMATION

When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name . The values are called arguments, and they can be provided as values or as variables.

## GETTING A SINGLE VALUE OUT OF A FUNCTION

Some functions return information to the code that called them. For example, when they perform a calculation, they return the result.

## GETTING MULTIPLE VALUES OUT OF A FUNCTION 

Functions can return more than one value using an array. For example, this function calculates the area and volume of a box. 

## ANONYMOUS FUNCTIONS & FUNCTION EXPRESSIONS 

Expressions produce a value. They can be used where values are expected. If a function is placed where a browser expects to see an expression, (e.g., as an argument to a function), then it gets treated as an expression. 

* FUNCTION DECLARATION 

A function declaration creates a function that you can call later in your code. It is the type of function you have seen so far in this book. 

In order to call the function later in your code, you must give it a name, so these are known as named functions. Below, a function called area() is declared, which can then be called using its name. 

* FUNCTION EXPRESSION 

If you put a function where the interpreter would expect to see an expression, then it is treated as an expression, and it is known as a function expression. In function expressions, the name is usually omitted. A function with no name is called an anonymous function. Below, the function is stored in a variable called area. It can be called like any function created with a function declaration. 


## IMMEDIATELY INVOKED FUNCTION EXPRESSIONS

This way of writing a function is used in several different situations. Often functions are used to ensure that the variable names do not conflict with each other (especially if the page uses more than one script). 

* IMMEDIATELY INVOKED FUNCTION EXPRESSIONS (llFE) 
* WHEN TO USE ANONYMOUS FUNCTIONS AND llFES

## VARIABLE SCOPE 

The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.

* LOCAL VARIABLES
* GLOBAL VARIABLES 

## HOW MEMORY & VARIABLES WORK

Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed.

* CREATING THE VARIABLES IN CODE

Each variable that you declare takes up memory. The more variables a browser has to remember, the more memory your script requires to run. Scripts that require a lot of memory can perform slower, which in turn makes your web page take longer to respond to the user.

* NAMING COLLISIONS 

You might think you would avoid naming collisions; after all you know which variables you are using. But many sites use scripts written by several people. If an HTML page uses two JavaScript files, and both have a global variable with the same name, it can cause errors


# 6 Reasons for Pair Programming

## How does pair programming work?

While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

## Why pair program?

While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

During a five-hour paired lab session, Code Fellows students work on all four of these language-specific skills. The abilities they foster will serve them well in completing assignments, in their own communication and learning, in interviews, and in readiness for a job at a company that utilizes this agile practice.

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness


# THE END
