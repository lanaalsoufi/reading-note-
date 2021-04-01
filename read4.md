# ***JAVASCRIPT & JQUERY***


## **HOW JAVASCRIPT MAKES WEB PAGES MORE INTERACTIVE** 

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


### **WHAT IS A SCRIPT AND HOW DO I CREATE ONE ?**

* A script is a series of instructions that a computer can follow to achieve a goal.

* Each time the script runs, it might only use a subset of all the instructions. 

* Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically. 

* To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help).


### **EXPRESSIONS**

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions.

1. EXPRESSIONS THAT JUST ASSIGN A 
VALUE TO A VARIABLE

* In order for a variable to be useful, it needs to be given a value. As you have seen, this is done using the assignment operator (the equals sign). var color = 'beige'; The value of co 1 or is now beige. 

* When you first declare a variable using the var keyword, it is given a special value of undefined This will change when you assign a value to it Technically, undefined is a data type like anumber string, or Boolean

2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE 

* You can perform operations on any number of individual values (see next page) to determine a single value. For example: var area = 3 * 2; The value of area is now 6. 

* Here the expression 3 * 2 evaluates into 6. This example also uses the assignment operator, so the result of the expression 3 * 2 is stored in the variable called area. 

* Another example where an expression uses two values to yield a single value would be where two strings are joined to create a single string. 


### **OPERATORS**

Expressions rely on things called operators; they allow programmers to create a single value from one or more values.

**ARITHMETIC OPERATORS**

JavaScript contains the following mathematical operators, which you can use with numbers.


var subtotal (13 + 1) * 5; // Subtotal is 70 

var shipping 0.5 * (13 + 1) ; // Shipping is 7 

var total subtotal + shipping ; // Total is 77 

var el Sub document .getElementByid(' subtotal' elSub .textContent =subtotal ;

var elShip = document .getElement Byid('shipping');elShip.textContent =shipping; 

var elTotal = document .getElementByid('total');elTotal .textContent =total; 

* This example demonstrates how mathematical operators are used with numbers to calculate the combined values of two costs. 

* The first couple of lines create two variables: one to store the subtotal of the order, the other  to hold the cost of shipping the order; so the variables are named accordingly: subtotal and shipping. 

* On the third line, the total is calculated by adding together these two values. 

* This demonstrates how the mathematical operators can use variables that represent numbers. (That is the numbers do not need to be written explicitly into the code.)

* The remaining six lines of code write the results to the screen. 
 

 **STRING OPERATOR**

 There is just one string operator: the+ symbol. It is used to join the strings on either side of it. 


## **WHAT IS A FUNCTION?**

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

*DECLARING A FUNCTION*

To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a function declaration. 


***CALLING A FUNCTION***

Having declared the function, you can then execute all of the statements between its curly braces with just one line of code. This is known as Calling the function.


***DECLARING FUNCTIONS THAT NEED INFORMATION***

Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it parameters. Inside the function, the parameters act like variables .


***CALLING FUNCTIONS THAT NEED INFORMATION***

When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name . The values are called arguments, and they can be provided as values or as variables.


***GETTING A SINGLE VALUE OUT OF A FUNCTION***

Some functions return information to the code that called them. For example, when they perform a calculation, they return the result.


# ***THE END***



