# ***HTML & CSS***
# Introduction

## the Web Works

When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.
 

 1. When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site; for example: google.com, bbc.co.uk, microsoft.com.

2. Your computer contacts a network of servers called Domain Name System (DNS) 
servers. These act like phone books; they tell your computer the IP address
associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer.

3. The unique number that the DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users

4. The web server then sends the page you requested back to your web browser.

# Structure

## HTML Describes the Structure of Pages

The HTML code is made up of characters that live inside angled brackets — these are called HTML elements. Elements are usually made up of two tags: an opening tag and a closing tag. (The closing tag has an extra forward slash in it.) Each HTML element tells the browser something about the information that sits between its opening and closing tags .

## Attributes Tell Us More About Elements

Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.


* body : 

Everything inside this element isshown inside the main browserwindow.

* head :


This contains informationabout the page (rather thaninformation that is shown within the main part of the browser window that is highlighted in blue on the opposite page). You will usually find a title element inside the head element

* Title :

The contents of this element are either shown in the top of the browser, above where you usually type in the URL of the page you want to visit, or on the tab for that page (if your browser uses tabs to allow you
to view multiple pages at the same time). 

## Creating a Web Page on a PC

1. Start All Programs (or Programs) Accessories Notepad, You might also like to download a free editor called Notepad++ from notepad-plus-plus.org.

2. Type the code shown on the right

3. Go to the File menu and select Save as... You will need to save the file somewhere you can remember. If you like, you could create a folder for any examples that you try out from this book. Save this file as first-test.
html. Make sure that the Save as type drop down has All Files selected.

4. Start your web browser. Go to the File menu and select Open. Browse to the file that you just created, select it and click on the Open button. The result should look something like the screen shot to the left.


## Summary 

- HTML Pages ages are text documents.

- HTML uses tags (characters that sit inside angled
brackets) to give the information they surround special
meaning.

- Tags are often referred to as elements.

- Tags usually come in pairs. The opening tag denotes
the start of a piece of content; the closing tag denotes
the end.

- Opening tags can carry attributes, which tell us more
about the content of that element.

- Attributes require a name and a value.

- To learn HTML you need to know what tags are
available for you to use, what they do, and where they
can go.


# Extra Markup

## DOCTYPEs

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included). 
We will therefore be including one in each example for the rest of the book.

## Comments in HTML

If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters: (!-- --)

It is a good idea to add comments to your code because, no matter how familiar you are with the page at the time of writing it, when you come back to it later (or if someone else needs to look at the code), comments will make it much easier to understand.

Although comments are not visible to users in the main browser window, they can be viewed by anyone who looks at the source code behind the page. On a long page you will often see comments used to indicate where sections of the page start or end, and to pass on notes to help anyone who is looking at the code understand it.

Comments can also be used around blocks of code to stop that code from being displayed in the browser. In the example on the left, the email link has been  commented out.

## ID Attribute

Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character).It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique).

## Class Attribute

Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other 
pages on your own site and links that point to external sites. 

## Block Elements

Some elements will always appear to start on a new line in the browser window. These are known as block level elements.

## Inline Elements

Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements.

## Escape Characters

There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.)

* Less-than sign <

* Greater-than sign >

* Ampersand &

* Quotation mark "

* Multiplication sign (*)

* Division sign /

## Summary

* DOCTYPES tell browsers which version of HTML you are using.

* You can add comments to your code between the (!-- and --) markers.

* The id and class attributes allow you to identify particular elements.

* The (div) and (span) elements allow you to group block-level and inline elements together.

* (iframes) cut windows into your web pages through which other pages can be displayed.

* The (meta) tag allows you to supply all kinds of information about your web page.

* Escape characters are used to include special characters in your pages such as <, >, and ©.

# HTML5 Layout

## Headers & Footers

The header and footer elements can be used for:

* The main header or footer that appears at the top or bottom of every page on the site.

* A header or footer for an individual article or section within the page.

## Navigation

* The nav element is used to contain the major navigational blocks on the site such as the primary site navigation.

* Going back to our blog example, if you wanted to finish an article with links to related blog posts, these would not be counted as major navigational blocks and therefore should not sit inside a nav element.

* At the time of writing, some of the developers that were already using HTML5 decided to use the nav element for the links that appear at the bottom of every page (links to things like privacy policy, terms and conditions and accessibility information). Whether this will be widely adopted is still yet to be seen

**Articles**

* The article element acts as a container for any section of a page that could stand alone and potentially be syndicated.

* This could be an individual article or blog entry, a comment or forum post, or any other independent piece of content.


* If a page contains several articles (or even summaries of several articles), then each individual article would live inside its own article element.


* The article elements can even be nested inside each other. For example, a blog post might live inside one article element and each comment on the article could live inside its own child article element.



1. The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.


2. The new elements provide clearer code (compared with using multiple div elements).


3. Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.

4. To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.


## Sections

The (section) element groups related content together, and typically each section would have its own heading

## Heading Groups

The purpose of the (hgroup) element is to group together a set of one or more (h1) through (h6) elements so that they are treated as one single heading. 

## Summary 

* The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.

* The new elements provide clearer code (compared with using multiple <div> elements).

* Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.

* To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

# Process & Design

## WireFrames


A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.


* lot of designers will take the elements that need to appear on each page and start by creating wireframes. This involves sketching or shading areas where each element of the page will go (such as the logo, primary navigation, headings and main bodies of text, user logins etc).

* By creating a wireframe you can ensure that all of the information that needs to be on a page is included.


* You should not include the color scheme, font choices, backgrounds or images for the website in the wireframe. It should focus on what information needs to be on each page and create a visual hierarchy to indicate the most important parts of each page


* The wireframes make design easier because you know what information needs to appear on which page before considering


* how the the page should look. It can be very helpful to show the wireframes of a site to a client before showing them a design. It enables the client to ensure the site has all the functions and information it needs to offer.


* If you just present a site design to a client, it is common for them to focus on how the site looks, which means they may not raise issues about its function after the site has been built.

## Visual hierarchy

* SIZE

Larger elements will grab users' attention first. For this reason it is a good idea to make headings and key points relatively large.

* COLOR

Foreground and background color can draw attention to key messages. Brighter sections tend to draw users' attention first.

* Style
An element may be the same size and color as surrounding content but have a different style applied to it to make it stand out.

## Designing Navigation

* Concise

Ideally, the navigation should be quick and easy to read. It is a good idea to try to limit the number of options in a menu to no more than eight links. These can link to section homepages which in turn link to other pages.

* Clear

Users should be able to predict the kind of information that they will find on the page before clicking on the link. Where possible, choose single descriptive words for each link rather than phrases.

* Selective

The primary navigation should only reflect the sections or content of the site. Functions like logins and search, and legal information like terms and conditions and so on are best placed elsewhere on the page.

## Summary

* It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.

* Site maps allow you to plan the structure of a site.

* Wireframes allow you to organize the information that will need to go on each page.

* Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.

* You can differentiate between pieces of information using size, color, and style. 

* You can use grouping and similarity to help simplify the information you present.


# ***JAVASCRIPT & JQUERY***

# Introduction

## HOW JAVASCRIPT MAKES WEB PAGES MORE INTERACTIVE

1. ACCESS CONTENT

You can use JavaScript to select any element attribute, or text from an HTML page. For example: 

* Select the text inside all of the hl 
elements on a page 

* Select any elements that have a class attribute with a value of note 

* Find out what was entered into a text input whose id attribute has a value of email 


2. MODIFY CONTENT

You can use JavaScript to add elements attributes, and text to the page, or remove them. For example: 

* Add a paragraph of text after the first hl element 

* Change the value of class attributes to trigger new CSS rules for those elements 

*  Change the size or position of an img element


3. PROGRAM RULES

You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page. For example: 

* A gallery script could check which image a user clicked on and display a larger version of that image.

* A mortgage calculator could collect values from a form, perform a calculation and display repayments.

* An animation could check the dimensions of the browser window and move an image to the bottom of the viewable area (also known as the viewport). 


4. REACT TO EVENTS 

You can specify that a script should run when a specific event has occurred. For example, it could be run when:

* A button is pressed 

* A link is clicked (or tapped) on

* A cursor hovers over an element 

* Information is added to a form 

* An interval of time has passed

* A web page has finished loading 

# The ABC of Programming

## WHAT IS A SCRIPT AND HOW DO I CREATE ONE ?

* A script is a series of instructions that a computer can follow to achieve a goal.

* Each time the script runs, it might only use a subset of all the instructions. 

* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically. 

* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help).

## Summary

* A script is a series of instructions that the computer can follow in order to achieve a goal. 

* Each time the script runs, it might only use a subset of all the instructions. 

* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically. 

* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 


## HOW DO COMPUTERS FIT IN WITH THE WORLD AROUND THEM ?

### OBJECTS & PROPERTIES

If you could not see the picture of the hotel and cars, the data in the 
information boxes alone would still tell you a lot about this scene. 

**OBJECTS (THINGS)**

* In computer programming, each physical thing in the world can be represented as an object. There are two different types of objects here: a hotel and a car.

* Programmers might say that there is one instance of the hotel object, and two instances of the car object.

* Each object can have its own: 
1. Properties 
2. Events 
3. Methods 

Together they create a working model of that object. 


**PROPERTIES (CHARACTERISTICS)**

* Both of the cars share common characteristics. In fact, all cars have a make, a color, and engine size. You could even determine their current speed. Programmers call these characteristics the properties of an object.

* Each property has a name and a value, and each of these name/value pairs tells you something about each individual instance of the object. 

* The most obvious property of this hotel is its name. The value for that property is Quay. You can tell the number of rooms the hotel has by looking at the value next to the rooms property.


## EVENTS

* WHAT IS AN EVENT? 

There are common ways in which people interact with each type of object. For example, in a car a driver will typically use at least two pedals. The car 
has been designed to respond differently when the driver interacts with each of the different pedals: 

• The accelerator makes the car go faster 
• The brake slows it down 

## METHODS 

* WHAT IS A METHOD? 

Methods typically represent how people (or other things) interact with an object in the real world. 

They are like questions and instructions that: 
• Tell you something about that object (using information stored in its properties) 
• Change the value of one or more of that object's properties

## HOW DO I WRITE A SCRIPT FOR A WEB PAGE ?

### Summary

* It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension. 

* The HTML (script) element is used in HTML pages to tell the browser to load the JavaScript file (rather like 
the (link) element can be used to load a CSS file). 

* If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web 
page that the browser has created. 


# THE END