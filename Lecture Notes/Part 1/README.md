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
21. While loop example

```js
// While loop example 

// Declare the num variable
let num = 100;

// Define the total
let total = 0; //1 + 2 +3

// Define the i variable
let i = 0;

// Use the while loop
while(i<=100){
    
    // Update the total variable
    total = total + i;
    
    // Update the i variable 
    i++;
}

// Return the total variable as output
console.log(total);

// Use the formula below to compute the sum of the variables
let total1 = (num*(num+1))/2;

// Return the total1 variable as output
console.log(total1);
```

22. Var and let uses
    
```js
/*
Note: 

1. If you use the let keyword then you will not be able to to access the value of the the i outisde the method.
2. If you use the var keyword then you will get the value of the of the i outisde the method also.

*/

// Introduction to the for loop
for(let i = 0;i<=9;i++){
    
    // Output the i value
    console.log(i);
}

// Output the value of the i variable
console.log("value of i is ",i);
```

23. For loop example

```js
// For loop example

// Define the total variable
let total = 0;

// Define the num variable
let num = 100;

// Use the for loop variable
for(let i = 1; i<=num; i++){
    
    // Compute the total
    total = total + i;
}

// Output the total variable
console.log(total);
```
24. Break & continue keyword

```js
// Break keyword and Continue keyword 

// For loop
for(let i = 1; i<=10; i++){
    
    // Break if i == 4 then break keyword
    if(i===4){
        break;
    }

    // Output
    console.log(i);
}


// Continue keyword
for(let i = 1; i<=10; i++){
    
    // Break if i == 4 then continue with the current iteration
    if(i===4){
        continue;
    }

    // Output
    console.log(i);
}

```
25. Do while loop
    
```js
// Do while loop

// Loop through the iteration 
while(i<=9){

    // Output the current iteration
    console.log(i);
    
    // Increment the iteration counter
    i++;
}


// Declare the i variable
let i = 10;

// Use the do while loop
do{

    // Output the current iteration
    console.log(i);

    // Increment the iteration counter
    i++;

}while(i<=9);

// Output the i variable value
console.log("value of i is ", i);
```
26. Introduction to array's
    

```js
// Introduction to arrays - reference type 
// Here the array is the reference type and its a type of the object.
// Define the fruits array
let fruits1 = ["apple", "mango", "grapes"];

// Define the number's array
let numbers = [1,2,3,4];

// Define the mixed array
let mixed = [1,2,2.3, "string", null, undefined];

// Ouput the respective array
console.log(mixed);

// Ouput the respective array
console.log(numbers);

// Ouput the respective fruits index array
console.log(fruits1[2]);

// Define the fruits array
let fruits = ["apple", "mango", "grapes"];

// Output the fruits array
console.log(fruits);

// Define the object literal
let obj = {}; 

// Update the first index of the fruits array
fruits[1] = "banana";
console.log(fruits);

// Output the type of the fruit array is the object because its the reference type
console.log(typeof fruits);

// Output the type of the object 
console.log(typeof obj);

// Check if the array is really an array
console.log(Array.isArray(fruits));

// Check if the object is really an object
console.log(Array.isArray(obj));

```

27. Array push, pop, shift and unshift

```js
// Array - push, pop, shift, unshift 

// Define the fruits array
let fruits = ["apple", "mango", "grapes"];
console.log(fruits);

// Use the push function to push the elements at end of the array
fruits.push("banana");
console.log(fruits);


// Use the pop function to pop to remove the elements at the end of the array
let poppedFruit = fruits.pop();
console.log(fruits);
console.log("popped fruits is", poppedFruit);

// Use the unshift method to add the elements at the start of the array
fruits.unshift("banana");
fruits.unshift("myfruit");
console.log(fruits);

// Use the shift function to remove the elements from the start of the array
let removedFruit = fruits.shift();
console.log(fruits);
console.log("removed fruits is ", removedFruit);


/*
Note: Push and pop is faster than shift and unshift
*/
```

28. Primitive vs reference data types

```js
// Primitve vs reference data types

// Declare the num1
let num1 = 6;

// Store the num1 into the num2
let num2 = num1;

// Output the num1 and num2
console.log("value is num1 is", num1);
console.log("value is num2 is", num2);

// Increment the num1 by 1
num1++;

// Outptu the num1 and num2
console.log("After incrementing num1")
console.log("Value is num1 is", num1);
console.log("Value is num2 is", num2);


// Reference types 

// Declare the array 1
let array1 = ["item1", "item2"];

// Store the array1 into the array2
let array2 = array1;

// Output the array1 and array2
console.log("array1", array1);
console.log("array2", array2);

// Push the item3 into the array1
array1.push("item3");

// Print the output
console.log("after pushing element to array 1");
console.log("array1", array1);
console.log("array2", array2);
```

29. How to clone the array

```js
// How to clone array 

// 3 Methods to clone array elements - Slice methods, Concat method and Spread method
// Method 1 - Clone array using the slice method
let arr_c1= array1.slice(0)

// Method 2 - Clone array using the concat method
let arr_c2= [].concat(array1);

// Method 3 - Clone array using the spread operator
let arr_c3= [...array1];

// Declare the array1
let array1 = ["item1", "item2"];

// Declare the array22
let array22 = ["item1", "item2"];

// Push one element to the array1
array1.push("item33"); 

// Print the 2 arrays
console.log(array1)
console.log(array22)

// Compare the 2 arrays
console.log(array1===array2);

// Use the slice and concat functions to add the array elements together 
// Here we can use both the slice and concat functions together to perform the operations
let arra = array1.slice(0).concat(["item3", "item4"]);

// Use the concat function to add the array1 and then extra elements to the array
let array_ce = [].concat(array1,["item3", "item4"]);

// Brand new array elements
let oneMoreArray = ["item3", "item4"]
let new_speread_operator_array = [...array1, ...oneMoreArray];



```

30. For loop in array

```js
// For loop in array 

// Declare the fruits array
let fruits = ["apple", "mango", "grapes", "banana"];

// Output the fruit array length
console.log(fruits.length);

// Getting the fruits array element using the length function
console.log(fruits[fruits.length-2]);

// Declare the fruits2 array
let fruits2 = [];

// Use the for loop to convert the fruit array into the uppercase string
for(let i=0; i < fruits.length; i++){

    // Convert the fruit array into the uppercase string
    fruits2.push(fruits[i].toUpperCase());
}

// Output the fruit2 array
console.log(fruits2);
```

31. Use the const for creating arrays

```js

// Use const for creating array
// Heap memory ["apple", "mango"] 0x11

// Use const for creating array
// The use of the const will prevent the array from being modified
// If we use the let for creating the array then we will be able to modify the the existing array
// So when we will be using the reference types we are supposed to use the const instead of let
const fruits = ["apple", "mango"];

// Push array element into the fruits array 
fruits.push("banana");

// Output the fruit array
console.log(fruits);

``` 

32. While loop in array's

```js
// While loop in array 
const fruits = ["apple", "mango", "grapes"];

// Declare the another array fruits2
const fruits2 = [];

// Declare the i element to 0
let i = 0;

// Use the while loop to iterate over the fruits
while(i<fruits.length){

    // Make the fruits array elements to the upper case
    fruits2.push(fruits[i].toUpperCase());

    // Increment the the i element
    i++;
}

// Output the fruit2 array
console.log(fruits2);
```

33. For of loop in array

```js
// For of loop in array

// Declare the fruits array 
const fruits = ["apple", "mango", "grapes", "fruit4", "fruit5"];

// Declare the fruit2 array
const fruits2 = [];

// Use the for of loop in array
for(let fruit of fruits){

    // Make the fruit array elements into the uppercase
    fruits2.push(fruit.toUpperCase());
}

// Output the fruits2 array
console.log(fruits2);


// For of loop in array use the simple for loop in array
for(let i = 0; i<fruits.length; i++){

    // Output the fruits array elements
    console.log(fruits[i]);
}

// We normally use the for of loop in array
// For of loop in array gives the direct element of the array and for in loop gives the index of the array element
```

34. For in loop in array

```js
// For in loop in array

// Declare the fruits array
const fruits = ["apple", "mango", "grapes", "fruit4", "fruit5"];

// Declare the fruit2 array
const fruits2 = [];

// Use the for in loop in array
for(let index in fruits){

    // Make the uppercase elements of the array
    fruits2.push(fruits[index].toUpperCase());
}

// Output the fruits2 array
console.log(fruits2);
```
35. Array destructuring

```js
// Array destructuring 

// Declare the myArray array
const myArray = ["value1", "value2", "value3","value4"];

// Extract the 0 and 1st index values from the array
let myvar1 = myArray[0];
let myvar2 = myArray[1];

// Output the values of the array
console.log("value of myvar1", myvar1);
console.log("value of myvar2", myvar2);

// Note: If you want to skip the value-2 then follow the syntax below
// Here the 2nd index value is skipped because of the comma in between the values
let [m1,,m3] = myArray

// Use the array destructuring concept to store the myArray elements
let [myva1, myva2, ...myNewArray] = myArray;

// Output the values of the array 
console.log("value of myvar1", myvar1);
console.log("value of myvar2", myvar2);
console.log(myNewArray);
```
36. Objects reference types

```js
// Objects reference type  

/*

Note: 

1. Arrays are good but not sufficient for real world data 
2. Objects store key value pairs, objects don't have index

*/

// How to create objects 
// Create the person object
const person = {
    name: "harshit",
    age: 22,
    hobbies: ["guitar", "sleeping", "listening music"]
}

// Output the person object 
console.log(person);

// How to access data from objects 
// Like dictionary in python use the keys to access the object elements
console.log(person["name"]);
console.log(person["age"]);
console.log(person.hobbies);

// How to add key value pair to objects
person["person"] = "male";

// Output the person object
console.log(person);
```

37. Difference between dot and bracket notation

```js
// Difference between dot and bracket notaion

// Define the key email
const key = "email";

// Define the person object key value pairs
const person = {
    name: "harshit",
    age: 22,
    "person hobbies": ["guitar", "sleeping", "listening music"]

}

// Output the person hobbies
console.log(person["person hobbies"]);

// Add the key to the person object
person[key] = "harshitvashisth@gmail.com";

// Log the person information
console.log(person);

```

38. How to iterate over object's

```js
// How to iterate object 

// Create the person object
const person = {
    name: "harshit",
    age: 22,
    "person hobbies": ["guitar", "sleeping", "listening music"]
}


// Use the for in loop to iterate over the person object
for(let key in person){
    
    // Outptu the ans
    console.log(`${key} : ${person[key]}`);
    console.log(key," : " ,person[key]);
}

// Output the the type of the person object
console.log(typeof (Object.keys(person)));

// Check if the person object is an array
const val = Array.isArray((Object.keys(person)));

// Output
console.log(val);


// Use the for of loop to iterate over the the person objects
for(let key of Object.keys(person)){

    // Output the person
    console.log(person[key]);
}
```
39. Computed propertie's

```js
// Computed properties

// Define the 2 keys
const key1 = "objkey1";
const key2 = "objkey2";

// Define the 2 values
const value1 = "myvalue1";
const value2 = "myvalue2";

// Here the problem is that key will not be computed so use the below method
const obj1 = {
    objkey1 : "myvalue1",
    objkey2 : "myvalue2",
}

// Use the computed properties concept to create the obejct
const obj2 = {
    [key1] : value1,
    [key2] : value2
}

// Doing it manually
const obj = {};

// Create
obj[key1] = value1;
obj[key2] = value2;

// Output
console.log(obj);


```

40. Spread operator in object's

```js
// Spread operator in objects

// Define the object1
const obj1 = {
  key1: "value1",
  key2: "value2",
};

// Define the object2
const obj2 = {
  key1: "valueUnique",
  key3: "value3",
  key4: "value4",
};

// Spread operator on the 2 objects
// Here imp point is in both the 2 objects we have key 1 repeated so final value of the key 1 will be last object specified
const newObject = { ...obj2, ...obj1, key69: "value69" };

// Spread operator on the 2 arrays here the 0th index wil be the item1 and the 1st will be the item2
const newObject1 = { ...["item1", "item2"] };

// Here the index will be the key and value will the the letters
const newObject2 = { ..."abcdefghijklmnopqrstuvwxyz" };


```

41. Object destructring

```js
// Object destructuring

// Declare the band object
const band = {
  bandName: "led zepplin",
  famousSong: "stairway to heaven",
  year: 1968,
  anotherFamousSong: "kashmir",
};


// Destructure the band object
let { bandName, famousSong, ...restProps } = band;

// Output the band object
console.log(bandName);

// Output the rest properties of the band object
console.log(restProps);

```

42. Object inside array

```js
// objects inside array 
// very useful in real world applications

// Declare the array of the objects
const users = [
    {userId: 1,firstName: 'harshit', gender: 'male'},
    {userId: 2,firstName: 'mohit', gender: 'male'},
    {userId: 3,firstName: 'nitish', gender: 'male'},
]

// Use the for of loop
for(let user of users){

    // Output
    console.log(user.firstName);
}

```

43. Nested destructuring

```js
// Nested destructuring 

// Declare the list of users
const users = [

    {userId: 1,firstName: 'harshit', gender: 'male'},
    {userId: 2,firstName: 'mohit', gender: 'male'},
    {userId: 3,firstName: 'nitish', gender: 'male'},
]

// Normal users destructuring
const [user1,user2,user3]= users

// Print the user1
console.log(user1)

// Object destructuring and changing the user first name to user1firstName
const [{firstName: user1firstName, userId}, , {gender: user3gender}] = users;

// Print the name
console.log(user1firstName);

// Print the userId
console.log(userId);

// Print the user3 gender
console.log(user3gender);
```
44. Function's

```js
// 1. Define the  functions
function printHello(){
    
    // Print the message to the console
    console.log("Hello");
}

// Calling the printHello method and printing it to the console
console.log(printHello());



// 2. Function expression
const printNumbers = function(numbers){

    // Print the numbers 
    return numbers
}

// Calling the printNumbers method and printing it to the console
console.log(printNumbers(3));




// 3. Arrow function
const printArrow = () =>{
    
    console.log("Arrow");
}

// Calling the printArrow method and printing it to the console
console.log(printArrow());

```











