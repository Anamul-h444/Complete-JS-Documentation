# Complete JS Documentation
<a name='top'></a>
<button style='padding:5px; font-size:18px;'>JS Fundamental</button>

1. [Statement and Comments](#Statement)
1. [Details about variable](#variable)
1. [Concatenation](#Concatenation)
1. [Data types](#dataTypes)

<a name='Statement'></a>
<details>
<summary> Statement and Comments</summary>
<h1> Statement and comments </h1>

> ***Statement***

Statement is a command. After complete command use (;). In below two variable is seperate statement.
### Example:
```js
var name;
let age;
```
> ***Comments***

In JavaScript, comments can be added using either double slashes (//) or a forward slash followed by an asterisk (/*) and an asterisk followed by a forward slash (*/).

Single-line comments, which are ignored by the JavaScript interpreter, can be added using double slashes:

`// This is a single-line comment`

Multi-line comments, which can span multiple lines and are also ignored by the interpreter, can be added using forward slash and asterisk:
```js
/* This is a
multi-line comment */
```
[Go to top:arrow_up: ](#top)
</details>


<a name='variable'></a>
<details>
<h1>Details about variable </h1>
    <summary>Details about variable</summary>

<button style='padding:3px; font-size:16px'>Learning summary</button>
- what is variable.
- Declaration of variable.
- Rules of assigning variable name.
- Assign value in variable.
- System of Re-assign value.
- Difference between var, let and const.
- Local and Global variable/scope.

> ***What is Variable?***  

Variable is a Container which store data.

> ***Declaration of Variable***

By three keyword declare variable.
- var
- let
- const  

### Example of declare variable
```js
var name;
let age;
const className;
```
> ***Rules of assigning variable name***

- Names can contain letters, digits, underscores, and dollar signs.
- Names must begin with a letter not number.
- Names can also begin with $ and _ (but we will not use it in this tutorial).
- Names are case sensitive (y and Y are different variables).
- Reserved words (like JavaScript keywords) cannot be used as names.
- Don't use ' ' or " " in variable name.

> Assign value in variable

Assign value in variable by = (assignment operator).

### Emample  of assign value:
```js
var name = "Anamul";
let age = 36;
const ClassName = 'Nine"
```
> ***Re-assign value***

When re-assign value in declared variable cann't use var, let and const.
```js
// Declare a variable with value
let name = 'Anamul';
console.log(name) // Result - Anamul

// Re-assign value in declared variable
name = 'Haque'
console.log(name) // Result - Haque
```
> ***Difference between var, let, const***

- var
    - variable can be re-declared by var
    - value can be re-assigned by var
- let
   - variable can't be re-declared by let
    - value can be re-assigned by let
- const
   - variable can't be re-declared by const
    - value can't be re-assigned by const

[Go to top:arrow_up: ](#top)

</details>


<a name='Concatenation'></a>

<details>
<summary>Concatenation</summary>

<h1> Concatenation </h1

<button style='padding:3px; font-size:16px'>Learning summary</button>
- Traditional concatenation using the plus (+) operator.
- concatenation with backtick (`).

> ***Traditional concatenation***
### Example:
```js
// Declare variable and assign value
const name = "Anamul";
const age = 35;

// Without Space
const bioData = "My name is" + name +"." + "I am" + age + "years old."
console.log(bioData);
// Output - My name isAnamul.I am35years old.

// With Space after is,am and before years
const bioData1 = "My name is " + name +"." + "I am " + age + " years old."
console.log(bioData1);
// Output - My name is Anamul.I am 35 years old.

// With Space " " 
const bioData2 = "My name is"+ " " + name +"." + "I am"+" " + age + " " + "years old."
console.log(bioData2);
// Output - My name is Anamul.I am 35 years old.
```
> ***concatenation with backtick (`)***

The rule of concatenation with backtick in JavaScript (also known as template literals) is to use the backtick (`) character instead of single or double quotes to define a string. Within the backticks, you can use expressions enclosed in ${} to concatenate variables or other expressions into the string.

For example, if you have a variable "name" with the value "John" and another variable "age" with the value 30, you can concatenate them into a string using the backtick notation like this:
```js
let name = "John";
let age = 30;
let message = `My name is ${name} and I am ${age} years old.`;
console.log(message);
```
This will output the following string: "My name is John and I am 30 years old."

The backtick notation allows for more readable and flexible string concatenation compared to traditional concatenation using the + operator. It also allows for multiline strings without the need for concatenating multiple lines using the + operator.
```js
let poem = `Roses are red
Violets are blue
Sugar is sweet
And so are you`;

console.log(poem);
```
[Go to top:arrow_up: ](#top)
</details>


<a name='dataType'></a>

<details>
--------------------------------------------------------------------------------------------------------
<summary>Data types</summary>
<h1>Data types</h1>

Ther are two types of data:  
1. Premitive data type.
2. Object/Reference type data.

> ***Premitive data type***

There are seven premitive type data:
1. Number: Use for decimal and integers (let age=25)
2. String: Sequence of characters. Used for text by Single or double cotation (let name='Anamul')
3. Boolean: Logical type that can only be true of false. Used for taking decision (let absent = true)
4. Undefined: Value taken by a variable that is not yet define (Empty value) (let age;)
5. Null: Means empty value;
6. Symbol: Vlue that is unique and connot be changed.
7. Bigint: For use large integers number.

> ***Object/Reference type data***

1. object.
2. Array.
3. date.

> ***Discription of Number type data***
- এই ডাটা লিখার সময় কোটেশন ব্যতিত লিখতে হয়।
- নাম্বারকে কোটেশনের মধ্যে লিখলে তা স্ট্রিং হয়ে যায়।
- এই ডাটায় দশমিক ব্যবহার করলে তাকে integer  বলে।
- এই ডাটায় দশমিক ব্যবহার না করলে তাকে floating point/decimal বলে। 
### _infinity Error:_
- 0 দিয়ে কাউকে ভাগ কররে যে ইরর আসবে তাকে infinity Error বলে। (let length = 25/0;)

### _non  Error:_
- স্ট্রিং এর সাথে কোন ম্যাথম্যাথিক্যাল অপারেশন করলে যে ইরর আসবে তাকে non Error বলে। (let length = "25"/0;)

> ***Discription of String type data***
- এই ডাটা লিখার সময় ডাবল বা সিংগেল কোটেশনের মধ্যে লিখতে হয়।
```js 
let name="Anamul"
```
- নাম্বারকে কোটেশনের মধ্যে লিখলে সেটি স্ট্রিং টাইপ ডাটা হয়ে যায়।
```js 
let mobile="01735..."
```
- ডাটার ভিতরে সিংগেল কোটেশনের অবজেক্ট থাকলে স্ট্রিং ডাবল কোটেশনে লিখতে হবে।
```js 
let abbr="'WWW'-World wide web"
```
- ডাটার ভিতরে ডাবল কোটেশনের অবজেক্ট থাকলে স্ট্রিং সিংগেল কোটেশনে লিখতে হবে।
```js 
let abbr=' "WWW"-World wide web'
```
## _Escape Character in string:_

|Code| Result | Description |  	
| --- | --- | --- |
| \\' | ' | Single quote |
| \\" | " | double quote |
| \\\ | \ | Backslace |
| \b  |  |  Backspace|
|\f |  | Form Feed |
|\n |  | New Line |
| \r|  | Carriage Return |
|\t |  | Horizontal Tabulator |
|\v |  | Vertical Tabulator |

## _String–type-data with (Backtick) (`):_
- Backtick দিয়ে স্ট্রিং লিখার নিয়মঃ
```js
let data =`I am a Student`
```
- Backtick দিয়ে লিখিত স্ট্রিং এর মধ্যে কোন ভেরিয়েবল এর ভেল্যু প্রিন্ট করতে হলে ${} এর ভিতরে ভেরিয়েবল লিখতে হবে।

```js
let firstName='Anamul";
let lastName='Haque';
let fullName = `${firstName} ${lastName}
```
> ***Description of null type data:***
- এই ডাটার অর্থ হল খালি ডাটা।
- যখন কোন ভেরিয়েবল এর ডাটা জানা থাকেনা অথবা পরবর্তীতে ইউজার থেকে ইনপুট আসবে তখন এই টাইপ ভেরিয়েবল ডিক্লিয়ার করা হয়।
- ইউজার কর্তৃক ইনপুট করার কথা কিন্তু ডাট না দিয়ে সাবমিট করলে null প্রদর্শিত হবে।
```js
let name = null;
let age = " ";
```
> ***Description of undefine type data:***
- এই ডাটার অর্থ হল ডাটার্টি undefine
- যখন কোন ভেরিয়েবল এ ভেল্যু এ্যাসাইন না করা হয় তখন undefine ইরর আসবে।
```js
let name;
console.log(name); // output - undefine
```
> ***Decription of Booleans type data:***
- এই ডাটায় শুধুমাত্র true এবং false থাকে।
```js
let x = true;
let y = false;
```
> ***Truthy and Falsy value:***

In JS there are five false value and all other is true value.
### _Five falsy value:_
    0 
    ""
    undefine
    null
    NaN
### _Example of falsy and truthly value:_
```js
console.log(Boolean("")); //false
console.log(Boolean(undefined)); //false
console.log(Boolean(null)); //false
console.log(Boolean(0)); //false
console.log(Boolean(NaN)); //false

console.log(Boolean({})); // true
console.log(Boolean([])); // true

// Example with statement
let amount1=0;
let amount2=100;

if (amount2){
    console.log("Do not spent all!")
}else{
    console.log("You need to income!")
}
// Output by amount1 - You need to income!
// output by amount2 - Do not spent all!
```
> ***Decription of Array type data***

In JavaScript, an array is a data type that holds a collection of elements, which can be of any data type, such as numbers, strings, objects, and even other arrays. Elements in an array are ordered and can be accessed by their index, which is a numerical value that represents the position of the element in the array. Arrays are created using the Array constructor or the array literal notation [ ]. For example:
```js
var numbers = new Array(1, 2, 3);
var fruits = ["apple", "banana", "orange"];
```
You can access the elements of an array using the index notation []. For example, to access the first element of the fruits array, you would use `fruits[0]`.

> ***Decription of Object type data***

In JavaScript, an object is a collection of properties, each with a name and a value. Objects are used to store and organize data in a structured way, and can be used to represent real-world objects, such as a person or a car. Objects can also be used to store and manipulate data in a program, such as a user's preferences or a game's score.

Here is an example of an object in JavaScript:
```js
let person = {
name: "John Doe",
age: 30,
occupation: "Developer",
hobbies: ["reading", "hiking", "coding"]
};
```
In this example, the object "person" has four properties: "name", "age", "occupation", and "hobbies". Each property has a name (a string) and a value (a string or an array or object).

Objects in JavaScript can be modified and accessed using the dot notation (e.g. person.name) or the bracket notation (e.g. `person["name"]`). They can also be used in loops, conditionals, and other JavaScript functions.

<a name='top'></a>
</details>