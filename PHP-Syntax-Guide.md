Challenge2 PHP Syntax Guide - Solomon Butler

PHP COMMENTS:

PHP allows single and multi-line comments.

// This is an example of a single like comment.

/_ This is an example of a multi-line comment _/

Comments allow the creator to explain their code without it affecting or interfering with the functionality.

PHP VARIABLES:

PHP variables are used for storing information.

PHP variables are written as follows:
$solomon = "Sol is my name";

- where $solomon, is the variables name,
- "Sol is my name", is the value held my the variable,
- and ; is the closing tag.
  Variables can hold numerical values, as well as text.

Variable names are case sensitive.

Variable names must start with either an underscore, or letter, but cannot begin with a number.

Variable names can only contain normal text characters and underscores, and con not contain spaces.

Constants in php are like variables except once they have been defined they can not be redefined, these are used for storing data like a my name, because thats not changing any time soon.

Constants are declared like so: define("MY_NAME", "Solomon Butler");

PHP ECHO / PRINT:

PHP Echo, outputs anything that can be displayed in the browser, this includes strings, numbers, variable values, and even html tags.

The syntax for Echo is as follows: echo 'Solomon';, this will print Solomon onto the browser.

PHP Print, is an alternative to Echo, although that are very similar is use cases.

PHP Print only allows the output of one argument at a time.

PHP DATA TYPES:

THe following data types are supported by the PHP engine:

- Integers
- Strings
- Floating point number
- Booleans
- Arrays
- Objects
- NULL
- Resource

Integers: are non-decimal whole numbers.

Strings: your everyday words or strings of characters, as well as numbers and special characters. Strings must be enclosed in single or double quotes, although they allow for differing outputs, single quotes are 'literal', strings can be concatenated with a ".".

Floating Point Numbers: are integers that allow decimal points, differing from a whole number.

Booleans: only have two possible values "True" and "False".

Arrays: are a variable that can hold multiple values at a time.
These are very useful when working with data as each value caries a unique index value, also known as a key.
There are three types of arrays in PHP:

- index array (Arrays with a numeric index: $skis = array("line", "armadam", "head")).
- associative key (Arrays with named keys: $skis = array("line"=>"good", "armada"=>"bad", "head"=>"good"))
- and multidimensional array (Arrays containing one or more arrays: $skis = array(array("line", "Sick Days"), array("Armada", "Crazy"), array("Head", "Core"));.

Objects: are used in a class template, they allow for a reusable framework of variables that can be given different values.
Objects are created using the "new" keyword.
class skis{
function goodSkis(){
echo "Line";
}
}
$object = new Skis;
echo $object;

NULL: a variable with no value, there for is automatically assigned the value NULL.

Resources: are a special variable referring to an external resource, they are not variables in the traditional sense.
$fp = fopen("test.txt", "w");
echo get_resource_type($fp) . "\n";

PHP STRINGS: Strings: your everyday words or strings of characters, as well as numbers and special characters. Strings must be enclosed in single or double quotes, although they allow for differing outputs, single quotes are 'literal', strings can be concatenated with a ".".

String escape-sequence replacements:
\n makes a new line.
\t is a tab character.
\$ is a $ symbol.

PHP Strings also have functions:
Length of string: strlen($string);
Number of words: str_word_count($string);
Replacing text: str_replace("word_to_be_injected", "word_to_be_replaced", $string);
Reverse string: strrev($string);

PHP NUMBERS: come in three forms, Integers, Floats, Number Strings.

Integers: are numbers without any decimal places, also known as whole numbers. Integers have limits on how large/small they can be, and any number outside of those parameters is stored as "float".
PHP has predefined constants for integers: PHP_INT_MAX is the maximum supported number.
PHP_INT_MIN is the minimum supported number.
PHP_INT_SIZE is a number in bytes.

Floats: are numbers with decimals, or in exponential form.
PHP_FLOAT_MAX is the largest representable floating point number.
PHP_FLOAT_MIN is the smallest representable positive floating point number.
PHP_FLOAT_MIN is the smallest representable negative floating point number.

Infinity: is any number that exceeds PHP_FLOAT MAX.

PHP CONSTANTS: Constants in php are like variables except once they have been defined they can not be redefined, these are used for storing data like a my name, because thats not changing any time soon.
Constants are defined my its Name, and its value, similar to a variable.
Constants can be accessed by using its name.
Constants are declared like so: define("MY_NAME", "Solomon Butler");

PHP OPERATORS:

- Arithmetic operators
- Assignment operators
- Comparison operators
- Increment/Decrement operators
- Logical operators
- String operators
- Array operators

Arithmetic Operators:
Addition + returns the sum.
Subtraction - returns the difference.
Multiplication \* returns product.
Division / returns the quotient.
Modulus % returns the percent.
Exponents \*\* returns the power.

Assignment Operators:
x = y assigns the value on the right to the variable on the left.
x += y is the same as addition, returning the sum of the two values.
x -= y is the same as subtraction, returning the difference of the two values.
x \*= y is the same as multiplication, returning the product of multiplication.
x /= y is the same as division, returning the quotient of the two values.
x %= y is the same as modulus, returning the percent of the two values.

Comparison Operators:
x == y Equal, returning true if the values are equal.
x === y Identical, returning true only if the two values are of equal value and same type.
x != y Not Equal, returning true if the two values are not equal in value.
<> same as above.
x !== y Not Identical, returning true only if the tow values are not equal and of different type.
x > y Greater Than, returning true if the first value is greater than that of the second.
x < y Less Than, returning true if the first value is less than that of the second.
x >= y Greater Than or Equal To, returning true the first value is greater or equal to that of the second.
x <= y Less Than or Equal To, returning true if the first value is less than or equal to that of the second.
x <=> y Spaceship, Less than, Equal to, or Greater than.

Increment/Decrement Operators:
++$ increments variable by one then returns the value.
$++ returns variable value then increments by one.
--$ decrements variable by one then returns the value.
$-- returns variable value then decrements by one.

Logical Operators:
x and y returns true if both variables are true.
x or y returns true if either variables are true.
x xor y returns true if either variables are true but not if both are.
x || y returns true if either variables are true.
x! returns true if variable is not true.

String Operators:
x . y Concatenating the two variables.
x .= y Concatenation Assignment appends the first variable to the second.

Array Operators:
x + y Union of the two variables.
x == y Equality, returns true if both variables have the same key/value pairs.
x === y Identity, returns true if both variables have the same key/value pairs in the same order and of the same type.
x != y Inequality, returns true if the first variable is not equal to the second.
<> same as above.
x !== y Non-identity, returns true if the first variable is not identical to the second.

PHP IF & ELSE & ELSEIF:

IF:
if (condition){
code to be executed if condition is met
};

ELSEIF:
elseif (condition){
code to be executed if this condition is met
};

ELSE:
else {
code to be executed if none of the conditions are met
};

PHP FUNCTIONS:

PHP has many built in functions, which makes it a very powerful language, though a user may create they're own.

Functions in php are a block of code that can be used multiple times, functions will not execute until called upon.

Function names must start with a letter or an underscore, same as variables, although function names are not case sensitive.

User generated function are very similar to those in javascript are are written as follows:

function function_name($parameter, $parameter){
  code to be executed;
}
function_name($parameter. $parameter);

PHP ARRAYS:

Arrays: are a variable that can hold multiple values at a time.
These are very useful when working with data as each value caries a unique index value, also known as a key.
There are three types of arrays in PHP:

- index array (Arrays with a numeric index: $skis = array("line", "armadam", "head")).
- associative key (Arrays with named keys: $skis = array("line"=>"good", "armada"=>"bad", "head"=>"good"))
- and multidimensional array (Arrays containing one or more arrays: $skis = array(array("line", "Sick Days"), array("Armada", "Crazy"), array("Head", "Core"));

PHP LOOPS:

Loops are used to execute the same line of code over and over until a certain condition is met, allowing for an automated approach to a repetitive task.

PHP supports four types of loops:

While: loops through a block of code as long as a specific condition returns true.
while (condition that must apply){
code to be executed
};

Do-While: loop will run the code to be executed, check if the specified condition has been met, then repeat this process until the condition returns false.

do {
code to be executed;
} while (condition returns true);

For: loop is used to loop through code-to-be-executed until a predetermined condition has been met, this is useful when incrementing values multiple times.

for (starting value, ending condition to be met, incrementation){
code to be executed for each incrementation until predetermined condition is met;
};

For-Each: is used to loop through an array and perform a task on each key/value pair.
foreach (array as value){
code to be executed;
};

A for-each will also work with associative arrays,
foreach(array as key => value){
code to be executed;
};
