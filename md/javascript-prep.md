# JavaScript 101

-
-

## Download a picture of a cute puppy
<img src="http://images4.fanpop.com/image/photos/14700000/So-cute-puppies-14749028-800-600.jpg" width=500px>

-

## Think like a computer

- Computers are obedient.
- They follow your instructions to a T.
- They cannot read your mind.
- You have to tell it in fine grain details exactly what you want.

-

## Find a picture of a cute puppy
1. Click on the `Chrome` image on the tool bar
2. Wait for `Chrome` to load
3. Click on the address bar
4. Delete all the text in the address bar
2. Type `cute puppy` in the address bar
3. Press `Enter`
4. Click `Images`
5. Click on the first image
6. Click 'View Image'
7. Right click on the image
8. Select `Save Image As...`
9. Click `Save`

-
-
## JavaScript

Created by Brendan Eich in May 1995 in 10 days.

It has evolved since then.

-
## Print out to the console

```javascript
console.log('I love ice cream!');
```

-

## Comments

```javascript
// short comments
console.log('Hello World!'); // inline short comments

/*
You can make long comments
with multiple lines here
*/
```

-
-
## Variables

Writing code without variable

```
// cube
console.log(4 * 4 * 4);

```
-
## Variables

Writing code WITH variable

```
// cube
let number = 4;
console.log(number * number * number);

```

-
## Variables
Just like 'x' in algebra, a variable is a named container for a value.

-

## Declaring Variables

Two ways to declare a variable:

the bad way
```javascript
let day;
day = 'Saturday';
```

the better way

```javascript
let day = 'Saturday';
```

-

## Using a variable

```
let day = 'Saturday';

console.log('Today is ' + day); // => Today is Saturday
console.log(day + ' is the best!'); // => Saturday is the best!
console.log('I love ' + day); // => // => I love Saturday
```

-

## Using a variable

```
let number = 2;
let cube = number * number * number;

```

-
-

## Data Types - Numbers

```
// integer
let integer = 13;

// decimal
let decimal = 3.14;
```

-

## Data Types - String
There are three ways to create a string.

```javascript
let user1 = 'Jane Lane'; // single quote
let user2 = "Jane Lane"; // double quote
let user3 = `Jane Lane`; // back tick
```

-

## Data Types - Boolean

Boolean has two values, either `true` or `false`.

```javascript
let catsAreTheBest = true;
let snakesAreTheBest = false;
```

-

## Data Types - null & undefined

``undefined`` means it has never been defined
```javascript
// it was never set to equal to anything
let favoriteThings;
```

``null`` is an empty value.
```javascript
// setting the fruit variable to an empty value
let fruit = null;
```
-
-

## Arithmetic Operators

```
let a = 7;
let b = 2;
```

<table>
    <thead>
      <tr>
        <th>Example</th>
        <th>Example Result</th>
        <th>Name</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>-a</code></td>
        <td>-7</td>
        <td> Negation</td>
        <td>Opposite of <code>a</code>.</td>
      </tr>
      <tr>
        <td><code>a + b</code></td>
        <td>9</td>
        <td>Addition</td>
        <td>Sum of <code>a</code> and <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a - b</code></td>
        <td>5</td>
        <td>Subtraction</td>
        <td>Difference of <code>a</code> and <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a * b</code></td>
        <td>14</td>
        <td>Multiplication</td>
        <td>Product of <code>a</code> and <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a / b</code></td>
        <td>3.5</td>
        <td>Division</td>
        <td>Quotient of <code>a</code> and <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a % b</code></td>
        <td>1</td>
        <td>Modulus</td>
        <td>Remainder of <code>a</code> divided by <code>b</code>.</td>
      </tr>
    </tbody>
 </table>

-

 ## The += operator

 We can easily add a number to itself using the ``+=`` operator
 ```javascript
 let sum = 0;
 sum = sum + 2;
 console.log(sum) // sum is equal to 2
 ```

 ```javascript
 let sum = 0;
 sum += 2;
 console.log(sum) // sum is equal to 2
 ```

-
-

## Strings

 Strings are a collection of characters.

 You can wrap a string in single, double quotes, or back tick.

 ```javascript
 let favoriteDonut = 'chocolate';
 let otherFavoriteDonut = "strawberry sprinkled";
 let donut = `Glazed`;
 ```

-
## Strings
Because JavaScript uses quotes to begin and end strings, if you want to use quotes in a string, you need to *escape* it.

 ```javascript
 let sentence = 'Domi\'s shop is the best!';
 ```
<br>
Or you can use a different quote.

```javascript
let sentence = "Domi's shop is the best!";
```

-

## Adding Strings

 We can *concatenate* strings using the ``+`` operator.

 ```javascript
 let firstName = "Ada";
 let lastName = "Lovelace";
 let fullName = firstName + " " + lastName;
 ```

-
## Adding Strings
 You can also use the ``+=`` operator

 ```javascript
 let fullName = "";
 fullName += "Ada"
 fullName += " ";
 fullName += "Lovelace"
 ```

-
## Combining Strings and Numbers

 When concatenating strings and numbers, numbers are automatically converted to strings.

 ```javascript
 let numberOfDonuts = 2;
 let typeOfDonuts = "chocolate";
 let stock = "We have " + numberOfDonuts
            + " " + typeOfDonuts + " " + "donuts.";
 ```

-
## String operations

`.length` returns the length of the string

```
'ice'.length
```

-
## String operations

`.includes` returns true if the string has that value, false otherwise

```
'ice'.includes('c'); // true
'ice'.includes('ic'); // true

'ice'.includes('a'); // false
```

-
## String operations

`.charAt` returns the character at that index.

Note index starts at 0. The last index is 11.
<img src="./img/apple.png">

```
let phrase = 'apple is red';
phrase.charAt(0); // a
phrase.charAt(9); // r
phrase.charAt(11); // d

//last character
phrase.charAt(phrase.length - 1); // d
```
-

## String operations

`.indexOf` returns the first index of that character.

<img src="./img/apple.png">

```
'apple is red'.indexOf('e'); // 4
```

-
## String operations

`.trim` returns the string with the space at the beginning and end removed

```
'  ice cream  '.trim(); // 'ice cream'
```

-
## String operations
- `length` - how many character are there
- `charAt` - the character at that index
- `includes` - checks if the string include this string
- `indexOf` - first index number of the character
- `toLowerCase` - converts all character to lower case
- `toUpperCase` - converts all character to upper case
- `trim` - remove spaces at the beginning and end

[Javascript API](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

-
-

## Arrays

Arrays are ordered lists of values.

```javascript
var numbers = [7, 3, 91, 3, 4];
```

-
## Arrays
You can put different types of data into an array.

```javascript
let colors = ['Red', 'Orange', 'Yellow', 'Green'];

let luckyNumbers = [52, 97, 91, 28, 43, 104];

let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];
```

-
## Arrays

`.length` returns the number of items in the array

```javascript
let colors = ['Red', 'Orange', 'Yellow', 'Green'];
colors.length; // 4;
```


```javascript
let luckyNumbers = [52, 97, 91, 28, 43, 104];
luckyNumbers.length; // 6
```

-

## Array - Get

Access an item in the array with the `[]` (ex: arrayName[index]).

Index is the position of the item. The position starts at `0`.

```javascript
let colors = ['Red', 'Orange', 'Yellow', 'Green'];

colors[0]; // 'Red'
colors[2]; // 'Yellow'
colors[colors.length - 1]; // 'Green'
```

-

## Array - Add

`.push` will add an item to the array

```javascript
let colors = ['Red', 'Orange', 'Yellow', 'Green'];
colors.push('Blue'); // ['Red', 'Orange', 'Yellow', 'Green', 'Blue']

```

-
## Array - Remove

`.pop` removes the last item from the array

```javascript
let colors = ['Red', 'Orange', 'Yellow', 'Green'];
colors.pop(); // ['Red', 'Orange', 'Yellow']

```

-
## Array - Update

`array.[index]` to update the value

```javascript

let colors = ['Red', 'Orange', 'Yellow'];
colors[1] = 'Blue'; // ['Red', 'Blue', 'Yellow']

```
-
## Array - Update

`array.[index]` to update the value

```javascript

let colors = ['Red', 'Orange', 'Yellow'];

let lastIndex = colors.length - 1;
colors[lastIndex] = 'Blue'; // ['Red', 'Orange', 'Blue']

```
-
-

## Functions

**Good developers are lazy developers.**

```javascript
let twoCube = 2 * 2 * 2;

let threeCube = 3 * 3 * 3;

let fourCube = 4 * 4 * 4;
```

-

## Do not repeat yourself

```javascript
cube(2);

function cube(number) {
          // 2    *   2    *    2
    return number * number * number;
}
```
-
## Do not repeat yourself

```javascript
cube(3);

function cube(number) {
          // 3    *   3    *    3
    return number * number * number;
}
```

-
## Do not repeat yourself

```javascript
function cube(number) {
    return number * number * number;
}

let twoCube = cube(2); // 8

let threeCube = cube(3); // 27

let fourCube = cube(4); // 64

```

-

## Anatomy of a function

```javascript

// function keyword - function name - parameters
function cube(number) {
    return number * number * number;
}
```

-

## Parameters

Parameters(/arguments) are named variables for values that will be passed in.

```javascript
// firstNum and secondNum act as aliases for values passed in later
function add(firstNum, secondNum) {
    console.log(firstNum + secondNum);
}

// invoke the function
add(2, 5) // firstNum is 2 and secondNum is 5
```

-

## Parameters

You can have any number of argument. Try to limit to 3.

```javascript
function noParam() {}

function oneParam(number){}

function threeParam(num1, num2, num3){}

noParam();
oneParam(1);
twoParam(3, 1, 20);

```

-

## The Return Keyword

Use the `return` keyword to get a result back from a function.

```javascript
function fullName(firstName, lastName) {
    return "My name is " + firstName + " " + lastName;
}

let name = fullName("Will", "Smith");
console.log(name); //My name is Will Smith
```
-

## The Return Keyword

`return` will exit the function

```javascript
function add(num1, num2) {
    // exits out of the function
    return true;

    // statement is never reached
    console.log("Hello!!!");
}
```

-
-

# Control Flow

-

## The If Statement

Use ``if`` statements to decide which lines of code to execute, based on a condition.

```javascript
if(condition) {
    // statements to excute
}
```

```javascript
let age = 30;

if (age > 18) {
  console.log('You are an adult');
}
```

JavaScript evaluates conditions to a ``boolean``, ``true`` or ``false``.

-

## Comparison Operators

<table>
    <thead>
      <tr>
        <th>Example</th>
        <th>Name</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>a == b</code></td>
        <td>Equal</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is equal to <code>b</code> (can be different types).</td>
      </tr>
      <tr>
        <td><code>a === b</code></td>
        <td>Identical</td>
        <td>
      <strong><code>TRUE</code></strong> if <code>a</code> is equal to <code>b</code>, and the same type. </td>
      </tr>
      <tr>
        <td><code>a != b</code></td>
        <td>Not equal</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is not equal to <code>b</code> (can be different types).</td>
      </tr>
      <tr>
        <td><code>a !== b</code></td>
        <td>Not identical</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is not equal to <code>b</code>, or they are not the same type.</td>
      </tr>
    </tbody>
  </table>

-

## Comparison Operators

<table class="smalltext">
    <thead>
      <tr>
        <th>Example</th>
        <th>Name</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>a &lt; b</code></td>
        <td>Less than</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is strictly less than <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a &gt; b</code></td>
        <td>Greater than</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is strictly greater than <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a &lt;= b</code></td>
        <td>Less than or equal to </td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is less than or equal to <code>b</code>.</td>
      </tr>
      <tr>
        <td><code>a &gt;= b</code></td>
        <td>Greater than or equal to </td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is greater than or equal to <code>b</code>.</td>
      </tr>
    </tbody>
  </table>

-

## Logical operators

<table>
    <thead>
      <tr>
        <th>Example</th>
        <th>Name</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><code>a &amp;&amp; b</code></td>
        <td>And</td>
        <td><strong><code>TRUE</code></strong> if both <code>a</code> and <code>b</code> are <strong><code>TRUE</code></strong>.</td>
      </tr>
      <tr>
        <td><code>a || b</code></td>
        <td>Or</td>
        <td><strong><code>TRUE</code></strong> if either <code>a</code> or <code>b</code> is <strong><code>TRUE</code></strong>.</td>
      </tr>
      <tr>
        <td><code>!a</code></td>
        <td>Not</td>
        <td><strong><code>TRUE</code></strong> if <code>a</code> is not <strong><code>TRUE</code></strong>.</td>
      </tr>
    </tbody>
  </table>

-

## Truthy and Falsy

```javascript
function logTruthiness(val) {
    if(val) {
        console.log("Truthy!");
    } else {
        console.log("Falsy.");
    }
}
```
-

## Truthy and Falsy

```javascript
// Outputs: "Truthy!"
logTruthiness(true);

// Outputs: "Truthy!"
logTruthiness({});

// Outputs: "Truthy!"
logTruthiness([]);

// Outputs: "Truthy!"
logTruthiness("some string");

// Outputs: "Truthy!"
logTruthiness(3.14);
```

-

## Truthy and Falsy

```javascript
// Outputs: "Falsy."
logTruthiness(false);

// Outputs: "Falsy."
logTruthiness(null);

// Outputs: "Falsy."
logTruthiness(undefined);

// Outputs: "Falsy."
logTruthiness(NaN);

// Outputs: "Falsy."
logTruthiness(0);

// Outputs: "Falsy."
logTruthiness("");
```

-

## The if else statement

If you have multiple conditions, you can use ``else if``.

```javascript
let age = 30;

if (age >= 35) {
  console.log('You can vote AND run for President!'); // win not run
} else if (age >= 30) {
  console.log('You can vote AND run for the Senate!'); // will run
} else if (age >= 18) {
  console.log('You can vote!'); // will not run
} else {
  console.log('You can\'t vote, but you can write your representatives.'); // will run
}
```

Only one condition will be met.

-

## Combining Individual If Statements

```javascript
let age = 30;

// individual if statement
if (age >= 35) {
  console.log('You can vote AND run for President!'); // will not run
}

if (age >= 30) {
  console.log('You can vote AND run for the Senate!'); // win run
}

if (age >= 18) {
  console.log('You can vote!'); // will run
} else {
  console.log('You can\'t vote, but you can write your representatives.'); // will not run
}
```
-

## Combining Conditionals

You can use logical operators to combine conditions

```javascript
let age = 30;
let yearsAsCitizen = 30;

// If you are over 30 and you've been a citizen for over 9 years
if (age >=30 && yearsAsCitizen > 9) {
  console.log('You can run for the Senate!');
} else {
  console.log('You are not eligible to run for the Senate');
}
```

```javascript
let birthYear = 1992;

// If you were born before 1980 or born after 2000
if(birthYear < 1980 || birthYear > 2000) {
    console.log('You are not a millennial');
}
```

-
-

## Scope

Variables defined in the global scope are declared outside of a set of curly braces {}, referred to as a block,
and are available throughout a program.

```javascript
let fullName = "Dominique Clarke";

function greet() {
    return "Hello " + fullName;
}

function farewell() {
    return "Bye " + fullName;
}
```
-

Variables defined in the global scope are open to mutation.

```javascript
let state = "Delaware";

let capitol = "Dover";

function printStateCapitol() {
    capitol = "Newark";
    console.log("The capitol of " + state " is " + capitol);
}

printStateCapitol();

console.log(capitol); // prints dover
```
This can create unintended consequences.

-

*But Dominique, I wouldn't do something silly like that.*

* You'll be working with a team of people, who won't understand your code as well as you do.
* You'll write tens of thousands of lines of code over your career, and forget a lot what your old code is doing.

-

We can prevent against values being changed using ``const``.

```javascript
const state = "Delaware";

const capitol = "Dover";

function printStateCapitol() {
    capitol = "Newark"; // Throws an error, which will stop your program
    console.log("The capitol of " + state " is " + capitol);
}
```
-

Instead of relying on global variables, we can write our functions to rely on parameters we give it.

```javascript
let state = "Delaware";

let capitol = "Dover";

function printStateCapitol(state, capitol) {
    capitol = "Newark";
    console.log("The capitol of " + state + " is " + capitol);
}

console.log(capitol); // prints Dover
```

-

Parameters are a special kind of variable that are assigned to the value passed in it, and scoped only to the function.

```javascript
let state = "Delaware";

let capitol = "Dover";

function printStateCapitol(state, capitol) {
    capitol = "Newark";
    // Prints "The capitol of Delaware is Newark"
    console.log("The capitol of " + state + " is " + capitol);
}

console.log(capitol); // prints Dover
```
-

When JavaScript encounters a variable, it looks to see if that variable is available in it's code block.

If it's not, it moves up the line of scope until it finds it.

```javascript
let state = "Delaware";

let capitol = "Dover";

function printStateCapitol(state, capitol) {
    capitol = "Newark";
    // Prints "The capitol of Delaware is Newark"
    console.log("The capitol of " + state + " is " + capitol);
}

console.log(capitol); // prints Dover
```
-

Variables can also be *locally scoped*. A new scope is created for each block of code between a set of curly braces.

Local variables are available within their code block, and any nested code blocks.


```javascript
// global scope (scope 1)
let radius = 2;

function calcAreaOfCircle(radius) {
    // local scope (scope 2)
    has access to scope 1 and scope 2 */
    const pi = 3.14;

    function calcDiameter() {
       /* local scope (scope 3)
       has access to scope 1, scope 2, and scope 3 */
       let diameter;

       /* has access to the radius variable,
       even though it wasn't passed into the function
       as a parameter */
       diameter = radius * 2;
       return diameter;
    }

    // Uncaught ReferenceError: diameter is not defined
    return pi * diameter;
}

calcAreaOfCircle(radius);

// Uncaught ReferenceError: pi is not defined
console.log(pi);

```
-

Other types of code blocks, like ``loops`` and ``if statements`` also create local scope.

```javascript
/* Global scope (scope 1)
Has access to scope 1 */
let n = 100;

function countByTenToN() {
    /* Local scope (scope 2)
    Has access to scope 1 and scope 2 */
    let currentNum = 0;

    while (currentNum <= 100) {
        /* Local scope (scope 3)
        Has access to scope 1, scope 2 and scope 3 */
        let iterator = 10;
        console.log(10
        currentNum += 10;
    }

    // Uncaught ReferenceError: iterator is not defined
    console.log(iterator);

}
```
-

The ``let`` and ``const`` keywords create brand new variables, and can share names with other variables
as long as they are located within a different level of scope.

```javascript
// Global scope (scope 1)
let radius = 2;
const pi = 3.14

function calcAreaOfCircle(radius) {
    // Local scope (scope 2)
    const pi = 3.141; // creates a new variable pi scoped within the curly braces.

    return pi * radius * radius;
}

// Global scope (scope 1)
const pi = 3.1415; // duplicate declaration of pi exists within this scope, creates an error

```

-

## The wilder days of JavaScript

The ``let`` and ``const`` keywords are new features of JavaScript available in the most recent specs.

Before ``let`` and ``const``, we'd declare variables with ``var``, which didn't follow the same scoping rules.

-

With ``var``, only functions create brand new levels of scope.

```javascript
// Global scope (scope 1)
var n = 100;

function countByTenToN() {
    // Local scope (scope 2)
    Has access to scope 1 and scope 2 */
    var currentNum = 0;

    while (i <= 100) {
        Has access to scope 1, scope 2 and scope 3 */
        var iterator = 10;
        console.log(10
        currentNum += 10;
    }

    // available from outside it's block
    console.log(iterator);
}
```

-
-

## Loops

-

## The For Loop

A for loop repeats until a specified condition evaluates to false.

```javascript
function printToN(n) {
    // define iterator; define condition; define increment
    // runs until i > n;
    for(let i = 1; i <= n; i++) {
        console.log(i);
    }
}
```

-

We can change the iterator, the condition, and the increment to suit our needs.

```javascript
function printFromN(n) {
    // define iterator; define condition; define increment
    // runs until i < n;
    for(let i = n; i >= n; i--) {
        console.log(i);
    }
}
```

``i++`` is shorthand for ``i = i + 1``;

``i--`` is shorthand for ``i = i - 1``;

-

We can increment by more than 1.

```javascript
function printEvenNumbers(n) {
    for(let i = 0; i <= n; i+=2) {
        console.log(i);
    }
}
```

-

## The while loop

The ``while`` statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

```javascript
var n = 0;
var x = 0;

while (n < 3) {
  n++;
  x += n;
}
```

* After the first pass: n = 1 and x = 1
* After the second pass: n = 2 and x = 3
* After the third pass: n = 3 and x = 6


-
-

## Objects

Objects help us represent real-world objects in JavaScript. Using ``key: value`` pairs (sometimes also referred to as properties) we can mock out an object's
``identity``, ``state``, and ``behavior``.


-


JavaScript objects are containers that can store data and functions. The data we store in an object is not ordered — we can only access it by calling its associated key.

```javascript
let object = {
    key: value,
    property: propertyValue,
}
```

* We create the object between curly braces: {}.
* We separate each key from its corresponding value by a colon ``:``, with the key first and the value second.
* Every key-value pair is separated by a comma ``,``.

-

```javascript
let car = {
    make: 'Ford',
    model: 'Taurus',
    totalMillage: 30000,
    drive: function() {
        // TO DO: Make car move
    }
}
```

-

## Object Review

-

## Accessing Object Properties

You can use dot notation to access object properties

```javascript
console.log(user.username) // outputs donutLover5000
```

Or you can use bracket notation and pass in a string representing the property
```javascript
console.log(user['username']) // outputs donutLover5000
```
-

## Changing Objects

You can use dot or bracket notation to change property values

```javascript
user.username = "imAHotDog";
user['username'] = "imAHotDog";
```
-

## Adding Properties to Objects

You can use dot or bracket notation to add properties and their value.

```javascript
let car = {
    make: 'Ford',
    model: 'Taurus',
    totalMillage: 30000,
}

car.color = 'red';
car['milesPerGallon'] = 30;
```

Since neither the property ``color`` or ``milesPerGallon`` exist on the car object, they are created when we try to assign them values.

-

## Bracket vs Dot Notation

Bracket notation can be helpful when you want to use a variable as a key.

```javascript
let currentDayOfWeek = 'Friday';

const dailySpecials = {
    Monday: 'Half-off Drinks',
    Wednesday: 'Half-off Burgers',
    Friday: 'Prime Rib',
}

if(dailySpecials[currentDayOfWeek]) {
    console.log(dailySepcials[currentDayOfWeek]);
}
```

-

## Creating Methods

When an object stores a function as the value of a property, we call that function a ``method``.

Objects can have ``idenity``, ``state``, and ``behavior``. Methods represent the behavior for our objects.

```javascript
let dog = {
    speak: function() {
        return 'bork';
    }  
}
```

-

```javascript
// ES6
let dog = {
    speak: () => {
        return 'bork';
    }  
}
```

```javascript
// ES6
let dog = {
    speak() {
        return 'bork';
    }  
}
```

-

## The This Keyword

Often, we want our methods to interact with properties that exist on the object itself.

```javascript
// ES6
let dog = {
    isSitting: false,
    speak() {
        return 'bork';
    },
    sit() {
        // ReferenceError: isSitting is not defined
        if(isSitting) {
          return "already sitting";
        } else {
          // looks for the isSitting variable up the line of scope,
          // if it doesn't find it creates a global variable on the window object
          isSitting = true;
          return "yes hooman i'll do a sit";
        }
    }
}
```
-

```javascript
// ES6
let dog = {
    isSitting: false,
    speak() {
        return 'bork';
    },
    sit() {
        // ReferenceError: isSitting is not defined
        if(isSitting) {
          return "already sitting";
        } else {
          // looks for the isSitting variable up the line of scope,
          // if it doesn't find it creates a global variable on the window object
          isSitting = true;
          return "yes hooman i'll do a sit";
        }
    }
}
```

Referencing the property name alone has unintended behavior and causes errors. The property name alone does not grab us the property value.

-

## The This Keyword

To grab the value of a property off the current object, use the ``this`` keyword.

```javascript
let dog = {
    isSitting: false,
    speak() {
        return 'bork';
    },
    sit() {
        if(this.isSitting) {
          return "already sitting";
        } else {
          this.isSitting = true;
          return "yes human i'll do a sit";
        }
    }
}
```

In Javascript, ``this`` refers to the object we call it inside.

-
-

## Iterators

-

Loops and arrays are best friends. We can use a loop to visit each element in the array

```javascript
let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];

for(let i = 0; i < myFavoriteThings.length; i++) {
    // do something with the current element in the array
    console.log(myFavoriteThings[i]);
}
```

-

There are quite a few scenarios in which we may need to visit each element in an array.

Arrays have a few built in ``methods`` that we can use to to accomplish common array tasks.

-

## Array iterator syntax

```javascript
arr.method(callback(currentElement, index, currentArray) {
    //your iterator
})
```

* ```arr``` - The array you are operating on

* ``method`` - The method you want to execute. Examples include ``forEach``, ``filter``, ``map`` and more.

* ``callback`` - Function to execute for each element. The callback functions for iterator methods typical accepts three arguments, ``currentElement``, ``index``, and ``currentArray``.

-

```javascript
arr.method(callback(currentElement, index, currentArray) {
    //your iterator
})
```

* ``currentElement`` - Mandatory parameter. The value of the current element being processed in the array.

* ``index`` - Optional parameter. The index of the current element being processed in the array.

* ``currentArray`` - Optional parameter. The array that forEach() is being applied to. I.E. ``arr``.

-

## Callback Functions

A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

```javascript
function greeting(name) {
  alert('Hello ' + name);
}

function processUserInput(callback) {
  var name = prompt('Please enter your name.');
  callback(name);
}

processUserInput(greeting);
```

Array iterators take our callback functions and use them in a meaningful way.

-

``.forEach()`` is used to execute the same code for every element in an array.

```javascript
let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];

myFavoriteThings.forEach(element => {
    console.log(element);
})
```

```javascript
let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];

for(let i = 0; i < myFavoriteThings.length; i++) {
    // do something with the current element in the array
    console.log(myFavoriteThings[i]);
}
```

-

``.map()`` creates a new array with the results of calling a provided callback function on every element in old array.

```javascript
let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];

let copy = myFavoriteThings.map(element => {
    return element;
})
```

```javascript
let myFavoriteThings = ['Donuts', 42, true, 'Pizza'];
let copy = []

for(let i = 0; i < myFavoriteThings.length; i++) {
    copy.push(myFavoriteThings[i]);
}
```
-

``.filter()`` checks every element in an array against a conditional to see if it meets a certain criteria,
then returns a new array with each element that meet that condition.

```javascript
let users = [{name: 'Dominique', age: 26}, {name: 'Sonja', age: 13}, {name: 'Nyla', age: 18}];
let adultUsers = [];

for(let i = 0; i < myFavoriteThings.length; i++) {
  if(users[i].age >= 18) {
    adultUsers.push(users[i]);
  }
}
```

```javascript
let users = [{name: 'Dominique', age: 26}, {name: 'Sonja', age: 13}, {name: 'Nyla', age: 18}];

let adultUsers = users.filter(user => {
    return user.age >= 18;
})
```
-

Iterators help us create clean, semantic code.

You can find more iterators and other array methods on <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array">MDN</a>

-
-

## Classes

-

## Object Review

JavaScript is an object-oriented programming (OOP) language we can use to model real-world items and their ``idenity``, ``state``, and ``behavior``.

We model these items using ``JavaScript objects`` that contain ``properties`` that represent an item's identity, state, and behavior.

Groups of similar, real world items share properties. The values of these properties can be consistent, or vary.

-

## Object Review

```javascript
let corgi = {
    breed: 'corgi',
    name: 'snuffles',
    speak() {
        return 'bork';
    }
}

let corgi2 = {
    breed: 'corgi',
    name: 'cuddles',
    speak() {
        return 'bork';
    }
}

let yorki = {
    breed: 'yorki',
    name: 'gadget',
    speak() {
        return 'bork';
    }
}

let yorki2 = {
    breed: 'yorki',
    name: 'wrinkle',
    speak() {
        return 'bork';
    }
}
```
We can avoid repeated code and create similar objects using ``classes``.

-

## Classes

Classes are the **blueprints** for objects. Rather than us creating objects directly, we can use classes as blueprints for creating objects.

```javascript
class Dog {
    constructor(breed, name) {
        this.breed = breed;
        this.name = name;
    }

    speak() {
        return 'bork';
    }
}

let corgi = new Dog('corgi', 'snuffles');
let corgi2 = new Dog('corgi', 'cuddles');
let yorki = new Dog('yorki', 'gadget');
let yorki2 = new Dog('yorki', 'wrinkle');
```

-

## Declaring Classes

We use the ``class`` keyword before the class name to declare a class.

We wrap the instructions for the class within a set of curly braces ``class Dog { }``, similar to objects.

```javascript
class Dog {
    constructor(breed, name) {
        this.breed = breed;
        this.name = name;
    }

    speak() {
        return 'bork';
    }
}
```

**Naming conventions**: Classes are capitalized to distinguish them from variables.

-

## Using Classes To Create Objects

We use classes to create objects, or ``instances`` of a class.

We create these unique instances using the ``new`` keyword which generates for us a new object using that class.

```javascript
let corgi = new Dog('corgi', 'snuffles');
let corgi2 = new Dog('corgi', 'cuddles');
let yorki = new Dog('yorki', 'gadget');
let yorki2 = new Dog('yorki', 'wrinkle');
```

Notice that using classes looks a lot like calling a function.
That's because when we invoke, or call, the class using its name and passing in parameters, it calls a special ``function`` called a ``constructor``.

-

## Constructors

Classes contain a special ``method`` called a ``constructor``.

Constructors are called every time we use the ``new`` keyword to create a new instance.

```javascript
class Dog {
    constructor(breed, name) {
        this.breed = breed;
        this.name = name;
    }

    speak() {
        return 'bork';
    }
}
```

-

## Constructors

Constructors declare the properties for our objects and set them with an initial value, with the exception of methods.

```javascript
class Student {
    constructor(name, email) {
        this.name = name;
        this.email = email;
        this.grades = [];
    }

    // TO DO: Write Methods
}
```

Remember the ``this`` keyword refers to the current object. When we use dot notation with the ``this`` keyword, we declare
new properties on our objects. Each object created with the ``Student`` class will now have a name, email, and grades property.

-

## Constructors

Students share properties, but the values of those properties can be vary. We can assign initial values for our properties through
the parameters we accept in the constructor.

```javascript
class Student {
    constructor(name, email) {
        /* assigns the name and email properties
        to the specific name and email we pass in*/
        this.name = name;
        this.email = email;

        // default initial value for grades
        this.grades = [];
    }

    // TO DO: Write Methods
}
```

We can also assign values to properties that share a default value across all objects.

-

## Methods

The ``behavior`` of our objects is defined through methods.

```javascript
// Creating a dog through a class
class Dog {
    constructor(breed, name) {
        this.breed = breed;
        this.name = name;
        this.hasBall = false;
    }

    // We can list methods underneath our constructor    
    speak() {
        return 'bork';
    }

    fetch() {
        this.hasBall = true;
    }
}

let dog = new Dog('corgi', 'snuggles');

// Creating a dog object directly
let dog2 = {
    breed: 'corgi',
    name: 'snuggles',
    speak() {
        return 'bork';
    },
    fetch() {
        this.hasBall = true;
    }
}
```

-

## Getters and Setters

A common object design pattern is to include getter and setter methods as attributes.

Getter and setter are special ``methods`` that get and set the properties inside of an object. Using getters and setters we can:

* You can check if new data is valid before setting a property.
* You can perform an action on the data while you are getting or setting a property.
* You can control which properties can be set and retrieved.

-

## Getters and Setters

When using getters and setters, we prepended the property names with underscores (_).
Javascript developers *sometimes* use an underscore before a property name to indicate a property or value should not be modified directly by other code.

```javascript
class Student {
    constructor(name, email) {
        /* these properties should only be
        accessed through getters and setters*/
        this._name = name;
        this._email = email;
        this._grades = [];
    }

    // TO DO: Write Getters and Setters
}
```

-

## Setters

Setters are great for validating input before mutating a value.
We create a setter by using the ``set`` keyword before the method declaration.  

```javascript
class Student {
    constructor(name, email) {
        /* these properties should only be
        accessed through getters and setters*/
        this._name = name;
        this._email = email;
        this._grades = [];
    }

    set email(newEmail) {
        if(typeof newEmail === 'string') {
            this._email = newEmail;
        }
    }
    // TO DO: Write Getter
}
```

-

## Setters

We name our setters the name of the property we are trying to mutate, minus the ``_``. Setters except **exactly one** parameter, representing the value we are trying to set the property to.

```javascript
class Student {
    constructor(name, email) {
        /* these properties should only be
        accessed through getters and setters*/
        this._name = name;
        this._email = email;
        this._grades = [];
    }

    set email(newEmail) {
        if(typeof newEmail === 'string') {
            this._email = newEmail;
        }
    }
    // TO DO: Write Getter
}
```

-

## Setters

When we create a setter, a **property** of the same name is automatically created on the object.
The setter method is called when we try to change the value of that property using ``=``, passing in the value on the right side of the ``=`` sign.

```javascript
let student = new Student('Domi', 'doclarke71@gmail.com');
student.email = 'dominique@zipcodewilmington.com';
student.email = 42;

console.log(student._email); // will read 'dominique@zipcodewilmington.com'
```

Because we don't yet have a ``getter``, we need to access the property we just mutated through ``_email``, which we shouldn't do. Let's fix that.

-

## Getters

We create a getter by using the ``get`` keyword before the method declaration.  

```javascript
class Student {
    constructor(name, email) {
        /* these properties should only be
        accessed through getters and setters*/
        this._name = name;
        this._email = email;
        this._grades = [];
    }

    get email() {
        return this._email;
    }

    set email(newEmail) {
        if(typeof newEmail === 'string') {
            this._email = newEmail;
        }
    }
}
```

-

## Getters

Getters take 0 parameters, and simply return the value of the associated property.
We name our getters the name of the value we're trying to return, minus the ``_``.

```javascript
class Student {
    constructor(name, email) {
        /* these properties should only be
        accessed through getters and setters*/
        this._name = name;
        this._email = email;
        this._grades = [];
    }

    get email() {
       return this._email;
    }

    set email(newEmail) {
        if(typeof newEmail === 'string') {
            this._email = newEmail;
        }
    }
}
```

-

## Getter

When we create a getter, a **property** of the same name is automatically created on the object.
The getter method is called when we try to access that property.

```javascript
let student = new Student('Domi', 'doclarke71@gmail.com');
student.email = 'dominique@zipcodewilmington.com';
student.email = 42;

/* now we can use our getter, email.
Since we aren't trying to assign it a new value,
the getter method is called instead of the setter
method
*/
console.log(student.email); // will read 'dominique@zipcodewilmington.com'
```
-

## Inheritance

Classes can borrow and extend functionality of other classes through ``inheritance``.

When multiple classes share properties or methods, they become candidates for inheritance.

With inheritance, you can create a parent class (also known as a superclass) with properties and methods that multiple child classes (also known as subclasses) share. The child classes inherit the properties and methods from their parent class.

-

## Inheritance

Let's say we want to recreate the Doggo chart.
Doggos share many properties, but specific doggos have different values for those properties, and sometimes even have extra properties and methods.

```javascript
class Doggo {
    constructor(name, breed, size) {
        this._name = name;
        this._breed = breed;
        this._size = size;
    }

    // Getters and Setters
}

class Pupper extends Doggo {
    constructor(name, breed) {
        this._name = name;
        this._breed = breed;
        this._size = 'smol';
    }
}
```
-

## Superclasses

Since ``Pupper`` extends ``Doggo``, ``Doggo`` is the super class of ``Pupper``.

``Pupper`` therefore inherits the properties and methods from ``Doggo``.

Puppers share the same properties as doggos, but their size is always smol.
When creating a pupper, we should be able to set its name and breed, but not its size.

-

## Calling the superclass constructor

In the previous example, we set the ``_name``, ``_breed``, and ``_size`` properties of ``Pupper`` manually, even though it extends from ``Doggo``.

-

## Calling the superclass constructor

Doggo already has a constructor that sets these properties, and we can call it using the ``super`` method. The super method calls the superclass's constructor.

```javascript
class Doggo {
    constructor(name, breed, size) {
        this._name = name;
        this._breed = breed;
        this._size = size;
    }

    // Getters and Setters
}

class Pupper extends Doggo {
    constructor(name, breed) {
       super(name, breed, 'smol');
    }
}
```

-

## Calling the superclass constructor

```javascript
class Doggo {
    constructor(name, breed, size) {
        this._name = name;
        this._breed = breed;
        this._size = size;
    }

    // Getters and Setters
}

class Pupper extends Doggo {
    constructor(name, breed) {
       super(name, breed, 'smol');
    }
}

class Woofer extends Doggo {
    constructor(name, breed) {
        super(name, breed, 'big ol');
    }
}
```
-

## Calling the superclass constructor

We can create chains of inheritance. Sub classes can also add properties or methods not available on its superclass.

```javascript
class Doggo {
    constructor(name, breed, size) {
        this._name = name;
        this._breed = breed;
        this._size = size;
    }

    // Getters and Setters
}

class Woofer extends Doggo {
    constructor(name, breed) {
        super(name, breed, 'big ol');
    }
}

class Grizlord extends Woofer {
    constructor(name, breed) {
        super(name, breed);
        this._eatsAHumans = true;
    }

    eatHuman(human) {
        human.isDead = true;
    }
}
```

-

## Static methods

Static methods are methods that **do not** operate on instance properties.
Because they do not operate on instance properties, we do not need to create a new object to use these methods.
We can use these methods directly on the class.

```javascript
// Notice how we did not create a new Date object. We simply used the date class
let date = Date.now();
```

-

## Static methods

Every time you call a static method, you should expect the same output when providing the same input.

```javascript
class Calculator {
    constructor() {
        this.memory = 0;
    }

    static add(x, y) {
        return x + y;
    }

    saveToMemory(x) {
        this.memory = x;
    }
}

let sum = Calculator.add(2, 2);

// in order to use memory, we need to create an instance of a calculator
let calc = new Calculator();

let sum2 = calc.add(2, 2);
calc.addToMemory(sum2);
```
