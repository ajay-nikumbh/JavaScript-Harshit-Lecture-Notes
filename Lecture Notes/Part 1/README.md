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
11. Undefined, null and bigint

```js
// Undefined and null

// Define the firstname w/o any value
let firstName;

// Output the firstname w/o any value and that will be undefined
// With let and var keywords you can define and output will be undefined but with the const keyword it will throw an error
console.log(typeof firstName);

// Define the firstname with the value
firstName = "Harshit";

// Output the typeof firstname as well as the firstname
console.log(typeof firstName, firstName);

// Define the null 
let myVariable = null;

// Output the null w/o any value
console.log(myVariable);

// Define the value with myvariable
myVariable = "harshit";

// Check the type of the myvariable which in this case is null and if we check the type of the null then its object
// Even thought if its a bug but keeping in mind the old code base its not removed and kept as its so that 
console.log(myVariable, typeof myVariable);

// Check the type of the null
console.log(typeof null);

// BigInt
// Define the big integer
let myNumber = BigInt(12);

// Define the big integer 
// If we want to declare the big int number explicitly then mention n
let sameMyNumber = 123n;

// Output the mynumber
console.log(myNumber);

// Output the max safe integer value
console.log(Number.MAX_SAFE_INTEGER);

// Add the 2 number's
console.log(myNumber+ sameMyNumber);

```

12. Boolean and comparision operator

```js

// Booleans & comparison operator. Booleans [true, false]

// Declare the 2 numbers num1 and num2
let num1 = 7;
let num2 = "7"; 

// Apply the comparison operator to num1 and num2 and return the result
console.log(num1<num2);

// Double equal == vs Triple equals === 
// Double equals return the result true if the both the number's are equal
console.log(num1 == num2);

// Triple equals returns the result true if both the number's data type is equal
console.log(num1 === num2);

// Not equal!= vs Not double eqaul!==
// Not equals return the result true if both the number's data type
// Double equals return the result true if both the number's data type is equal
console.log(num1 !== num2);

```
13. Truthy and falsy values


```js
// truthy and falsy values 

false
""
null 
undefined
0

```

14. If else condition

```js

// If else condition 

// Define the age parameter
let age = 17;

// If case
if(age>=18){

    // Output
    console.log("User can play ddlc");
}

// Else case
else {

    // Output
    console.log("User can play mario");
}

// Define the num parameters
let num = 13;

// Even number logic
if(num%2===0){

    // Even number o/p
    console.log("even");
}

// Else
else{

    // Odd number o/p
    console.log("odd");
}

// Falsy values -   false, "", null, undefined, 0, 
// truthy values -  "abc", 1, -1

// Define the firstname parameter
let firstName= 0;

// If case
if(firstName){

    // Output the firstname parameter
    console.log(firstName);
}

// Else case 
else{

    // Output 
    console.log("firstName is kinda empty");
}
```
15. Ternary operator

```js
// Ternary operator 

// Define the age parameter
let age = 4;

// Define the drink parameter
let drink;

// If case
if(age>=5){
    drink = "coffee";
}

// Else case
else{
    drink = "milk";
}

// Output the drink
console.log(drink);

// Ternary operator / Conditional operator 

// Define the age parameter
let age1 = 3;

// Define the drink parameter and use the ternary operator
let drink1 = age1 >= 5 ? "coffee" : "milk";

// Output the drink
console.log(drink1);
```
16. And or operator

```js

// And  or operator 

// Declare the firstname variable
let firstName = "arshit";

// Define the age variable
let age = 16;

// If case 
if(firstName[0] === "H" || age>18){
    
    // Output the ans
    console.log("inside if");
}

// Else case
else{

    // Output the ans
    console.log("inside else");
}
```

17. Nested if statement
    
```js
// Nested if else

// Define the winning number
let winningNumber = 19;

// Define the userguess number and take the  input value from the input field from the user input
let userGuess = +prompt("Guess a number");

// If case
if(userGuess === winningNumber){
    
    // Output
    console.log("Your guess is right!!");
}

// Else case
else{

    // If case
    if(userGuess < winningNumber){
        
        // Output
        console.log("too low !!!");
    }
    
    // Else case
    else{

        // Output
        console.log("too high !!!");
    }
}
```
18. Else if ladder

```js
// Declare the variables tempindegree
let tempInDegree = 4;

// If case
if(tempInDegree > 40){
    
    // Output
    console.log("too hot");
}

// Else if case
else if(tempInDegree > 30){
    
    // Output
    console.log("lets go for swim");
}

// Else if case
else if(tempInDegree > 20){
    
    // Output
    console.log("weather is cool");
}

// Else if case
else if(tempInDegree > 10){
    
    // Output
    console.log("it is very cold outside");
}

// Else case
else{

    // Output
    console.log("extremely cold");
}

// Output the answer
console.log("hello");
```

19. Switch case

```js 

// Define the day variable
let day = 9;

// Use the switch statement to switch the day variable
switch(day){

    // Handle the different cases
    case 0:
        console.log("Sunday");
        break; 
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    case 4:
        console.log("Thrusday");
        break;
    case 5:
        console.log("Friday");
        break;
    case 6:
        console.log("Saturday");
        break;
    
    // Handle the default case if none is satisfied
    default:
        console.log("Invalid Day");
}

```
20. While loop

```js
// While loop 

// Declare the variables i
let i = 0; 

// Use the while loop
while(i<=9){
    
    // Output
    console.log(i);
    
    // Increment the counter
    i++;
}

// Return the current variable i
console.log(`Current value of i is ${i}`);

```







