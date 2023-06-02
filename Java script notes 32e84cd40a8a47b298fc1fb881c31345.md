# Java script notes

## Javascript

javascript is added to webpage in four ways

1.Inline Script

```jsx
<body>
    <button onclick="alert('hello world')">Click Me</button>
  </body>
```

2.Internal Script

```
<head>
<script>
      console.log('hello world')
    </script>
</head>
```

3.External Script

another file is created with extension .js and write the code in the file then link the file to the html file using the code below

```jsx
<script src="introduction.js"></script>
```

4.Multi External Script

it is the same as the external script but we can link two or more js files to the html file.

### comments in java script

1. single line comment (//)
2. multi line comment(//*     */)

## Variables

Variables are memoryspace for storing data (storing data values).

Example

Variables in java script are declared using the keyword let ,var and const.

rules of writing javascript variables

- should not begin with a number.
- does not allow special characters except dollar sign and underscore.
- name should not have space between words.

## Datatype

Datatype describes the characterstics of the data.

1. String

2.numbers

3. Boolean

4. Undefined

5. Null

### primitive and non primitive datatype

primitive datatype (immutable or non modifiable)

1. Numbers- datatypes which includes integer and float values
2. Strings-a character or group of character under double,single or back-tick qoute
3. Booleans - datatype with truth value(True or False)
4. Null-is when the variable is empty
5. Undefined-if a variable is not intialized it is undefined

non primitive datatype(mutable or modifiable)

1. Objects-It is used to store various keyed collections and more complex entities
2. Arrays-An array is a special variable, which can hold more than one value

primitive datatypes are compared by value where as non primitive data type are can not be compared by value rather they are compared by reference 

for example

```jsx
let a=6
let b=6
console.log(a==b) // this is true because numbers are primitive data types
let a={10,20,'a'}
let b={10,20,'a'}
console.log(a==b) // this is false because numbers are non primitive data types
// they are not compared by value.
let a={10,20,'a'}
let b=a
console.log(a==b) //this true because they have the same reference
```

***N.B***  ***A JavaScript variable can hold any type of data.***

### Strings

-are texts that are under single qoute , double qoute or back-tick quote

-to combine two strings we use ‘+’ (plus) sign and the process is called concatination.

```jsx
let name='sara'
let fathername='feleke'
let fullname= name+fathername
console.log(fullname)  // output will be sara feleke
```

Long literal string : are strings with big length like paragraph. we can use ( / ) to show the string continues next line.

Template literals: use back-ticks (``) rather than the quotes ("") to define a string.

using template literals you can use both single and double quotes inside a string.

Template literals provide an easy way to interpolate variables and expressions into strings.

The method is called string interpolation.

The syntax is:

${...}

```jsx
let firstName = "sara";
let lastName = "feleke";
let text = `Welcome ${firstName}, ${lastName}!`;
```

***String methods***

length: console.log(stringname.length)

**access character in string**:  stringname[index number]

**change the characters of string to upper case:** console.log(stringname.toUpperCase())

**change the characters of string to lower case**: console.log(stringname.toLowerCase())

**substr()**: It takes two arguments, the starting index and number of characters to slice: console.log(stringname.substr(starting index , number of characters to cut))

**substring()**: It takes two arguments, the starting index and the stopping index but it doesn't include the character at the stopping index.

**split()**: The split method splits a string at a specified place. first changes it to array then splits it.

**trim()**: Removes  space in the beginning or the end of a string.

**includes()**: It takes a substring argument and it checks if substring argument exists in the string. *includes()* returns a boolean.

**replace():** takes as a parameter the old substring and a new substring. it is used to replace a string by another one.

**charAt()**: Takes index and it returns the character at that index.

**charCodeAt()**: Takes index and it returns ASCII number of the value at that index.

**concat():** used to concatinate strings.

      How to check datatype

syntax 

`console.log(typeof variablename)`

       Casting datatypes or converting one datatype to another

String to Int (converted using the methods below) 

- parseInt()  `parseInt(stringname to be converted)`
- Number() `Number(stringname to be converted)`
- Plus sign(+)

let num1=’20’

let num2=+ num1

String to float 

except the first method used above the two methods work for conversion of string to float and the third method is

• parseFloat()

Float to Int

• parseInt()

## Operators

There are different types of JavaScript operators:

- Arithmetic Operators

Addition(+)

Subraction(-)

Division(/)

Multiplication(*)

Modulus(%)

Exponential(**)

- Assignment Operators

Example   =,+=,-=……

- Comparison Operators

Example ==(equal by value only),===(equal by value and datatype) ,>,≥,≤….

- Logical Operators

Example  &&,|| and !

- Bitwise Operators

Example AND,NOT,OR,XOR

- Ternary Operators(Ternary operator allows to write a condition.)

Example

```jsx
let number = 2
number > 0
  ? console.log(` positive number`)
  : console.log(` negative number`)
// output postive number
```

***operation(addition) of different data type (string and number)***

When adding a number and a string, JavaScript will treat the number as a string. as shown below

```jsx
let x = 16 + "Volvo"
// it will read as
let x = "16" + "Volvo";
```

JavaScript evaluates expressions from left to right. Different sequences can produce different results as shown below.

```jsx
let x = 16 + 4 + "Volvo";
//Result:
//20Volvo
let x = "Volvo" + 16 + 4;
//Result:
//Volvo164
```

# Javascript control statements

Javascript control statement is used to control the flow of program based on the specified condition.

### Conditional statements

**1. If Statement**

JavaScript If Statement:

If statement is used to execute a block of statements if specified condition is true.

Syntax:

```jsx
if(condition){
 //Block of JavaScript statements. 
}
```

**2.if else statements**

```jsx
if(condition){
//Block of JavaScript statements1.
}else{
//Block of JavaScript statements2.
}
```

**3. if else if statement**

```jsx
if(condition1){
 //Block of JavaScript statements1. 
}else if(condition2){ 
//Block of JavaScript statements2. 
} . . . else if(conditionn){
 //Block of JavaScript statementsn. 
}else{
 //Block of JavaScript statements. 
}
```

```jsx
<html>
<head>
<script>  
var num=2;  
if(num==1){  
document.write("JavaScript Statement 1");  
}  
else if(num==2){  
document.write("JavaScript Statement 2");  
}  
else if(num==3){  
document.write("JavaScript Statement 3");  
}  
else{  
document.write("JavaScript Statement n");  
}  
</script>  
</head>
<body>
</body>
</html>
```

**4.switch statements**(alternative form of if else if statement)

```jsx
switch(caseValue){
  case 1:
    // code
    break
  case 2:
   // code
   break
  case 3:
   // code
   break
  default:
   // code
}
```

### Loops

**1.For loop**

The `for` statement creates a loop with 3 optional expressions:

syntax:

```jsx
for (expression 1; expression 2; expression 3) {
  // code block to be executed
}
// example
let text=0
for (let i = 0; i < 5; i++) {
  text += "The number is " + i + "<br>";
}
```

**2.The While Loop**
The while loop loops through a block of code as long as a specified condition is true.
Syntax:

```jsx
while (condition) {
  // code block to be executed
}
//example
while (i < 10) {
  text += "The number is " + i;
  i++;
}
```

**3.The Do While Loop**

The `do while` loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.

Syntax:

```jsx
do {
  // code block to be executed
}
while (condition);
//example
do {
  text += "The number is " + i;
  i++;
}
while (i < 10);
```

**4.For of loop**

it is used to iterate through an array if we are not interested in the index of each element in the array.

```jsx
for (const element of arr) {
  // code goes here
}
```

**Break**

is used to break a loop.

```jsx
for(let i = 0; i <= 3; i++){
  if(i == 1){
    break
  }
  console.log(i)
}
// after it iterates once then it will stop
```

**Continue**

used to skip some iterations and continue.

```jsx
for(let i = 0; i <= 2; i++){
  if(i == 1){
    continue
  }
  console.log(i)
// after 0 is displayed it escapes 1 and displays 2
```

# Data structure

All primitives are *immutable*; that is, they cannot be altered. It is important not to confuse a primitive itself with a variable assigned a primitive value. The variable may be reassigned to a new value, but the existing value can not be changed in the ways that objects, arrays, and functions can be altered.

**Non-primitive data types:** The data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types. It is also known as derived data types or reference data types.

JavaScript has primitive and non-primitive data structures. Primitive data structures are native to the programming language, such as boolean, number, string, array, and object. [Non-primitive data structures are not built-in and have to be coded, such as linked list, stack, queue, set, and hash table](https://data-flair.training/blogs/javascript-data-structures/)

# Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

JavaScript function is defined with the `function` keyword, followed by a **name**, followed by parentheses **()**.

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:

**(*parameter1, parameter2, ...*)**

A function can be declared or created in couple of ways:

- Declaration function

```jsx
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

Function without parameter and return (Function can be declared with out including variables)

the value of function is undefined,`If a function doesn't return it doesn't store data`

```jsx
function number(){
let num1=6;
let num2=3;
let res=num1/num2;
console.log(res)

}
number()

```

Function with returns

```jsx
function number(){
let num1=6;
let num2=3;
let res=num1/num2;
return res
}
console.log(number())

```

Functions can accept one, two or many parameters,or unlimted parameter

- Expression function

are anonymous function after it is declared it is assigned to a variable.

```jsx
const add = function(n) {
let sum=n+n
  return sum
}

console.log(add(2))
```

- Anonymous function

function without name

```jsx
const anonymousFun = function() {
  console.log()
  )
}
```

- Arrow function

another way to declare functions.

```jsx
const functionA = (parameter1, parameter2, ..., parameterN) => {
  // Function body here
}
//example
const printHello = () => {
  console.log('hello');
};
```

When JavaScript reaches a `return` statement, the function will stop executing.

Functions often compute a **return value**. The return value is "returned" back to the "caller":

```jsx
// Function is called, the return value will end up in x
let x = myFunction(4, 3);

function myFunction(a, b) {
// Function returns the product of a and b
  return a * b;
}
```

The () operator invokes (calls) the function:

```jsx
function toCelsius(fahrenheit) {

return (5/9) * (fahrenheit-32);

}

let value = toCelsius();
```

Accessing a function without () returns the function and not the function result.

# Array

An array is a special variable, which can hold more than one value:

array can have different data types

Creating arrays

Using array constructor

```jsx
const arr = Array()
// or
let arr = new Array()
```

using square bracket

```jsx
const arr = []
//array with values
const arr = [2,5,7,8]
// to find length
arr.length
```

creating an array using split

```jsx
let js = 'JavaScript'
const charsInJavaScript = js.split('')

console.log(charsInJavaScript) // ["J", "a", "v", "a", "S", "c", "r", "i", "p", "t"]
```

we can access array using index number and modifying element of an array

```jsx
const arr = [2,5,7,8]
console.log(arr[0])// access elements
arr[0]=9// modify the first element of an array
```

Methods used to manipulate array

**array()**-used to create array

```jsx
const arr = Array()
```

**sort()**- to sort an array

```jsx
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
```

**reverse()**- to reverse elements of an array

```jsx
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.reverse();
```

**concat()**- used to concatinate two arrays

```jsx
let arr1=[1,2,3]
let arr2=[4,5,6]
let arr3=arr1concat(arr2)
```

**indexOf**- the find the index of element.  arrayname.indexOf(element of array)

**LastIndexOf**-It gives the position of the last item in the array.

**includes**:To check if an item exist in an array. arrayname.includes(element)

**Array.isarray**-if the datatype is array. `Array.isArray(numbers)` result is boolean value

**toString()**-change array to string. arrayname.toString()

**join**-to join elements of arrays and returns ad string. arrayname.join()

**push**- used to add new element in the array arrayname.push(new element)

**pop**- used to remove the last element in the array. arrayname.pop()

**shift**- remove the first element of an array. arrayname.shift()

**unshift**-add an element from the beginning. arrayname.unshift(new element)

# JavaScript Objects

Variables scopes can be:

- Global

Anything declared without let, var or const is scoped at global level.

A globally declared variable can be accessed every where in the same file. But the term global is relative. It can be global to the file or it can be global relative to some block of codes. can not be accessed by another files.

- Local

A variable declared as local can be accessed only in certain block code.Block (variable declared with let and const)and Function scope(variable declared with var)

The scope *let* and *const* are the same. The difference is only reassigning. We can not change or reassign the value of the const variable.

### Objects in javascript

creating object

```jsx
const number = {}// empty object
const circle = {
  radius: 20
 
}
```

How to access values of object

- using . followed by key name if the key-name is a one word
- using square bracket and a quote

```jsx
const circle = {
  radius: 20
 
}
console.log(circle.radius)
console.log(circle['radius'])
```

set new key for an object

```jsx
const circle = {
  radius: 20
 
}
circle.radius=6;
```

Object methods

 **Object.assign() method** is used to copy the values and properties from one or more source objects to a target object. It invokes getters and setters since it uses both [[Get]] on the source and [[Set]] on the target.

```jsx
Object.assign(target, ...sources)
//Parameters: 
//target: It is the target object to which values and properties have to be copied.
//sources: It is the source object from which values and properties have to be copied.
//Object.assign() returns the target object.
//example
const obj1 = { a: 1 };
const new_obj = Object.assign({}, obj1);
  console.log(new_obj)
// output object { a: 1 }
```

**Object.key()**

To get the keys or properties of an object as an array

```jsx
const object1 = {
  a: 'somestring',
  b: 42,
  c: false
};

console.log(Object.keys(object1));
// Expected output: Array ["a", "b", "c"]
```

**Object.values()**

To get values of an object as an array

```jsx
const object1 = {
  a: 'somestring',
  b: 42,
  c: false
};

console.log(Object.values(object1));
// Expected output: Array ["somestring", 42, false]
```

**Object.entries()**

To get the keys and values in an array

```jsx
const object1 = {
  a: 'somestring',
  b: 42
};

for (const [key, value] of Object.entries(object1)) {
  console.log(`${key}: ${value}`);
}

// Expected output:
// "a: somestring"
// "b: 42"
```

Use the keyword `class` to create a class.

Always add a method named `constructor()`:

```jsx
class ClassName {
  co.nstructor() { ... }
}
//Example
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
}
```

```jsx
//create objects
const myCar1 = new Car("Ford", 2014);
const myCar2 = new Car("Audi", 2019);
```

Example 

```jsx
class Car {
  constructor(name, year) {
    this.name = name;
    this.year = year;
  }
  age() {
    const date = new Date();
    return date.getFullYear() - this.year;
  }
}

const myCar = new Car("Ford", 2014);
document.getElementById("demo").innerHTML =
"My car is " + myCar.age() + " years old.";
```