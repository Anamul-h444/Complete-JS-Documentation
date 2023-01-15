# Complete JS Documentation
<a name='top'></a>
<button style='padding:5px; font-size:14px;'>JS Fundamental Contents</button>

***Please click to go to topic>>>>>***

1. [Statement and Comments](#Statement)
1. [Details about variable](#variable)
1. [Concatenation](#Concatenation)
1. [Data types](#dataTypes)
1. [Operators](#operator)
1. [Conditional Statement](#statement)
1. [function](#function)
1. [Loop in JS](#loop)

<a name='topf'></a>
<button style='padding:5px; font-size:14px;'>JS Advanced Level Contents</button>

***Please click to go to topic>>>>>***

<button style='padding:5px; font-size:14px;'>JS Fundamental Topics Details</button>

***Please click for open details topic>>>>>***
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


<a name='dataType'></a>

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

<a name='function'></a>

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


<button style='padding:5px; font-size:14px;'>JS Advanced Lavel Topics Details</button>

***Please click for open details topic>>>>>***