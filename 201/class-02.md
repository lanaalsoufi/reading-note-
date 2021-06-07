<img src ="https://media.geeksforgeeks.org/wp-content/uploads/20191205185435/Untitled-drawing-61.png">


# Text

## Headings

**HTML has six "levels" of 
headings:**

* (h1) is used for main headings

* (h2) is used for subheadings

* If there are further sections under the subheadings then the (h3) element is used, and so on...

Browsers display the contents of headings at different sizes. The contents of an (h1) element is the largest, and the contents of an (h6) element is the smallest. The exact size at which each browser shows the headings can vary slightly Users can also adjust the size of text in their browser. You will see how to control the size of text, its color, and the fonts used when we come to look at CSS.


## Paragraphs

* To create a paragraph, surround the words that make up the paragraph with an opening tag and closing tag.

* By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.

## Superscript & Subscrip

* (sup)

The (sup) element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.

* (sub)

The (sub) element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

## Line Breaks & Horizontal Rules

* (br)

As you have already seen, the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag (br)

* (hr)
To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the (hr) tag.


## Strong & Emphasis


* (strong)

The use of the (strong) element indicates that its content has strong importance. For example, the words contained in 
this element might be said with strong emphasis. By default, browsers will show the contents of a (strong)element in bold.


* (em)
The (em) element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an (em) element in italic.

## Quotations

* (blockquote)

The (blockquote) element is used for longer quotes that take up an entire paragraph. Note how the (p) element is still used inside the (blockquote) element. Browsers tend to indent the contents of the (blockquote) element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS. 

* (q)

The (q) element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around 
the (q) element, however Internet Explorer does not — therefore many people avoid using the (q) element.


## Summary

* HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).

* They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation)



<img src ="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20191219190325/CSS5.png">


# **Introducing CSS**

CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.

## **Example Styles:**

 **Boxes :**

* Width and height 

* Borders (color, width, and style)

* Background color and images 

* Position in the browser window.

**Text :**

* Typeface

* Size

* Color

* Italics, bold, uppercase, lowercase, small-caps

**Specific :**

There are also specific ways in which you can style certain elements such as lists, tables, and forms.


## **CSS Associates Style rules with HTML elements**

CSS works by associating rules with HTML elements These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

* This rule indicates that all (p) elements should be shown in the Arial typeface. 

* **Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

* **Declarations** indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon


## **CSS Properties Affect How Elements Are Displayed**

CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.

* This rule indicates that all (h1), (h2) and (h3) elements should be shown in the Arial typeface, in a yellow color

* **Properties** indicate the aspects of the element you want to change. For example, color, font, width, height and border.

* **Values** specify the settings you want to use for the chosen properties. For example, if you want to specify a color property then the value is the color you want the text in these elements to be.


## **Using External CSS**

* ***link***

The (link) element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the (head) element. It should use three attributes:

1. href

This specifies the path to the CSS file (which is often placed in a folder called css or styles).

2. type

This attribute specifies the type of document being linked to. The value should be text/css.

3. rel

This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.


## **CSS Selectors**

1. Universal Selector

2. Type Selector

3. Class Selector

4. ID Selector

5. Child Selector

6. Descendant Selector

7. Adjacent Sibling Selector

8. General Sibling Selector


## **Summary**

* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.

* Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).

* Different types of selectors allow you to target your 
rules at different elements.

* Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.

* CSS rules usually appear in a separate document although they may appear within an HTML page.


<img src ="https://www.geeksforgeeks.org/wp-content/uploads/javascript-768x256.png">


# Basic JavaScript Instructions

## STATEMENTS

A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 

## COMMENTS 

You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code. 

**MULTI-LINE COMMENTS**

* To write a comment that stretches over more than one line, you use a multi-line comment, starting with the /* characters and ending with the */ characters. Anything between these characters is not processed· by the JavaScript interpreter 

* Multi-line comment s are often used for descriptions of how the script works, or to prevent a section of the script from running when testing it.


**SINGLE-LINE COMMENTS**

* In a single-line comment, anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter. Singleline comments are often used for short descriptions of what the code is doing. 

* Good use of comments will help you if you come back to your code after several days or months. They also help those who are new to your code. 


## WHAT IS A VARIABLE? 

A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

A variable is a good name for this concept because the data stored in a variable can change (or vary) each time a script runs. 

* No matter what the dimensions of any individual wall are, you know that you can find its area by multiplying the width of that wall by its height. Similarly, scripts often need to achieve the same goal even when they are run with different data, so variables can be used to represent values in your scripts that are likely to change. The result is said to be calculated or computed using the data stored in the variables.

* The use of variables to represent numbers or other kinds of data is very similar to the concept of algebra (where 
letters are used to represent numbers). There is one key difference, however. The equals sign does something very different in programming (as you will see on the next two pages). 

## Variable: How to declare them

Before you can use a variable, you need to announce that you want to use it. This involves creating the variable and giving it a name. Programmers say that you declare the variable.


## Variable: How to assign them a value

Once you have created a variable, you Can tell it what information you would like it to store for You. Programmers say that You Assign a value to the Variable.


## DATA TYPES

JavaScript distinguishes between numbers, strings, and true or false values known as Booleans. 

**NUMERIC DATA TYPE**

The numeric data type handles numbers. 

**STRING DATA TYPE**

The strings data type consists of letters and other characters.

**BOOLEAN DATA TYPE**

Boolean data types can have one of two values: true or false. 

## ARRAYS 

An array is a special type of variable. It doesn't just store one value; it stores a list of values. 

## VALU ES IN ARRAYS 

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 

* NUMBERING ITEMS IN AN ARRAY 

Each item in an array is automatically given a number called an index. This can be used to access specific items in the array.

* ACCESSING ITEMS IN AN ARRAY 

To retrieve the third item on the list, the array name is specified along with the index number in square brackets.

* NUMBER OF ITEMS IN AN ARRAY 

Each array has a property called length, which holds the number of items in the array. 


## EXPRESSIONS 

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions. 

1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE

2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE

## OPERATORS

Expressions rely on things called operators; they allow programmers to create a single value from one or more values. 


## SUMMARY

* A script is made up of a series of statements. Each statement is like a step in a recipe. 

* Scripts contain very precise instructions. For example, you might specify that a value must be remembered before creating a calculation using that value. 

* Variables are used to temporarily store pieces of information used in the script. 

* Arrays are special types of variables that store more than one piece of related information.

* JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false). 

* Expressions evaluate into a single value.

* Expressions rely on operators to calculate a value. 


# Decisions and Loops

## DECISION MAKING

There are often several places in a script where decisions are made that determine which lines of code should be run next. Flowcharts can help you plan for these occasions.

## COMPARISON OPERATORS:

 ***EVALUATING CONDITIONS***

You can evaluate a situation by comparing one value in the script to what you expect it might be. The result will be a Boolean : true or false. 

**(==) IS EQUAL TO** 

This operator compares two values (numbers, strings, or Booleans ) to see if they are the same.

**(!=) IS NOT EQUAL TO**

This operator compares two values (numbers, strings, or Booleans ) to see if they are not the same.

**(===) STRICT EQUAL TO**

This operator compares two values to Check that both the data type and value are the same. 

**(!===) STRICT NOT EQUAL TO**

This operator compares two values to Check that both the data type and value are not the same.

**(>) GREATER THAN**

This operator checks if the number on the left is greater than the number on the right.

**(<) LESS THAN**

This operator checks if the number on the left is less than the number on the right.

**(>=) GREATER THAN OR EQUAL TO**

This operator checks if the number on the left is greater than or equal to the number on the right.

**(<=) LESS THAN OR EQUAL TO**

This operator checks if the number on the left is less than or equal to the number on the right.


## LOGICAL OPERATORS

Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison operator.

**(&&) LOGICAL AND**

This operator tests more than one condition.

**(||) LOGICAL OR**

This operator tests at least one condition.

**(!) LOGICAL NOT**

This operator takes a single Boolean value and inverts it.


## IF STATEMENTS 

The if statement evaluate ( or checks ) a condition. If the condition evaluates to true, any statements in the subsequent code block are executed.

## IF...ELSE STATEMENTS

The If...else statement checks a condition. If it resolves to true the first code block is executed. If the condition resolves to false the second code block is run instead.


# THE END