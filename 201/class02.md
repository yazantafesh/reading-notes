# Duckett HTML Book

### Chapter 2

This chapter talks about different types of text that can be written into a webpage and the different tags used for different types starting with headings starting from 1 and going down, and then paragraphs. Bold and italic tags, superscript and subscript.
Browsers treat multiple spaces as one space always which is called "white space collapsing".
Line breaks and horizontal rules are used to create spaces when needed using br and hr tags.
Visual editors make it easier to type code because it showcases the results on the other half of the screen live as the code is being written.
blockquote and q are used for quotations.
abbr tag is used for abbreviations and acronyms.
cite and dfn are used for citations and definitions.
address tag will usually display its contents in italics.


### Chapter 10

This part gives an introduction about CSS and it's relationship with HTML, CSS helps control and modify the HTML elements already existing and make them more appealing to the user's eyes.
A CSS rule contains a selector and a declaration. p{font-family: Arial;}.
CSS file can be linked to HTML file by <link href="" type="text/css" rel="stylesheet">
or it can be internal withing the HTML file.
Different types of selectors help target different rules and elements.
Declarations have two parts: properties and the values of these properties.

# Duckett JS Book:

### Chapter 2

This chapter starts with explaining what a statements is which is the main component of a script and then explains comments which are part of the code that is not executed and is used to help any code reader understand what is happening. Also a variable is what is used to store a certain value that will be used in different functions and operations.
To declare a variable we must use var or let or any other declaration words then the variable name and then the value wanted for that variable.
There are 3 data types; numeric, string and boolean.
There are multiple ways to declare variables; they can be declared and assigned a value in the same statement or all declared in the same line then assigned variables separately or maybe declared and assigned values on the same line.
after a variable is created you can just change its value by using its name.

Rules for naming variables:

- must begin with a dollar sign or a letter or underscore
- cant use dash or dot
- cant use keywords or reserved words
- variable names are case sensitive
- use descriptive names
- use camel case writing

An array is used to store multiple values.
items in an array are numbered starting from 0, and the number of items in an array is called length.

Then we start talking about comparison operators, they are used to compare a value in the script to the value you might expect it to be and it will give you a boolean result.

(==) is equal to. which compares two values
(===) strict equal to. compares both data type and value
(!=) is not equal to. compares two values to see if they are **not** the same
(!==) strict not equal to. compares both values and data types to check if they are **not** the same
(>) greater than
(<) less than
(>=) greater than or equal to
(<=>) less than or equal to

logical operators allow the comparison of the results of more than one comparison operator.

((5<2) && (2>=3)) do both expressions evaluate to true? no? then it will give out false

&& Logical and
|| Logical or
! Logical not  !true condition returns false and vice versa

### Chapter 4

This chapter talks about decision making and loops. Decision making and understanding the steps involved in a script is extremely important to get the code to work.
Decisions compose of a condition and an evaluation of the condition, and evaluations can be done using comparison operators to compare a value in the script to what it is expected to be.
expressions are often enclosed in brackets and have two operands with an operator in between.
operands do not have to be single values, they can be an expression each.
Comparison operators usually return true or false values and logical operators allow us to compare the results of more than one comparison operator. && is a logical and; || is a logical or; ! is a logical not.
If statemets checks a condition and if it is true, the code block inside will be executed. And else is used to execute another code block if the condition is false.