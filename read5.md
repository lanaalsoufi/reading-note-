<img src ="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSi1GVyeklIQE3uwsx9ud3XIrZK4slTbpkd9w&usqp=CAU">

# **COMPARISON OPERATORS:**
## ***EVALUATING CONDITIONS***

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


# **LOGICAL OPERATORS**

Comparison operators usually return single values of true or false. Logical operators allow you to compare the results of more than one comparison operator.

**(&&) LOGICAL AND**

This operator tests more than one condition.

**(| |) LOGICAL OR**

This operator tests at least one condition.

**(!) LOGICAL NOT**

This operator takes a single Boolean value and inverts it.


<img src ="https://devtutorialspoint.com/wp-content/uploads/2020/11/introduction-to-javascript-11-780x470.png">


# **LOOPS**

Loops check a condition. If It returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. 

## ***There are three common types of loops :***

**FOR**

If you need to run code a specific number of times, use a for loop. ( it is the most common loop). In a for loop, the condition is usually a counter which is used to tell how many times the loop should run.

**WHILE**

If you do not know how many times the Code should run, you Can use a while loop. Here the condition can be something other than a counter, and the code will continue to loop for as long as the condition is true.

**DO WHILE**

The do... while loop is very similar to the while loop, but has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to false.


# **LOOP COUNTERS**

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














