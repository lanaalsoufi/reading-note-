# LISTS

There are lots of occasions when we need to use lists. HTML provides us with three different types:

*  Ordered lists are lists where each item in the list is numbered. For example the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.

* Unordered lists are lists that begin with a bullet point (rather than characters that indicate order).

* Definition lists are made up of a set of terms along with the definitions for each of those terms.

## Ordered Lists

(ol)

The ordered list is created with the (ol) element.

(li)

Each item in the list is placed between an opening (li) tag and a closing (li) tag. (The listands for list item.)

## Unordered Lists

(ul)

The unordered list is created with the (ul) element.

(li)

Each item in the list is placed between an opening (li) tag and a closing (li) tag. (The listands for list item.)

## Definition Lists

(dl)

The definition list is created with the (dl) element and usually consists of a series of terms and their definitions.Inside the (dl) element you will usually see pairs of (dt) and (dd) elements.

(dt)

This is used to contain the term being defined (the definition term).

(dd)

This is used to contain the definition.

## Summary 

* There are three types of HTML lists: ordered, unordered, and definition. 

*  Ordered lists use numbers.

*  Unordered lists use bullets.

* Definition lists are used to define terminology.

* Lists can be nested inside one another.


# BOXES

## Border, Margin & Padding

Every box has three available properties that can be adjusted to control its appearance:

1. Border

Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another

2. Margin

Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

3. Padding

Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

## White space & Vertical Margin

The padding and margin properties are very helpful in adding space between various items on the page


## Change Inline/Block display

The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.The values this property can take are:

* inline

This causes a block-level element to act like an inline element.

* block

This causes an inline element to act like a block-level element.inline-block
This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

* none

This hides an element from the page. In this case, the element acts as though it is not on the page at all (although a user could still see the content of the box if they used the view source option in their browser).



## CSS3: Box Shadows box-shadow

The box-shadow property allows you to add a drop shadow around a box. It works just like the text-shadow property that you met on page 288. It must use at least the first of these two values as well as a color:

* Horizontal offset

Negative values position the shadow to the left of the box.

* Vertical offset

Negative values position the shadow to the top of the box.

* Blur distance

If omitted, the shadow is a solid line like a border.

* Spread of shadow

If used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract.

The inset keyword can also be used before these values to create an inner-shadow.


## CSS3: Elliptical Shapes border-radius

To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners.

## Summary

* CSS treats each HTML element as if it has its own box. 

* You can use CSS to control the dimensions of a box.

* You can also control the borders, margin and padding for each box with CSS.

* It is possible to hide elements using the display and visibility properties.

* Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.

* Legibility can be improved by controlling the width of boxes containing text and the leading.

* CSS3 has introduced the ability to create image borders and rounded borders.


# Basic JavaScript Instructions

## ARRAYS

An array is a special type of variable. It doesn't just store one value; it stores a list of values. 

## VALUES IN ARRAYS

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 

* NUMBERING ITEMS IN AN ARRAY 

* ACCESSING ITEMS IN AN ARRAY

* NUMBER OF ITEMS IN AN ARRAY

# Decisions and Loops

## IF...ELSE STATEMENTS

The If...else statement checks a condition. If it resolves to true the first code block is executed. If the condition resolves to false the second code block is run instead.


## SWITCH STATEMENTS

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 

## TYPE COERCION & WEAK TYPING 

If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error. 


* JavaScript can convert data types behind the scenes to complete an operation.This is known as type coercion. For example, a string 'l ' could be converted to a number 1 in the following expression:(' 1' > 0). As a result, the above expression would evaluate to true. 

* JavaScript is said to use weak typing because the data type for a value can change. Some other languages require that you specify what data type each variable will be. They are said to use strong typing. 

* Type coercion can lead to unexpected values in your code (and also cause errors). Therefore, when checking if two values are equal, it is considered better to use strict equals operators ===and ! == rather than == and ! = as these strict operators check that the value and data types match. 

## TRUTHY & FALSY VALUES

Due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects. 

* Falsy values are treated as if they are fa 1 se. The table to the left shows a hi ghScore variable with a series of values, all of which are falsy. 

Falsy values can also be treated as the number 0 . 

* Truthy values are treated as if they are true. Almost everything that is not in the falsy table can be treated as if it were true. 

Truthy values can also be treated as the number 1. 

## LOOPS

Loops check a condition. If It returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. 

## ***There are three common types of loops :***

**FOR**

If you need to run code a specific number of times, use a for loop. ( it is the most common loop). In a for loop, the condition is usually a counter which is used to tell how many times the loop should run.

**WHILE**

If you do not know how many times the Code should run, you Can use a while loop. Here the condition can be something other than a counter, and the code will continue to loop for as long as the condition is true.

**DO WHILE**

The do... while loop is very similar to the while loop, but has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to false.

## LOOP COUNTERS

A for loop uses a counter as a condition. This instructs the code to run a specified number of times. Here you Can see the condition is made up of three statements:

**INITIALIZATION**

Create a variable and set it to 0. This is variable is commonly called i, and it acts as the counter.

Var i = 0;

**CONDITION**

The loop should continue to run until the Counter reaches a specified number.

i < 10;

**UPDATE**

Every time the loop has run the statements in the curly braces, it adds one to the counter.

i++


# **USING WHILE LOOPS**

c04/ js/while-1oop.js 

var i = l ;     //Set counter to 1 

var msg = ' ' ; //Message 

// Store 5 times table in a variable 

while (i < 10) { 

msg += i + ' x 5 = ' + (i * 5) + '<br />'; 

i++; 

document .getElementByid( ' answer') . innerHTML = msg; 

* Here is an example of awhile loop. It writes out the 5 times table. Each time the loop is run, another calculation is written into the variable called msg. 

* This loop will continue to run for as long as the condition in the parentheses is true. That condition is a counter indicating that, as long as the variable i remains less than 10, the statements in the subsequent code block should run.

* Inside the code block there are two statements: 

1. The first statement uses the+= operator, which is used to add =new content to the msg variable. Each time the loop runs a new calculation and line break is added to the end of the message being stored in it. So+" works as a shorthand for writing: msg = msg + 'new msg' (See bottom of the next page for a breakdown of this statement.) 

2. The second statement increments the counter variable by one. (This is done inside the loop rather than with the condition.)

* When the loop has finished, the interpreter goes to the next line of code, which writes the msg variable to the page. 

* In this example, the condition specifies that the code should run nine times. A more typical use of awhi le loop would be when you do not know how many times you want the code to run It should continue to run as long as a condition is met. 


## Summary

* Conditional statements allow your code to make decisions about what to do next. 

* Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>) are used to compare two operands.

* Logical operators allow you to combine more than one set of comparison operators. 

* if ... else statements allow you to run one set of code if a condition is true, and another if it is false. 

* switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match). 

* Data types can be coerced from one type to another. 

* All values evaluate to either truthy or falsy. 

* There are three types of loop: for, while, and do ... while. Each repeats a set of statements.