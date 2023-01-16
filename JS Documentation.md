# Complete JS Documentation
<a name='top'></a>
<kbd>**JS Fundamental Contents**</kbd>

_Please click to go to topic >>>>>_

1. [Statement and Comments](#Statement)
1. [Details about variable](#variable)
1. [Concatenation](#Concatenation)
1. [Data types](#dataTypes)
1. [Operators](#operator)
1. [Conditional Statement](#statement)
1. [function](#functiontutorial)
1. [Loop in JS](#loop)

<a name='topAdv'></a>
<kbd>**JS Advanced Level Contents**</kbd>

_Please click to go to topic>>>>>_

1. [Scope in JS](#scope)
1. [JS String](#advanceString)
1. [JS Array](#array)
1. [JS Object](#object)


<kbd>**JS Fundamental Topics Details**</kbd>

_Please click for open details topic>>>>>_
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
- Traditional concatenation using the string (+) operator.
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


<a name='dataTypes'></a>

<details>

<summary>Data types</summary>
<h1>Data types</h1>
<button style='padding:3px; font-size:16px'>Learning summary</button>

- How many types of data
- list of primitive data type
- list of object data type
- Description of Number type data
- Description of string type data
- Rules of writing string type data
- Escape Character in string
- String–type-data with (Backtick) (`)
- Description of null type data
- Description of undefine type data
- Description of boolean type data
- Truthly and falsy value
- Description of Array type data
- Description of Object type data

> ***How many types of data***
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

> ***The typeof Operator:***

You can use the typeof operator to find the data type of a JavaScript variable.

### _Example:_

```js
typeof "John"                 // Returns "string"
typeof 3.14                   // Returns "number"
typeof NaN                    // Returns "number"
typeof false                  // Returns "boolean"
typeof [1,2,3,4]              // Returns "object"
typeof {name:'John', age:34}  // Returns "object"
typeof new Date()             // Returns "object"
typeof function () {}         // Returns "function"
typeof myCar                  // Returns "undefined" *
typeof null                   // Returns "object"
```
_Please observe:_

- The data type of NaN is number
- The data type of an array is object
- The data type of a date is object
- The data type of null is object
- The data type of an undefined variable is undefined *
- The data type of a variable that has not been assigned a value is also undefined *

[Go to top:arrow_up: ](#top)
</details>

<a name='operator'></a>

<details>
<summary>Operaotrs</summary>
<h1>Operators</h1>
<button style='padding:3px; font-size:16px'>Learning summary</button>

- Operators list
- Name of different part in operator
- Details about Arithmetic Operator
- Unary operator
- Binary operator
- Details about Comparison/Relational Operator
- Details about Logical Operator
- Details about Ternary/conditional operator
- Details about Assignment operator
- Details about String operator
- Details about Comma Operator

> ***Operators list:***

- Arithmetic Operator  
- Comparison/Relational Operator
- Logical Operator
- Ternary/conditional operator
- Assignment operator
- String operator
- comma operator
- Spread operator
- Rest Operator

> ***Name of different part in operator:***

let number = 2*3;  
- 2 and 3 is operand.
- (*) is operator.
-  2*3 all combindly call expression.

> ***Arithmetic Operator:***

- [+] - Addition
- [-] - Sustraction
- [*] - Multipication
- [**] - Exponentiation
- [/] - Division
- [%] - Modulus
- [++] - Increment
- [--] - Decrement  
Ther are two kinds of Arithmetic Operators:
> ***Unary operator:***

যে অপারেটর একটি অপারেন্ড নিয়ে কাজ করে তাকে Unary operator বলে। 
```js
let number = (-5); //(if use - call negation operator)
let count = (5);
```
> ***Binary operator:***

যে অপারেটর দুইটি অপারেন্ড নিয়ে কাজ করে তাকে Binary operator বলে।
```js
let number = (9-5);
let count = (5*3);
```
> ***Comparison/Relational Operator***

In JavaScript, you can use comparison operators to compare values which return true or false.
- [==] - equal to
- [===] - equal value and data type
- [!=] - not equal
- [!==] - not equal and type
- [>] - greater then
- [<] - small then
- [>=] - greater then or equal
- [<=] - small then and equal

> ***Example of comparison operator:***
```js
let x = 10;
let y = "10"
console.log(x==y); //true (value same)
console.log(x===y); //false (value same but data type different)
console.log(x != y);//false (value same)
console.log(x!==y); //true (value same but data type different)
console.log(x<=y); //true 
```
> ***Logical Operator (For check condition):***

The logical operator rule in JavaScript is used to combine two or more conditional statements together to create a more complex logical expression. There are three main logical operators in JavaScript: AND (&&), OR (||), and NOT (!).

> ***AND (&&) operator:***

If all side give true he return true and any side give false he return false:
```js
let x = 5;
let y = 10;

if (x > 3 && y > 9) {
   console.log("I am executed");
} 
// Output: "I am executed"
```
> ***OR (||) operator:***

If any side give true he return true and all side give false he return false:
```js
let a = 5;
let b = 10;

if (a > 8 || b <> 15) {
   console.log("I am executed");
} 
// Output: "I am executed"
```
> ***NOT(!) Operator:***

The NOT operator will negate the condition being evaluated. If the condition is true, it will return false, and if the condition is false, it will return true.
- !(true)-> Means false.
- !(false)-> Means true.
```js
let c = 15;

if (!(c > 20)) {
   console.log("c is not greater than 20");
} 
// Output: "c is not greater than 20"

```
> ***Ternary/conditional operator (same as if else):***

- condition ? "First Value" : "second value" (One dimensional)
- FirstCondition ? "First Value" : SecondCondition ? "third value" :"Fourth value"

-> If FirstCondition is true print First value and code execute off.  
-> if FirstCondition is false check secondCondition, If SeconCondition is true print Third value and code execute off.  
-> if First and second both are false print Fourth value.  
-> Same as if, else if, else.

The ternary operator in JavaScript is a shorthand way of writing an if-else statement. It takes the form of a question mark (?) followed by the value or expression to return if the condition is true, followed by a colon (:) followed by the value or expression to return if the condition is false.

For example, the following if-else statement:
```js
// By if else
if (x > 5) {
    result = "x is greater than 5";
} else {
    result = "x is less than or equal to 5";
}

//Can be written using the ternary operator as:

result = (x > 5) ? "x is greater than 5" : "x is less than or equal to 5";
```
In this example, if the condition (x > 5) is true, the expression on the left side of the colon will be returned (in this case, "x is greater than 5"). If the condition is false, the expression on the right side of the colon will be returned ("x is less than or equal to 5").

```js
// Multiple dimensional example
let score = 75;
let grade = (score >= 90) ? "A" : (score >= 80) ? "B" : (score >= 70) ? "C" : (score >= 60) ? "D" : "F";
console.log(grade); // Output: "C"
```

> ***short-circuit operator:***

> ***short-circuit AND (&&) Operator:***

The short-circuit behavior of the && operator means that the second operand is only execute if the first operand is truthy. 
```js
//--------AND (&&)----------------
console.log(10>9 && 90); //90
console.log(10<9 && 90); //false
console.log(10>9 && 9>4 && 2+3); //5
console.log(10>9 && 9<4 && 2+3); //false

const firstOperand = true;
const secondOperand = () => console.log('This function is called');

firstOperand && secondOperand(); // This function is called
```
> ***short-circuit OR (||) Operator:***

- If the left operand is falsy, the operator execute the right operand and returns that value.
- If the right operand is falsy, the operator execute the left operand and returns that value.
- if left is true then code executed true code and off advance.
```js
//--------OR (||)----------------
console.log(10>9 || 90); //true
console.log(10<9 || 90); //90
console.log(10>9 || 9>4 || 2+3); //true
console.log(10<9 || 9<4 || 2+3); //5

let amount =500;
console.log(amount || 100);//500

let amount =0;
console.log(amount || 100);//100
```
> ***nullish coalescing operator:***

The ?? operator (also known as the "nullish coalescing operator") is used in JavaScript to check if a value is null or undefined, and if so, provide a default value. Here is an example of how it can be used:
```js
let userName = "John Smith";
let defaultName = "Guest";

console.log(userName ?? defaultName); // prints "John Smith"

userName = null;
console.log(userName ?? defaultName); // prints "Guest"

userName = undefined;
console.log(userName ?? defaultName); // prints "Guest"
```

Note that the ?? operator only checks for null and undefined values, and will not check for other "falsy" values like 0 or an empty string. If you want to check for all falsy values, you can use the || operator instead.

> ***Difference between operators:***

- Logical operator check condition and return true of false.
- Ternary operator work as else if.
- short circuit operator return both side code depands on condition.

> ***combined use logical and ternary operator:***

```js
let result=0;
let grade = result > 70 && result < 80 ? "A" : result > 80 && result < 90 ? "A+":"Fail";
console.log(grade)
```
> ***Assignment operator (=)***
```js
let x = 10;
x+=5; //x=x+5 (value re-assign) - result=15
x*=2 //x=x*2 result = 30
x++; // x=x+1 result =31
x--; // x=x-1 result = 30
```
> ***String operator (+)***

In JavaScript, the + operator is used to concatenate.
```js
let greeting = 'Hello' + ' ' + 'world';
console.log(greeting);  // Output: "Hello world"

let greeting = 'Hello';
greeting += ' world';
console.log(greeting);  // Output: "Hello world"
```
> ***Comma Operator (,)***

The comma operator is use for print multiple expression value separetly.
```js
let x = 10;
let y=4;
console.log(x++, Y--);
```
> ***Operator presedency (অপারেটরের অগ্রাধিকার)***

> ***What is operator presendence:***

Operator precedence describes the order in which operations are performed in an arithmetic expression.  
- একটি expression এর মধ্যে যদি একাধিক অপারেটর থাকে তাহলে অপারেটরগুলোর মধ্যে যার presedency বা অগ্রাধিকার বেশি সে আগে কাজ করবে। নিচের এক্সপ্রেশনে মাল্টিপিকেশন এর অগ্রাধিকার বেশি তাই আগে মাল্টিপিকেশন হয়ে তারপর প্লাস হয়েছে। 
```js
let number = 2+3*5; //Result - 17
``` 
- নিচের এক্সপ্রেশনে প্যারানথিসিস () রয়েছে যার অগ্রাধিকার সবচেয়ে বেশি তাই সে আগে কাজ করে তারপর মাল্টিপিকেশন কাজ করেছে।
```js
let number = (2+3)*(5-1); //Result - 20
``` 
- নিচের এক্সপ্রেশনে অপারেটরগুলোর অগ্রাধিকার সমান থাকায় বাম থেকে ডানে কাজ করেছে।
```js
let number = 2+3-1; //Result - 4
let number = 2*3/2; //Result - 3
```  
- operator presendence value:
[Click for see operator presendence value ](https://www.w3schools.com/js/js_precedence.asp)

[Go to top:arrow_up: ](#top)
</details>

<a name='statement'></a>

<details>
<summary>Conditional Statement</summary>

<h1> Control Statement </h1>
<button style='padding:3px; font-size:16px'>Learning Summary</button>

- if, else if, else
- switch

> ***if, else if, else***

``` js
if (FirstCondition){  
    FirstCode
}else if(SecondCondition){
    SecondCode
}else{
    ThirdCode
}
```
- যদি FirstCondition কন্ডিশন সত্য হয় তাহলে FirstCode কোড এক্সিকিউট হবে এবং প্রোগ্রাম বন্ধ হয়ে যাবে।
- যদি FirstCondition কন্ডিশন মিথ্যা হয় তাহলে SecondCondition চেক হবে যদি সত্য হয় তাহলে SecondCode কোড এক্সিকিউট হবে এবং প্রোগ্রাম বন্ধ হয়ে যাবে।
- যদি উভয় কন্ডিশন মিথ্যা হয় তাহলে ThirdCode কোড এক্সিকিউট হবে। 

#### _Example_
```js
    let age =prompt("Type your age:");
if (age>=50 && age<=80) {
    console.log ("old!!!")
} else if (age>=40 && age<50) {
    console.log ("middle year")
}
else if (age>=18 && age<40) {
    console.log ("Young")
} else {
    console.log("baby")
}
```
> ***Switch***

_Syntax:_  
```js
switch(RcvVaribale) {
  case value1: //Condition check between value and variable
    // if true execute code block
    break;
  case value2:
    // code block
    break;
  default:
    // code block
}
```
- case  -> check with variable if true then execute and programme break.
- if no case it match with variable execute default value.

### _Example:_
```js
 let input = prompt("Enter Alphabet for check:")
        input.toLowerCase;

        switch (input) {
            case "a": 
            Result="vowel" 
            break;
            case "e": Result="vowel"
            break;
            case "i": Result="vowel"
            break;
            case "o": Result="vowel"
            break;
            case "u": Result="vowel"
            break;
            default: Result="Consonent"

/* If Same case write together*/
            case "a":
            case "e":
            case "i":
            case "o":
            case "u": Result = "vowel"
                break;
            default: Result = "Consonent"
        }
        console.log(Result)
```
[Go to top:arrow_up: ](#top)
</details>

<a name='functiontutorial'></a>
<details>
<summary>function</summary>
<h1>function</h1>

<button style='padding:3px; font-size:16px;'>Learning Summary </button>

- What is function
- Processedure of Define and call function
- What is parameter and argument
- return statement in function
- deceleration vs expression in JavaScript function

> ***What is function:***

In JavaScript, a function is a block of code that performs a specific task. It can be defined and then called by name. Functions can take input in the form of parameters, and they can also return output in the form of a return value.

> ***Processedure of Define and call function:***

```js
// Without Parameter define function
function student(){
    const name = "Anamul";
    console.log(name)
};
//Without argument call function
student(); //output - Anamul
```
> ***What is parameter and argument***

- In JavaScript, a parameter is a variable that is used in a function definition. When a function is called, the values that are passed in as arguments are used to initialize the function's parameters.
- In JavaScript, an argument is a value that is passed to a function when the function is called. The function can then use the argument(s) in its calculations and return a result.
- You can also define a function that takes multiple arguments by separating the argument names with commas.

```js
// With Parameter define function
function greet(firstName, lastName) {
  console.log(`Hello ${firstName} ${lastName}!`);
}
// With argument call function
greet('Anamul', 'Haque');  // prints "Hello Anamul Haque!"
```
> ***return statement in function:***

In JavaScript, the return statement is used to specify the value that a function should return when it is called. When a function is called, it will execute the code within its body and then return a value. This value can be a literal value (such as a number or a string), an expression, or even another function. without rerurn do not get data when function is called.

Here is an example of a function that uses the return statement to return a value:

```js
function multiply(a, b) {
  return a * b;
}

let result = multiply(3, 4);  // returns 12
```
In this example, the multiply function takes two arguments, a and b, and returns the product of the two. When the function is called with the arguments 3 and 4, it returns the value 12.

It's important to note that the return statement ends the execution of the function and returns a value to the caller. Any code after the return statement will not be executed.
```js
function add(a, b) {
  return a + b;
  console.log('This line will not be executed');
}
```
> ***deceleration vs expression in JavaScript function:***

In JavaScript, a function declaration is a way of defining a function with a given name and function body. It has the following syntax:
```js
function functionName(parameters) {
  // function body
}
```
On the other hand, a function expression is a way of defining a function as part of a larger expression, such as a variable assignment or an object property. It has the following syntax:
```js
const functionName = function(parameters) {
  // function body
};
```
[Go to top:arrow_up: ](#top)
</details>

<a name='loop'></a>

<details>
<summary>Javascript Loop </summary>
<h1> JAVASCRIPT LOOP </h1>

<button>Learning Summary</button>

- What is loop in JavaScript
- How many types of loop in JavaScript
- Details about while loop
- Details about do-while loop
- Details about for loop
- Details about for-in loop
- Details about for-of loop


> ***What is loop in JavaScript:***

In JavaScript, a loop is a control structure that allows you to repeat a block of code a certain number of times or until a certain condition is met. There are several types of loops in JavaScript, including:

> ***How many types of loop in JavaScript:***

There are several types of loops in JavaScript, including:
- for loop
- for-in loop
- for-of-loop
- while loop
- do-while loop

 > ***Details about while loop:***

A while loop in JavaScript will execute a block of code as long as a specified condition is true. Here is the basic syntax for a while loop:
```js
while (condition) {
  //if condition is true code block to be executed
}
```
Here is an example of a while loop that counts from 0 to 9:
```js
let count = 0;

while (count < 10) {
  console.log(count);
  count++;
}
// output - 0 through 9
```
This will output the numbers 0 through 9 to the console. The count++ statement increments the value of count by 1 each time the loop runs. When the value of count is no longer less than 10, the loop will terminate.

It's important to make sure that the condition in the while loop will eventually evaluate to false, or the loop will run indefinitely, which is known as an infinite loop.

> ***Details about do-while loop***

A do-while loop is a loop that will execute its code block at least once, and then repeat the block as long as a given condition is true. Here is the syntax for a do-while loop in JavaScript:
```js
do {
  // code block to be executed
} while (condition);
```
The do-while loop is similar to a while loop, except that the do-while loop will always execute the code block at least once, regardless of the value of the condition. The condition is then checked at the end of each iteration, and if it is true, the loop will continue to run. If the condition is false, the loop will exit and control will be passed to the next statement in the program.

Here is an example of a do-while loop that counts from 1 to 10:
```js
let i = 1;
do {
  console.log(i);
  i++;
} while (i <= 10);
```
This loop will first execute the code block with i equal to 1, then it will check the condition i <= 10. Since 1 is less than or equal to 10, the loop will continue to run and i will be incremented to 2. The loop will then check the condition again, and since 2 is still less than or equal to 10, the loop will continue to run. This process will repeat until i is equal to 11, at which point the condition will be false and the loop will exit.

> ***Details about for loop***

In JavaScript, you can use a for loop to iterate over the elements in an array or to repeat a block of code a certain number of times.
Here is an example of a for loop in JavaScript:
```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```
This will print out the numbers 0 through 4 to the console. Here's how it works:

- The initialization statement let i = 0 initializes the loop and creates a variable i that will be used to track the progress of the loop.
- The condition i < 5 specifies the loop should continue as long as i is less than 5.
- The increment statement i++ increases the value of i by 1 each time the loop runs.

You can also use a for loop to iterate over an array. Here's an example:
```js
const arr = [1, 2, 3, 4, 5];

for (let i = 0; i < arr.length; i++) {
  console.log(arr[i]);
}
```
This will print out each element in the arr array to the console.

> ***Details about for-in loop***

A for-in loop is a loop that iterates over the properties of an object. Here is an example of a for-in loop in JavaScript:
```js
const object = {a: 1, b: 2, c: 3};

for (const property in object) {
    console.log(property) // property print
    console.log(object[property) // value print
    console.log(`${property}: ${object[property]}`);
}
```
This will output:
```js
a: 1
b: 2
c: 3
```
The for-in loop is different from the for loop, which is used to iterate over an array or a range of numbers.

> ***Details about for-of loop***

The for-of loop is a looping construct introduced in ECMAScript 6 that allows you to iterate over iterable objects such as arrays, strings, and maps. It works by calling the Symbol.iterator method on the object being iterated over, and then repeatedly calling the next() method of the iterator object until the done property of the returned object is true.

Here is an example of using a for-of loop to iterate over the characters in a string:
```js
const str = 'hello';

for (const c of str) {
  console.log(c);
}
```
This will log each character in the string to the console:
```js
h
e
l
l
o
```
You can also use a for-of loop with an array:
```js
const arr = [1, 2, 3, 4, 5];

for (const element of arr) {
  console.log(element);
}
```
This will log each element in the array to the console:
```js
1
2
3
4
5
```
Note that the for-of loop does not give you access to the index of the current element like a for loop does. If you need to access both the element and its index, you can use the for-of loop in conjunction with the Array.prototype.entries() method, which returns an iterator that yields an array containing the index and value of each element in the array:
```js
const arr = [1, 2, 3, 4, 5];

for (const [index, element] of arr.entries()) {
  console.log(`${index}: ${element}`);
}
```
This will log the index and element of each element in the array to the console:
```js
0: 1
1: 2
2: 3
3: 4
4: 5
```
[Go to top:arrow_up: ](#top)

</details>


<kbd>**JS Advanced Lavel Topics Details**<kbd>

_Please click for open details topic>>>>>_

<a name='scope'></a>

<details>
<summary>JS Scope</summary>
<h1>JS Scope</h1>

<kbd>Learning Summary<kbd>

- What is Scope
- Global Scope
- Local Scope
- example of global and local scope

> ***What is Scope?***

In JavaScript, scope refers to the accessibility or visibility of variables, functions, and objects in some particular part of your code during runtime. Scopes can be global or local.

> ***Global Scope:***

 Variables declared outside of any function have global scope, which means they can be accessed by any script on the page.
 
 > ***Local Scope:***

  Variables declared within a function have local scope, which means they can only be accessed within that function. variables and functions.

 > _example of global and local scope in JavaScript:_

```js
// variable declared outside of any function has global scope
var globalVariable = "I am a global variable";

function myFunction() {
  // variable declared within a function has local scope
  var localVariable = "I am a local variable";
  
  console.log(globalVariable); // "I am a global variable"
  console.log(localVariable); // "I am a local variable"
}

console.log(globalVariable); // "I am a global variable"
console.log(localVariable); // ReferenceError: localVariable is not defined
```
In this example, the variable `globalVariable` is declared outside of any function, so it has global scope and can be accessed by any script on the page. The variable `localVariable` is declared within the function myFunction, so it has local scope and can only be accessed within that function. If you try to access the `localVariable` outside of the function myFunction, you will get a ReferenceError.

It's important to understand that when a variable is defined with let or const inside a block, it will have a block scope instead of a function scope.

```js
if(true){
    let x = 1;
}
console.log(x);  // ReferenceError
```
In this case, the variable `x` is block scoped and can only be accessed within the block.

[Go to top:arrow_up: ](#topAdv)
</details>

<a name='advanceString'></a>
<details>
<summary>JS String</summary>
<h1>JS string</h1>

JS string is a data type in JavaScript that represents a sequence of characters, such as words or sentences.
string can be concatenated, manipulated, and accessed using various string methods and properties.

<kbd>Learning Summary</kbd>

> ***JavaScript String Methods list:***

- String length
- String slice()
- String substring()
- String substr()
- String replace()
- String replaceAll()
- String toUpperCase()
- String toLowerCase()
- String concat()
- String trim()
- String trimStart()
- String trimEnd()
- String padStart()
- String padEnd()
- String charAt()
- String charCodeAt()
- String split()

> ***JavaScript String Search Methods list:***

- String indexOf()
- String lastIndexOf()
- String search()
- String match()
- String matchAll()
- String includes()
- String startsWith()
- String endsWith()


_Please click for open details topic>>>>>_

<details>
<summary>Details about JavaScript String Methods</summary>

<h1>Details about JavaScript String Methods</h1>

### **String length**
---
In JavaScript, you can use the `.length` property of a string to determine its length. For example:
```js
let myString = "hello";
let stringLength = myString.length;
console.log(stringLength); // outputs 5
```
The `.length` property returns the number of characters in the string, including spaces and special characters.

### **String slice()**
---
In JavaScript, the `slice()` method is used to extract a section of a string and return it as a new string. The method takes two arguments: the starting index and the ending index (optional) of the section to be extracted. The original string is not modified.

### _Syntax:_

```js
string.slice(start, end)
```

_Start_: The index at which to begin the extraction (inclusive).  
_End_: The index at which to end the extraction (exclusive).

### _For example:_
```js
let str = "Hello World!";
let res = str.slice(0, 5);
console.log(res); // Output: "Hello"
```
In this example, the slice method extracts a substring from the original string "Hello World!" starting at index 0 (inclusive) and ending at index 5 (exclusive), resulting in the substring "Hello".

### **String substring()**
---
- The substring() method returns a new string that is a substring of the original string. 
- It takes two arguments, start and end, which represent the starting and ending index of the substring.
- If the start index is greater than the end index, the method will swap the values.It does not include the character at the end index. It is the different between `Slice()` Method.

### _Example:_
```js
let str = "Hello World";
let sub = str.substring(0, 5); // "Hello"
let sub = str.substring(5, 0); // "Hello" swap value
```
In this example, we are trying to extract a substring from index 5 to index 0. However, since the start index (5) is greater than the end index (0), the substring() method automatically swaps the values, so the resulting substring is actually from index 0 to index 5, which is "Hello".

### **String substr()**
---
In JavaScript, the `substr()` method is used to extract a specified number of characters from a string, starting at a specified index. The method takes two parameters: the starting index and the number of characters to extract. For example, the following code would extract the substring "world" from the string "hello world":

```js
let str = "hello world";
let sub = str.substr(6, 5);
console.log(sub); // Output: "world"
```
### ***String replace()***
---
In JavaScript, the `replace()` method is used to replace a specified value with another value in a string. The method takes two arguments: the value to be replaced, and the replacement value.

Here is an example of how to use the replace() method to replace all instances of the word "world" with the word "javascript":

```js
let str = "Hello world, welcome to the world of programming";
let newStr = str.replace("world", "javascript");
console.log(newStr); // Output: "Hello javascript, welcome to the javascript of programming"
```

The `replace()` method can also take a regular expression as its first argument, which allows for more powerful search-and-replace operations. Here is an example of how to use a regular expression to replace all occurrences of the word "world" (regardless of case) with the word "javascript":

```js
let str = "Hello World, welcome to the World of programming";
let newStr = str.replace(/world/i, "javascript");
console.log(newStr); // Output: "Hello javascript, welcome to the javascript of programming"
```

Note that the replace() method only replaces the first occurrence of the search value if it is a string, but if it is a regular expression with the global flag, it will replace all occurrences.

### **String replaceAll()**
---
JavaScript does not have a replaceAll() method built-in to the String object. However, you can use the replace() method with a regular expression and the global g flag to replace all occurrences of a specified value in a string. Here is an example of how to use the replace() method with a regular expression to replace all occurrences of the word "world" (regardless of case) with the word "javascript":

```js
let str = "Hello World, welcome to the World of programming";
let newStr = str.replace(/world/gi, "javascript");
console.log(newStr); // Output: "Hello javascript, welcome to the javascript of programming"
```
The `g` flag tells the regular expression to replace all matches, and the `i` flag to make the search case-insensitive.

### **String toUpperCase()**
---
In JavaScript, the toUpperCase() method is used to convert all the characters in a string to uppercase letters. Here is an example of how to use the `toUpperCase()` method:

```js
let str = "hello world";
let upperStr = str.toUpperCase();
console.log(upperStr); // Output: "HELLO WORLD"

This method does not take any arguments and returns a new string with all the characters in uppercase.
```
### **String toLowerCase()**
---
In JavaScript, the `toLowerCase()` method is used to convert all the characters in a string to lowercase letters. Here is an example of how to use the toLowerCase() method:

```js
let str = "HELLO WORLD";
let lowerStr = str.toLowerCase();
console.log(lowerStr); // Output: "hello world"
```

### **String concat()**
---
In JavaScript, the `concat()` method is used to join two or more strings together. The method takes one or more strings as arguments, and returns a new string that is the concatenation of the input strings. Here is an example of how to use the concat() method to join two strings together:
```js
let str1 = "Hello";
let str2 = "World";
let newStr = str1.concat(" ", str2);
console.log(newStr); // Output: "Hello World"
```

### **String trim()**
---
In JavaScript, the `trim()` method is used to remove whitespace from the beginning and end of a string. The method does not take any arguments, and returns a new string with the whitespace removed. Here is an example of how to use the `trim()` method:

```js
let str = "   Hello World    ";
let newStr = str.trim();
console.log(newStr); // Output: "Hello World"
```
It's worth noting that the trim() method does not modify the original string, it creates a new string with the leading and trailing whitespace removed.

### **String trimStart()**
---
In JavaScript, the `trimStart()` method is used to remove whitespace from the beginning of a string. The method does not take any arguments and returns a new string with the leading whitespace removed. This method was introduced in ECMAScript2019 and it is not widely supported.

Here is an example of how to use the trimStart() method:

```js
let str = "   Hello World    ";
let newStr = str.trimStart();
console.log(newStr); // Output: "Hello World    "
```

### **String trimEnd()**
---
In JavaScript, the `trimEnd()` method is used to remove whitespace from the end of a string. The method does not take any arguments and returns a new string with the trailing whitespace removed. This method was introduced in ECMAScript2019 and it is not widely supported.

Here is an example of how to use the trimEnd() method:
```js
let str = "   Hello World    ";
let newStr = str.trimEnd();
console.log(newStr); // Output: "   Hello World"
```
### **String padStart(), padEnd()**
---
In JavaScript, the `.padStart()` method can be used to pad the beginning (i.e. the left side) of a string with a specified character or set of characters. The method takes two arguments: the first is the total length of the final padded string, and the second is the character or set of characters to use for padding. For example:

```js
let str = "hello";
str = str.padStart(10, '*');
console.log(str); // Output: "*****hello"
```

This will output `"*****hello"` because the original string `"hello"` is padded with 5 * characters on the left side to reach a total length of 10 characters.

You can also use `padEnd` method to pad the end of the string.

```js
let str = "hello";
str = str.padEnd(10, '*');
console.log(str); // Output: "hello*****"
```
Please note that .padStart() and .padEnd() was introduced in ES2017, this means that it's not supported by all browsers.

### ***String charAt()***
In JavaScript, the `.charAt()` method can be used to retrieve a specific character from a string at a given index. The method takes one argument, which is the index of the character you want to retrieve. The index starts at 0 for the first character, 1 for the second character, and so on. For example:

```js
let str = "hello";
let firstChar = str.charAt(0);
console.log(firstChar); // Output: "h"
```
This will output "h" because the .charAt() method is used to retrieve the character at index 0 of the string "hello".

You can also use bracket notation to get the character of string at specific index.

```js
let str = "hello";
let firstChar = str[0];
console.log(firstChar); // Output: "h"
```

Please note that if you pass an index that is out of bounds of the string, .charAt() will return an empty string.

### **String split()**
---
In JavaScript, the `.split()` method can be used to split a string into an array of substrings based on a specified separator. The method takes one argument, which is the separator used to split the string. For example:

```js
let str = "hello, world";
let words = str.split(', ');
console.log(words); // Output: ["hello", "world"]
```
This will output ["hello", "world"] because the .split() method is used to split the string "hello, world" into an array of substrings using the separator ", " (a comma followed by a space).

You can also use an empty string as separator to split the string by each character.

```js
let str = "hello";
let letters = str.split('');
console.log(letters); // Output: ["h", "e", "l", "l", "o"]
```
If no separator is specified, the .split() method will use whitespace as the separator.

```js
let str = "hello world";
let words = str.split();
console.log(words); // Output: ["hello", "world"]
```

You can also specify a limit for the number of splits that the method should perform using the second argument.

```js
let str = "a-b-c-d-e";
let words = str.split('-',3);
console.log(words); // Output: ["a", "b", "c-d-e"]
```
This will output `["a", "b", "c-d-e"]` because the `.split()` method is used to split the string `"a-b-c-d-e"` into an array of substrings using the separator "-" and it will only split 3 times.
</details>

<details>
<summary>Details about JS String Search Methods</summary>

<h1>Details about JS String Search Methods</h1>

### **String indexOf()**
---
In JavaScript, the `.indexOf()` method can be used to find the first occurrence of a specified value in a string and returns the index of that value or -1 if the value is not found. The method takes one argument, which is the value that you want to find in the string. For example:

```js
let str = "hello world";
let index = str.indexOf('world');
console.log(index); // Output: 6
```

This will output 6 because the `.indexOf()` method is used to find the first occurrence of the string `"world"` in the string `"hello world"` and returns the index of the first character of that substring (6)

You can also pass a second argument to the `.indexOf()` method to specify the position in the string where the search should start.

```js
let str = "hello world";
let index = str.indexOf('o', 4);
console.log(index); // Output: 7
```

This will output `7` because the `.indexOf()` method is used to find the first occurrence of the letter `"o"` starting from the index `4` in the string `"hello world"` and returns the index of the first character of that substring `(7)`

If the value is not found, the method will return `-1`.

```js
let str = "hello world";
let index = str.indexOf('xyz');
console.log(index); // Output: -1
```

Please note that `.indexOf()` is case-sensitive and it only returns the first occurrence of the value, if you want to find all occurrences of the value in the string, you should consider using regular expressions with `.match()` or `.search()` method.

### **String lastIndexOf()**
---
In JavaScript, the `.lastIndexOf()` method is similar to the .indexOf() method, but it finds the last occurrence of a specified value in a string, instead of the first one. The method takes one argument, which is the value that you want to find in the string. For example:

```js
let str = "hello world, hello";
let index = str.lastIndexOf('hello');
console.log(index); // Output: 14
```

This will output 14 because the `.lastIndexOf()` method is used to find the last occurrence of the string "hello" in the string `"hello world, hello"` and returns the index of the first character of that substring `(14)`

You can also pass a second argument to the `.lastIndexOf()` method to specify the position in the string where the search should start from the end of the string.

```js
let str = "hello world, hello";
let index = str.lastIndexOf('o', 15);
console.log(index); // Output: 7
```

This will output 7 because the `.lastIndexOf()` method is used to find the last occurrence of the letter `"o"` starting from the index `15` (counting from the end) in the string `"hello world, hello"` and returns the index of the first character of that substring `(7)`

If the value is not found, the method will return `-1`.

```js
let str = "hello world";
let index = str.lastIndexOf('xyz');
console.log(index); // Output: -1
```

Please note that `.lastIndexOf()` is case-sensitive and it only returns the last occurrence of the value, if you want to find all occurrences of the value in the string, you should consider using regular expressions with `.match()` or `.search()` method.

### **String search()**
---
In JavaScript, the `.search()` method can be used to find the first occurrence of a specified regular expression in a string and returns the index of that match or -1 if no match is found. The method takes one argument, which is the regular expression that you want to use to search for a match in the string. For example:

```js
let str = "hello world";
let index = str.search(/world/);
console.log(index); // Output: 6
```

This will output 6 because the `.search()` method is used to find the first occurrence of the regular expression `/world/` in the string `"hello world"` and returns the index of the first character of that match `(6)`

You can also use the `.search()` method with a string that represents the regular expression.

```js
let str = "hello world";
let index = str.search("world");
console.log(index); // Output: 6
```

If no match is found, the method will return `-1`.

```js
let str = "hello world";
let index = str.search(/xyz/);
console.log(index); // Output: -1
```

The `.search()` method can be useful when you want to find a match of a specific pattern in a string, it's faster than using `.indexOf()` or `.lastIndexOf()` when you are working with regular expressions.

Please note that `.search()` is also case-sensitive, if you want to perform a case-insensitive search, you can use the `i` flag in your regular expression.

```js
let str = "Hello world";
let index = str.search(/hello/i);
console.log(index); // Output: 0
```

### **String match()**
---
The `match()` method in JavaScript is used to search a string for a match against a regular expression, and returns the matched substring. The method returns an array containing the matched results, or null if no match is found.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.match(/ain/gi);
console.log(res); // Output: ["ain", "ain", "ain"]
```

The `match()` function takes a regular expression as its argument and returns an array of all the matches found in the string. The `g` flag is used to perform a global search, and `i` is used to perform a case-insensitive search.

Note that match() only returns the first match if the global flag is not used.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.match(/ain/);
console.log(res); // Output: ["ain"]
```

### **String matchAll()**
`matchAll()` is a JavaScript method that allows you to iterate over all matches of a regular expression in a string, rather than just the first match. The method returns an iterator object that you can use to access the matched substrings.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let regex = /ain/gi;
let matches = str.matchAll(regex);
for (const match of matches) {
  console.log(match);
}

//Output:

["ain", index: 5, input: "The rain in SPAIN stays mainly in the plain"]
["ain", index: 10, input: "The rain in SPAIN stays mainly in the plain"]
["ain", index: 28, input: "The rain in SPAIN stays mainly in the plain"]
```
The result of each match is an array that has the matched string, the index of the match, and the input string.

### **String includes()**
---
The `includes()` method in JavaScript is used to check if a string contains a specified substring. The method returns a Boolean value indicating whether the substring is found within the string.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.includes("Spain");
console.log(res); // Output: false
```

You can also specify a starting index for the search using the second argument to the `includes()` method:

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.includes("in",5);
console.log(res); // Output: true
```

In this example, the search for the substring `"in"` starts at the index `5`, so the method returns true because the substring `"in"` is found at index 10.

The `includes()` method is case-sensitive, so it will not match substrings that have a different case.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.includes("Spain");
console.log(res); // Output: false
```
It is important to note that includes() method is available in all modern browser and also in Node.js environments.

### **String startsWith()**
---
The `startsWith()` method in JavaScript is used to check if a string begins with a specified substring. The method returns a Boolean value indicating whether the string starts with the specified substring.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.startsWith("The");
console.log(res); // Output: true
```
You can also specify a starting index for the search using the second argument to the `startsWith()` method:

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.startsWith("in",5);
console.log(res); // Output: false
```
In this example, the search for the substring `"in"` starts at the index `5`, so the method returns false because the substring `"in"` is not at the beginning of the string.

The `startsWith()` method is case-sensitive, so it will not match substrings that have a different case.
```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.startsWith("the");
console.log(res); // Output: false
```
It is important to note that startsWith() method is available in all modern browser and also in Node.js environments.

### **String endsWith()**
---
The `endsWith()` method in JavaScript is used to check if a string ends with a specified substring. The method returns a Boolean value indicating whether the string ends with the specified substring.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.endsWith("plain");
console.log(res); // Output: true
```
You can also specify a ending index for the search using the second argument to the `endsWith()` method:

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.endsWith("in",27);
console.log(res); // Output: false
```

In this example, the search for the substring `"in"` ends at the index 27, so the method returns false because the substring `"in"` is not at the end of the string.

The `endsWith()` method is case-sensitive, so it will not match substrings that have a different case.

```js
let str = "The rain in SPAIN stays mainly in the plain";
let res = str.endsWith("Plain");
console.log(res); // Output: false
```
It is important to note that endsWith() method is available in all modern browser and also in Node.js environments.
</details>

[Go to top:arrow_up: ](#topAdv)
</details>


<a name='array'></a>

<details>
<summary>JS Array</summary>
<h1>Array</h1>

<kbd>Learning Summary<kbd>

- Counting value from nested array
- Counting value from Array into object
- Counting value from object into Array
- The .length method
- Add, Replace and delete methods
  - By indexing
  - push()
  - pop()
  - shift()
  - unShift()
- Array concate
- Array Sorting
  - sort(Accending)
  - sort(Deaccending)
- The Sets data Structure in JS
  - Essential Set Methods & Properties
  - Create Set and use its methods
- Array Destructruing
- The forEach() Method
- The forEach() method in Set
- The map() method
- The filter() Method
- The Filter() & Map() use together
- The reduce() Mehtod
- chaining filetr(), map() and reduce() method

     

> ***Counting value from nested array***
```js
let city =['Dhaka', 'Sylhet',['Rangpur', 'Pabna']]
// count Rangpur = city[2][0]
// count Pabna = city[2][1]
```
> ***Counting value from Array into object***
```js
let arr = ["Dhaka", "Sylhet",["Narsingdi", "Hasnabad"],{Pop: "one", set:["Anam", "Rafiq"],}, "Vola"];
//count pop = arr[3]["pop"] or arr[3].pop
//count Rafiq = arr[3]["set"][1]
```
> ***Counting value from object into Array***
```js
let bio_data = {Name:"Anam", age:["12","45"]};
//count 12 = bio_data["age"][0] or bio_data.age[0]
```
> ***Add, Replace and delete methods:***
```js
// Change value by index
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries[2] = "china" 
alert (countries);
//Output:["Bangladesh", "India", "china"]

// Add value by index
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries[3] = "Norway" 
alert (countries);
//output:["Bangladesh", "India", "Pakistan","Norway" ]

// Add value at last by measuring Arrays length 
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries [countries.length] = "Malaysia"; 
alert (countries);
//outpue:["Bangladesh", "India", "Pakistan","Malaysia" ]

//Push value at last by push() method
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries.push("Malaysia", “Northland”); 
console.log (countries);
//Output:["Bangladesh", "India", "Pakistan", "Malaysia", “Northland”]

//Delete last value by pop() method
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries.pop();
console.log (countries);
//Outpue:["Bangladesh", "India"]

// Delete first value by shift() method
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries.shift();
console.log (countries);
//Output: ["India", "Pakistan"]

//Add value in first index by unShift() method
let countries = ["Bangladesh", "India", "Pakistan"]; 
countries.unshift("Malaysia", “Northland”); 
console.log (countries);
```
> ***Array concate***
```js
let countries = ["Bangladesh is our country"]; 
let myName = ["Anamul"]
let decide =myName.concat(countries);
console.log (decide);
//result:  [ "Anamul", "Bangladesh is our country" ] 
```
> ***sort(Accending)***
```js
let countries = ["Bangladesh", "India","Pakistan", "Malaysia" ]; 
countries = countries.sort();
console.log (countries);
//result:   [ "Bangladesh", "India", "Malaysia", "Pakistan" ]
```
> ***sort(Deaccending)***
```js
let countries = ["Bangladesh", "India","Pakistan", "Malaysia" ]; 
countries = countries.reverse();
console.log (countries);
//result:   ["Pakistan", "Malaysia", "India", "Bangladesh" ]
```

# The Sets data Structure in JS
A JavaScript Set is a collection of unique values.
Each value can only occur once in a Set.

> ***Essential Set Methods & Properties:***
- new Set() -	Creates a new Set
- add() -	Adds a new element to the Set
- delete() -	Removes an element from a Set
- has() -	Returns true if a value exists in the Set
- forEach() -	Invokes a callback for each element in the Set
- values() - Returns an iterator with all the values in a Set
- size - Returns the number of elements in a Set

> ***How to Create a Set***

You can create a JavaScript Set by:

  - Passing an Array to new Set()
  - Create a new Set and use add() to add values
  - Create a new Set and use add() to add variables

```js
//Passing an Array to new Set()
const data = new Set(["1", "2", "3"]);
console.log(data); //Set(3) [ "1", "2", "3" ]

//Create a new Set and use add() to add values
const data1 = new Set();
data1.add(["Orange", "Apple", "Banana"]);
data1.add("Malta");
console.log(data1) //Set [ (3) […], "Malta" ]

//Create a new Set and use add() to add variables
const data2 = new Set();

let a = "Pen";
let b = "Book";

data2.add(a);
data2.add(b);
console.log(data2); //Set [ "Pen", "Book" ]
```
## Array Destructruing

In JavaScript, destructuring is a way to unpack values from arrays, or properties from objects, into distinct variables.

For arrays, you can use the array destructuring syntax to assign items in the array to separate variables.
For example, consider the following array:
- Array destructure by []
- Destructuring array and assigning variable serially.
```js
let arr = [1, 2, 3, 4, 5];
```
You can unpack the values of the array into separate variables like so:
```js
let [a, b, c, d, e] = arr;
console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
console.log(d); // 4
console.log(e); // 5
```
You can also skip certain elements by leaving out the variable name.
```js
let [a, ,c, , e] = arr;
console.log(a); // 1
console.log(c); // 3
console.log(e); // 5
```
You can also use the rest operator (...) to capture all remaining elements into an array.
```js
let [a, b, ...rest] = arr;
console.log(a); // 1
console.log(b); // 2
console.log(rest); // [3, 4, 5]
```
You can also do array destructuring and assign a value by default if the array have undefined value
```js
let arr = [1, 2, 3, 4, 5];
let [a=0, b=0, c=0, d=0, e=0, f=100] = arr;
console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
console.log(d); // 4
console.log(e); // 5
console.log(f); // 100
```
In JavaScript, you can destruct a nested array by using nested destructuring assignments. Here's an example:
```js
let nestedArray = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];

let [ [a, b, c], [d, e, f], [g, h, i] ] = nestedArray;

console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
console.log(d); // 4
console.log(e); // 5
console.log(f); // 6
console.log(g); // 7
console.log(h); // 8
console.log(i); // 9
```
```js
let nestedArray = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];

let [ [a, b], [d, e, f], [g, ...rest] ] = nestedArray;

console.log(a); // 1
console.log(b); // 2
console.log(d); // 4
console.log(e); // 5
console.log(f); // 6
console.log(g); // 7
console.log(rest); // [8, 9]
```
To destruct an array from an object in JavaScript, you can use the destructuring assignment syntax.
```js
// 1st System
const obj = {
  array: [1, 2, 3]
};

const { array: [elem1, elem2, elem3] } = obj;
console.log(elem1); // 1
console.log(elem2); // 2
console.log(elem3); // 3

// 2nd System
const  [elem1, elem2, elem3] = obj["array"];
```
To destruct an array from a method in JavaScript, you can use the destructuring assignment syntax.
```js
// Method that returns an array of numbers
function getNumbers() {
  return [1, 2, 3, 4, 5];
}

// Destructing the array and assigning variables
let [a, b, c, d, e] = getNumbers();

console.log(a); // 1
console.log(b); // 2
console.log(c); // 3
console.log(d); // 4
console.log(e); // 5
```
> ***The forEach() Method***

In JavaScript, the forEach() method is used to iterate over the elements of an array. It allows you to execute a function for each element in the array. The basic syntax of the `forEach()` method is:

```js
array.forEach(function(currentValue, index, arr), thisValue)
````
  - currentValue is the current element being processed in the array.
  - index is the index of the current element being processed in the array.
  - arr is the array that forEach() is being applied to.
  - thisValue (Optional) is a value to use as this when executing the callback function

### Example:
```js
let fruits = ["apple", "banana", "mango"];
fruits.forEach(function(item, index, array) {
  console.log(item, index);
});

//This will log "apple 0", "banana 1", "mango 2" in the console.
```

You can also use arrow function like this:
```js
let fruits = ["apple", "banana", "mango"];
fruits.forEach((item, index) => console.log(item, index))

//This will also log "apple 0", "banana 1", "mango 2" in the console.
```
> ***The forEach() method in Set***

For Sets, the forEach method takes a callback function that is called for each value in the set. The callback function is passed two arguments: the value and the set itself. Here's an example:

```js
let mySet = new Set();
mySet.add("apple");
mySet.add("banana");

mySet.forEach((value, set) => {
  console.log(value);
});

// Output:
// apple
// banana
```
> ***The map() method***

The map() method in JavaScript is used to create a new array.
The map() function in JavaScript is a method that is used to transform the elements of an array. It takes a callback function as its first argument, which is called for each element in the array. The callback function takes three arguments: the current element, the index of the current element, and the array itself.

- ম্যাপ এ্যারের প্রত্যেকটি ইলিমেন্টকে পর্যায়ক্রমে আলাদাভাবে এ্যাকসেস করে।
- ম্যাপ প্যারামিটার হিসেবে একটি ফাংশন রিসিভ করে, ঐ ফাংশনের প্যারামিটার এ্যারের প্রত্যেকটি ইলিমেন্টকে পর্যায়ক্রমে আলাদাভাবে এ্যাকসেস করে। এই প্যারামিটার থেকে ভেল্যু এ্যাকসেস করে তার থেকে আউটপুট পাওয়ার জন্য রিটার্ণ করতে হয়।

```js
let students = [
            {
                Name: "Anamul",
                gpa: 3.5
            },
            {
                Name: "mamun",
                gpa: 3
            },
            {
                Name: "Anis",
                gpa: 2.5
            }
        ]

        /*Map with anonymous function*/
        const student = students.map(function (student) {
           console.log(student)
           return student.Name
        })
        document.write(student)

        /*Map with arrow function*/
        const student1 = students.map((student) =>student.Name)
        document.write(student1)
```
> ***The filter() Method***

The filter() method in JavaScript is a built-in function that allows you to filter an array based on a specified condition. It creates a new array with all elements that pass the test implemented by the provided function.
- ফিল্টার কন্ডিশনের উপর ভিত্তি করে এ্যারে থেকে ফিল্টার করে পুনরায় ঐ ফিল্টারের এ্যারে রিটার্ণ করে।
- এখানে এ্যারে থেকে প্রত্যেকটা student কে রিসিভ করে যাদের gpa তিন এর কম অথবা সমান তাদের এ্যারেকে রিটার্ণ করে। 
```js
//Syntax:
var newArray = oldArray.filter(function(element, index, array) {
  // Code to test the element
  // Return true if the element should be included in the new array
  // Return false if the element should be excluded from the new array
});
```
```js
//Example:

var numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
var evenNumbers = numbers.filter(function(number) {
  return number % 2 === 0;
});
console.log(evenNumbers); // Output: [2, 4, 6, 8, 10]
```
In this example, the filter() method is used to filter out all odd numbers from the numbers array. The function passed to filter() checks if each element in the array is divisible by 2 (meaning it's even) and returns true if it is and false if it's not. The filter() method then creates a new array (evenNumbers) with all elements that returned true and excludes the elements that returned false.

> ***The Filter() & Map() use together***

- যাদের  তিন এর নিচে তাদেরকে ফিল্টার করে Map করলে Map এর ফাংশেনের প্যারামিটারে সে এ্যারেটি চলে আসে। পরে ম্যাপিং এ সে  এ্যারে থেকে ছাত্রের নাম/ নামের এ্যারে এ্যাকসেস করা হয়।
```js
const student4 = students.filter((student) => student.gpa < 3)
        .map((student)=> student.Name)
        console.log(student4)
        console.log(student4[0])
```
> ***The reduce() Mehtod***

The reducer() method in JavaScript is a higher-order function that is used to reduce an array of values into a single value. 
- It takes two parameters: a callback function and an initial value. The callback function is called for each element in the array and is passed two arguments: the accumulated value (also known as the "accumulator") and the current value. 
- The initial value is the starting value for the accumulator.

The callback function should return the updated accumulator value after each iteration. The final value returned by the reducer() method is the final accumulator value after all iterations have completed.
### Syntax:
```js
array.reduce((acc, currentValue)=>{}, intialValue);
```

Here is an example of using the reducer() method to add up all the values in an array:
```js
let numbers = [1, 2, 3];
let sum = numbers.reduce(function(acc, currentValue) {
    return acc + currentValue;
}, 0);
console.log(sum); // 7
// acc means previous value
/*
with set initial value
preValue/acc  currentValue
0       +        1 = 1
1       +        2 = 3
3       +        3 = 7
7
*/

/*
without set initial value
preValue/acc  currentValue
1       +        2 = 3
3       +        3 = 6
6
*/
```
In this example, the callback function is adding the current value to the accumulator, and the initial value is 0. The final value returned by the reducer() method is 15, which is the sum of all the values in the array.

Here is an example of using the reducer() method to find the largest value in an array:
```js
let numbers = [5, 10, 15, 20, 25];
let largest = numbers.reduce(function(acc, currentValue) {
    if (currentValue > acc) {
        return currentValue;
    } else {
        return acc;
    }
}, 0);
console.log(largest); // 25
```
In this example, the callback function compares the current value to the accumulator. If the current value is larger, it becomes the new value for the accumulator. The initial value for the accumulator is 0. The final value returned by the reducer() method is 25, which is the largest value in the array.

Another example of using the reducer() method is creating a new object from an array of objects:
```js
let people = [
    { name: "John", age: 30 },
    { name: "Jane", age: 25 },
    { name: "Bob", age: 35 }
];
let ages = people.reduce(function(acc, currentValue) {
    acc[currentValue.name] = currentValue.age;
    return acc;
}, {});
console.log(ages); // { John: 30, Jane: 25, Bob: 35 }
```
In this example, the callback function creates a new property in the accumulator object for each person's name, and sets its value to the person's age. The initial value for the accumulator is an empty object. The final value returned by the reducer() method is an object containing the name and age of each person in the array.

As you can see, the reducer() method is a powerful tool that can be used to perform a variety of operations on arrays of values. It can be used to simplify complex code and make it more readable.

> ***chaining filetr(), map() and reduce() method***
```js
/*
1. create an array with number
2. From this array filter number wihich is greater then 20
3. Finding filtering data divide by 2
4. Finally add all numbers.
*/
let numbers = [10, 14, 20, 22, 24, 40, 35, 43, 46, 48];

let sum=numbers.filter((number) => number > 20).map((largeNumber) => largeNumber/2).reduce((acc,val)=>acc+val);
console.log(sum); //129
```
[Go to top:arrow_up: ](#topAdv)
</details>

<a name='object'></a>

<h1>JS Obect</h1>
<kbd>Learning Summary</kbd>

> ***Access Properties by Dot & Bracket Notation:***

In JavaScript, dot notation and bracket notation are both ways to access the properties of an object.

```js
let bio_data = {name:"Anamul", Age: 32, Home_town: "Narsingdi"};

//Access properties by dot notation
console.log(bio_data.name); //output - Anamul
console.log(bio_data.Age); //output - 32

// Access properties by Bracket notation (Must use "" in properties)
console.log(bio_data["name"]); //output - Anamul
console.log(bio_data["Age"]); //output - 32
```
> ***Value changing system***
```js
//1st System
let bio_data = {name:"Anamul", Age: 32, Home_town: "Narsingdi"};
bio_data["Home_town"] = "Dhaka" 
console.log(bio_data);
//result: { name: "Anamul", Age: 32, Home_town: "Dhaka" }

//2nd System
let bio_data = {name:"Anamul", Age: 32, Home_town: "Narsingdi"};
bio_data.Home_town = "Dhaka" 
console.log(bio_data);
//result: { name: "Anamul", Age: 32, Home_town: "Dhaka" }
```
> ***Delete Property***
```js
let bio_data = {name:"Anamul", Age: 32, Home_town: "Narsingdi"};
delete bio_data.Age;
console.log(bio_data);
//result:  { name: "Anamul", Home_town: "Narsingdi" }
```