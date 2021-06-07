# **Chapter (6)**

# TABLES

## What's a Table?

A table represents information in a grid format Examples of tables include financial reports, TV schedules, and sports results.

## Basic Table Structure

* table

The table element is used to create a table. The contents of the table are written out row by row.

* tr

You indicate the start of each row using the opening tr tag. (The tr stands for table row.)

It is followed by one or more td elements (one for each cell in that row).

At the end of the row you use a closing tr tag.

* td

Each cell of a table is represented using a td element. (The td stands for table data.) At the end of each cell you use a closing td tag.

## Table Headings

* th

The th element is used just like the td element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)

Even if a cell has no content, you should still use a td or th element to represent the presence of an empty cell otherwise the table will not render correctly (The first cell in the first row of this example shows an empty cell.)

Using th elements for headings helps people who use screen readers, improves the ability for search engines to index your pages, and also enables you to control the appearance of tables better when you start to use CSS.

You can use the scope attribute on the th element to indicate whether it is a heading for a column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column.


## Long Tables

There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content).

These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table (as you will see when you learn about CSS).

* thead

The headings of the table should sit inside the thead element.

* tbody

The body should sit inside the tbody element.

* tfoot

The footer belongs inside the tfoot element.

## Summary

* The table element is used to add tables to a web page.

* A table is drawn out row by row. Each row is created with the tr element.

* Inside each row there are a number of cells represented by the td element (or th if it is a header)

* You can make cells of a table span more than one row or column using the rowspan and colspan attributes.

* For long tables you can split the table into a thead, tbody, and tfoot.

# **Chapter (3)**

# Functions, Methods, and Objects

## CREATING MANY OBJECTS: CONSTRUCTOR NOTATION

Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects. First, create the template with the object's properties and methods.

## RECAP: WAYS TO CREATE OBJECTS

* CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS

* CREATING AN OBJECT WITH PROPERTIES & METHODS

## THIS (IT IS A KEYWORD)

The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates.

* A FUNCTION IN GLOBAL SCOPE

When a function is created at the top level of a (that is, not inside another object or function), then it is in the global scope or global context.

The default object in this context is the window object. so when this is used inside a function in the global context it refers to the window object.

* GLOBAL VARIABLES

All global variables also become properties of the window object. so when a function is in the global context, you can access global variables using the window object, as well as its other properties.

Here, the showWidth () function is in global scope, and this.width refers to the width variable

* A METHOD OF AN OBJECT

When a function is defined inside an object, it becomes a method. In a method, this refers to the containing object.

* FUNCTION EXPRESSION AS METHOD

If a named function has been defined in global scope, and it is then used as a method of an object, this refers to the object it is contained within.

## RECAP: STORING DATA

In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.

* VARIABLES

A variable has just one key (the variable name) and one value.

* ARRAYS

Arrays can store multiple pieces of information. Each piece of information is separated by a comma. The order of the values is important because items in an array are assigned a number (called an index).

If you want to access items via a property name or key, use an object (but note that each key in the object must be unique). if the order of the items is important, use an array.

* INDIVIDUAL OBJECTS

Objects store sets of name/value pairs. They can be properties (variables) or methods (functions).

* MULTIPLE OBJECTS

When you need to create multiple objects within the same page, you should use an object constructor to provide a template for the objects.

## WHAT ARE BUILT-IN OBJECTS?

Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.

## DATA TYPES REVISITED

In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).

1. String
2. Number
3. Boolean
4. Undefined
5. Null
6. Object

## Summary

* Functions allow you to group a set of related statements together that represent a single task.

* Functions can take parameters (information) required to do their job) and may return a value.

* An object is a series of variables and functions that represent something from the world around you.

* In an object, variables are known as properties of the object; functions are known as methods of the object.

* Web browsers implement objects that represent both the browser window and the document loaded into the
browser window.

* JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.

* Arrays and objects can be used to create complex data
sets (and both can contain the other).

# Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## Define a constructor and initialize properties

To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.


This is **object-oriented programming** in JavaScript at its most fundamental level.

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.

## Generate random numbers

To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

**Here's some tips to follow when building your own domain models.**

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.

2. Model its attributes with a constructor function that defines and initializes properties.

3. Model its behaviors with small methods that focus on doing one job well.

4. Create instances using the new keyword followed by a call to a constructor function.

5. Store the newly created object in a variable so you can access its properties and methods from outside.

6. Use the this variable within methods so you can access the object's properties and methods from inside.


# **THE END**