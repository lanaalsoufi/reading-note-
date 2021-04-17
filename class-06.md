# **Chapter (3)**

# Object Literals

## WHAT IS AN OBJECT?

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

* **IN AN OBJECT: VARIABLES BECOMEKNOWN AS PROPERTIES**

If a variable is part of an object, it is called aproperty. Properties te ll us about the object, such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.

* **IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS**

If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms.


* Like variables and named functions,properties and methods have a name and a value. In an object, that name is called a key.

* An object cannot have two keys with the same name. This is because keys are used to access their corresponding values.

* The value of a property can be a string, number, Boolean, array, or even another object. The value of a method is always a function.

**Programmers use a lot of name/value pairs:**

* HTML uses attribute names and values.

* CSS uses property names and values.

**In JavaScript:**

* Variables have a name and you can assign them a value of a string, number, or Boolean.

* Arrays have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)

* Named functions have a name and value that is a set of statements to run if the function is called.

* Objects consist of a set of name/value pairs (but the names are referred to as keys).


## CREATING AN OBJECT: LITERAL NOTATION 

Literal notation is the easiest and most popular way to create objects. (There are several ways to create objects)

* The object is the curly braces and their contents.The object is stored in a variable called hotel, so you would refer to it as the hotel object. 

* Separate each key from its value using a colon. Separate each property and method with a comma (but not after the last value). 

## ACCESSING AN OBJECT AND DOT NOTATION

You access the properties or methods of an object using dot notation. You can also access properties using square brackets.

* To access a property or method of an object you use the name of the object, followed by a period, then the name of the property or method you want to access. This is known as dot notation.

* The  Period is known as the member operator. The property or method on its right is a member of the object on its left. Here, two variables are created to hold the hotel name and number of vacant rooms.


# **Chapter (5)**

# Document Object Model

## THE DOM TREE IS A MODEL OF A WEB PAGE

As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.

**THE DOCUMENT NODE**

* Above, you can see the HTML code for a shopping list, and on the right hand page is its DOM tree. Every element attribute, and piece of text in the HTML is represented by its own DOM node. At the top of the tree a document node is added; it represents the entire page (and also corresponds to the document object).

* When you access any element, attribute, or text node, you navigate to it via the document node. It is the starting point for all visits to the DOM tree.

**ELEMENT NODES**

* HTML elements describe the structure of an HTML page. (The h1 - h6 elements describe what parts are headings; the (p)tags indicate where paragraphs of text start and finish; and so on.) 

* To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to. This is why you start by learning methods that allow you to access element nodes, before learning to access and alter text or attributes.


Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser.


<img src ="https://o.quizlet.com/AfUFVsyOPvhSUhhrRfG0-A.png">


**ATTRIBUTE NODES**

* The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree.

* Attribute nodes are not children of the element thar carries them; they are part of that element. Once you access an element, there are specific JavaScript methods and properties to read or change that element's attributes. For example, it is common to change the values of cl ass attributes to trigger new CSS rules that affect their presentation.

**TEXT NODES**

* Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node.

* Text nodes cannot have children. If an element contains text and another child element, the child element is not a child of the text node but rather a child of the containing element. (See the (em) element on the first (li) item.) This illustrates how the text node is always a new branch of the DOM tree, and no further branches come off of it.


## WORKING WITH THE DOM TREE

Accessing and updating the DOM tree involves two steps:

1: Locate the node that represents the element you want to work with.

2: Use its text content, child elements, and attributes.

**STEP 1: ACCESS THE ELEMENTS**

* SELECT AN INDIVIDUAL ELEMENT NODE

Here are three common ways to select an individual element:

***get El ement Byld ()***

Uses the value of an element's id attribute (which should be unique within the page).

***querySe 1 ector ()***

Uses a CSS selector, and returns the first matching element.

You can also select individual elements by traversing from one element to another within the DOM tree (see third column).

* SELECT MULTIPLE ELEMENTS (NODELISTS)

There are three common ways to select multiple elements:

***getElementsByClassName()***

Selects all elements that have a specific value for their cl ass attribute.

***getElementsByTagName()***

Selects all elements that have the specified tag name ..

***querySelectorAll()***

Uses a CSS selector to select all matching elements.

* TRAVERSING BETWEEN ELEMENT NODES

You can move from one element node to a related element node.

***parentNode***

Selects the parent of the current element node (which will return just one element).

***previousSibl ing / nextSibl ing***

Selects the previous or next sibling from the DOM tree.

***firstChild / lastChild***

Select the first or last child of the current element.

The terms elements and element nodes are used interchangeably but when people say the DOM is working with an element, it is actually working with a node that represents that element.

**STEP 2: WORK WITH THOSE ELEMENTS**

* ACCESS/ UPDATE TEXT NODES

* WORK WITH HTML CONTENT

* ACCESS OR UPDATE ATTRIBUTE VALUES

## CACHING DOM QERIES

Methods that find elements in the DOM tree are called DOM queries. When you need to work with an element more than once you should use a variable to store the result of this query.

When people talk about storing elements in variables, they are really storing the location of the element(s) within the DOM tree in a variable. The properties and methods of that element node work on the variable.


## ACCESSING ELEMENTS

DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.

Sometimes you will just want to access one individual element (or a fragment of the page that is stored within that one element). Other times you may want to select a group of element s, for example, every (hl) element in the page or every (li) element within a particular list.

Here, the DOM tree shows the body of the page of the list example. We focus on accessing elements first so it only shows element nodes. The diagrams in the coming pages highlight which elements a DOM query would return. (Remember, element nodes are the DOM representation of an element.)

* **GROUPS OF ELEMENT NODES**

If a method can return more than one node, it will always return a Nodelist, which is a collection of nodes (even if it only finds one matching element). You then need to select the element you want from this list using an index number (which means the numbering starts at 0 like the items in an array).

For example, several elements can have the same tag name, so get El ementsByTagName () will always return a Nodel i st.


* **FASTEST ROUTE**

Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive. This usually means evaluating the minimum number of nodes on the way to the element you want to work with. For example, getEl ementByld () will quickly return one element (because no two elements on the same page should have the same value for an id attribute), but it can only be used when the element you want to access has an id attribute.


## NODELISTS: DOM QUERIES THAT RETURN MORE THAN ONE ELEMENT

When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).


## SELECTING AN ELEMENT FROM A NODELIST

There are two ways to select an element from a Nodelist: The item() method and array syntax. Both require the index number of the element you want.

## SELECTING ELEMENTS USING CLASS ATTRIBUTES

The get El ementsByCl ass Name() method allows you to select elements whose c 1 ass attribute contains a specific
value. 

The method has one parameter: the class name which is given in quotes within the parentheses after the method name.

Because several elements can have the same value for their class attribute, this method always returns a Nodelist.

## SELECTING ELEMENTS BY TAG NAME

The get El ementsByTagName () method allows you to select elements using their tag name.

The element name is specified as a parameter, so it is placed inside the parentheses and is contained by quote marks.

Note that you do not include the angled brackets that surround the tag name in the HTML (just the letters inside the brackets).

## SELECTING ELEMENTS USING CSS SELECTORS

querySe 1 ector() returns the first element node that matches the CSS-style selector. querySe 1ectorA11 () returns a Nodelist of all of the matches.

Both methods take a CSS selector as their only parameter. The CSS selector syntax offers more flexibility and accuracy when selecting an element than

just specifying a class name or a tag name, and should also be familiar to front-end web developers who are used to targeting elements using CSS.

## TRAVERSING THE DOM

When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM.

* parentNode

* previousSibling nextSibling

* firstChild lastChild

## WHITESPACE NODES

Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between 
elements.

## ACCESS & UPDATE TEXT WITH TEXTCONTENT (& INN ERTEXT)

The textCon tent property allows you to collect or update just the text that is in the containing element (and its children).

**textContent**

To collect the text from the (li) elements in our example (and ignore any markup inside the element) you can use the
textContent property on the containing (li) element. In this case it would return the value: fresh figs.

You can also use this property to update the content of the element; it replaces the entire content of it (including any
markup).

**innerText**

You may also come across a property called i nner Text, but you should generally avoid it for three key reasons:

* SUPPORT

Although most browser manufacturers adopted the property, Firefox does not because i nnerText is not part of any standard.

* OBEYS CSS

It will not show any content that has been hidden by CSS. For example, if there were a CSS rule that hid the (em) elements, the innerText property would return only the word figs.

* PERFORMANCE

Because the i nnerText property takes into account layout rules that specify whether the element is visible or not, it can be slower to retrieve the content than the textContent property.

## ADDING ELEMENTS USING DOM MANIPULATION

DOM manipulation offers another technique to add new content to a page (rather than innerHTML). It involves three steps:

1. CREATE THE ELEMENT / createEl ement ()

2. GIVE IT CONTENT / createTextNode()

3. ADD IT TO THE DOM / appendChild()

## DEFENDING AGAINST CROSS-SITE SCRIPTING

### VALIDATE INPUT GOING TO THE SERVER

1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation. Do not allow untrusted users to submit HTML markup or JavaScript.

2. Double-check validation on the server before displaying user content/storing it in a database. This is important because users could bypass validation in the browser by turning JavaScript off.

3. The database may safely contain markup and script from trusted sources (e.g., your content management system). This is because it does not try to process the code; it just stores it.

### ESCAPE DATA COMING FROM THE SERVER & DATABASE

6. Do not create DOM fragments containing HTML from untrusted sources. It should only be added as text once it has been escaped.

5. Make sure that you are only inserting content generated by users into certain parts of the template files.

4. As your data leaves the database, all potentially dangerous characters should be escaped

## Summary

* The browser represents the page using a DOM tree.

* DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.

* You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.

* Whenever a DOM query can return more than one node, it will always return a Nadelist.

* From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.

* An element node can contain multiple text nodes and child elements that are siblings of each other.

* In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).

* Browsers offer tools for viewing the DOM tree .

# Understanding The Problem Domain Is The Hardest Part Of Programming

## What is the hardest thing about writing code?

There are many common answers to this question:

1. Learning a new technology
2. Naming things
3. Testing your code
4. Debugging
5. Fixing bugs
6. Making software maintainable
7. The list goes on and on.


## Why problem domains are hard

Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.

## What can you do about it?

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1. Make the problem domain easier
2. Get better at understanding the problem domain

* You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.

Games are really good at this.  Look at most games today and you’ll find that you start with a very small problem domain.The first level is usually a tutorial that has a basic set of things you can do so that you don’t get overwhelmed.  But, as you advance through the levels, you usually find they get harder and introduce new concepts that build gradually on what you know, until you understand a pretty large problem domain. 

The other choice is to become better at understanding problem domains. As developers, we tend to think that sitting down and talking to customers or business people who know about the problem domain is a waste of time. It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it. Best to resist the temptation to “not waste anymore time talking” and make sure you understand a problem inside and out before you try and solve it with code.  It is much more expensive and time consuming to do things over than it is to do them right the first time. I learn this lesson the hard way time and time again.

#THE END 
