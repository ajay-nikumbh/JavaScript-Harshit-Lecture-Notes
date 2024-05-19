## Part I lectures

01. Introduction

```js
// Console.log can print something on console 
console.log("hello world");
```

02. Variables

```js
// Use the strcit because we want to restrict the type
"use strict";

// Intro to variables. Variables can store some information

// Declare a variable 
var firstName = "Harshit";

// Output the variable 
console.log(firstName);

// Change the variable
firstName = "Mohit";

// Output the variable which was changed
console.log(firstName);
```

03. Rules for naming the variable's

```js
// Rules for naming variables 

// Declare the variables and log it
var value1 = 2;
console.log(value1);

// You can use only undersore _ or dollar symbol 
first_name (valid)
_firstname (valid) 
first$name (valid)
$firstname (valid)

// You cannot use spaces 
// Snake case writing
var first_name = "harshit";

// Camel case writing 
var firstName = "harshit"; 

```
04. Let keyword

```js
// Let keyword 
let firstName = "harshit";

// Update the name
firstName = "Mohit";

// Log the first name
console.log(firstName);

```
05. Const keyword

```js
// Declare constants 
const pi = 3.14;

// Output the pi value
console.log(pi);

```

06. String declaration

```js
// String declaration
let firstName = "harshitdfjakldsfdf";

// Log the firstcharacter
console.log(firstName[0]);

// length of string 
console.log(firstName.length);

// Get me the second last character
console.log(firstName[firstName.length-2]);


```
07. String methods

```js
// Declare the string 
let firstName = "harshit";

// Output the string length
console.log(firstName.length);

// Use the trim method to trim the string
firstName = firstName.trim();
console.log(firstName)
console.log(firstName.length);

// Make the string to the upper case
firstName = firstName.toUpperCase();
console.log(firstName);

// Make the string lower case
firstName = firstName.toLowerCase();
console.log(firstName);

// Make the string sliceable from the first index to the last index
let newString = firstName.slice(1); // hars
console.log(newString);
```
08. Type of operator

```js
// Typeof operator 
// Data types as follows : string, number, booleans, undefined, null, BigInt, Symbol

// Define the age parameter
let age = 22; 

// Define the firstname parameter
let firstName = "harshit";

// Define the type of age parameter
console.log(typeof age);

// Convert number to string. 
age = age + "";

// Output the age parameter
console.log(typeof(age)); "22"

// Convert string to number. 
let myStr = +"34";

// Output the age parameter 
console.log(typeof myStr);

// Define the age parameter
let age1 = "18";

// Convert string to number. 
age = Number(age1);

// Output the age parameter
console.log(typeof age);
```
09. String concatenation

```js
// String concatenation 
// Define the 2 strings 
let string1 = "17";
let string2 = "10";

// Perform the concatenation using the + operator
let newString = +string1 + +string2;

// Output the new string
console.log(typeof newString);


```
10. Template string

```js
// Template string 
// Define the age parameter
let age = 22;

// Define the firstname parameter
let firstName = "harshit"

// Define the about me with the name and age parameter dynamically with the backtick symbol
let aboutMe = `My name is ${firstName} and my age is ${age}`

// Output the aboutme with the name and age parameter dynamically with the backtick symbol
console.log(aboutMe);

```











