# **Chapter (10)**

## ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:

This script above creates a greeting message, then writes it to an alert box (see right-hand page). In order to create that greeting, two functions are used:
greetUser () and getName () .

You might think that the order of execution (the
order in which statements are processed) would be
as numbered: one through to four. However, it is a
little more complicated.

## EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context there are two phases of activity:

**1. PREPARE**

• The new scope is created

• Variables, functions, and arguments are created

• The value of the this keyword is determined

**2. EXECUTE**

• Now it can assign values to variables

• Reference functions and run their code

• Execute statements


## UNDERSTANDING SCOPE

In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object

Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the current execution context's variables object, plus the
variables object for each parent execution context.

## ERROR OBJECTS CONTINUED

* **Syntax Error**    
SYNTAX IS NOT CORRECT

This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.

* **Reference Error**  
VARIABLE DOES NOT EXIST

This is caused by a variable that is not declared or is
out of scope.

## HOW TO DEAL WITH ERRORS

Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.

1. DEBUG THE SCRIPT TO FIX ERRORS

If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.

You will find that the developer tools available in
every major modern browser will help you with this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)


2. HANDLE ERRORS GRACEFULLY

You can handle errors gracefully using try, catch,
throw, and finally statements.

Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.

## A DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error. Here is a workflow for techniques you will meet over the next 20 pages. Try to narrow down where the problem might be, then look for clues.

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.


## HANDLING EXCEPTIONS

If you know your code might fail, use try, catch, and finally. Each one is given its own code block.

* **TRY**

First, you specify the code that you t hink might throw an exception within the try block.

If an exception occurs in this section of code, control is automatically passed to the corresponding catch block.

The try clause must be used in this type of error handling code, and it should always have either a catch, fi na 1 ly, or both.

If you use a continue, break, or return keyword inside a try, it will go to the fina11 y option.


* **CATCH**

If the try code block throws an exception, catch steps in with an alternative set of code.

It has one parameter: the error object. Although it is optional, you are not handling the error if you do not catch an error.

The ability to catch an error can be very helpful if there is an issue on a live website.

It lets you tell users that something has gone wrong (rather than not informing them why the site stopped working).


* **FINALLY**

The contents of the fina11y code block will run either
way - whether the try block succeeded or failed.

It even runs if a return keyword is used in the try or catch block. It is sometimes used to clean up after the previous two clauses.

These methods are similar to the .done(), . fail() , and. a1ways() methods in jQuery.

You can nest checks inside each other (place another 
try inside a catch), but be aware that it can affect performance of a script.


## THROW ERROR FOR NaN

If you try to use a string in a mathematical operation (other than in addition), you do not get an error, you get a special value called NaN (not a number).

## Summary

* If you understand execution contexts (which have two
stages) and stacks, you are more likely to find the error in your code.

* Debugging is the process of finding errors. It involves a process of deduction.

* The console helps narrow down the area in which the
error is located, so you can try to find the exact error.

* JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

# THE END