# JavaScript 101

-
-

## Download a picture of a cute puppy
<img src="https://images.phillypublishing.com/onwardstate/uploads/2013/04/puppy3.jpg" width=500px>

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

## Comments

Is this valid?

```javascript

// You can make long comments
// with multiple lines here

```

<p class="fragment">Yes</p>

-

## Comments

Is this valid?

```javascript
console.log('Hello World!'); /* inline comments */

```

<p class="fragment">Yes</p>

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

Writing code without variable

```
// cube
console.log(10 * 10 * 10);

```

When we edit a value, we have to change it in three places.

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

Writing code WITH variable

```
// cube
let number = 10;
console.log(number * number * number);

```

When we edit a value, we only need to change it in ONE place.
-
## Variables
Just like 'x' in algebra, a variable is a named container for a value.

-

## Variables

#### Why do we use variable in programming?

<p class="fragment">to make it easier to change the value</p>

-

## Declaring Variables

Two ways to declare a variable:


```javascript
// declare a variable in two statements
let day;
day = 'Saturday';
```

the better way

```javascript
// declare it in one statement
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

```javascript
let day = 'Sunday';

console.log('Today is ' + day); // => Today is Sunday
console.log(day + ' is the best!'); // => Sunday is the best!
console.log('I love ' + day); // => // => I love Sunday
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

## The % operator

Returns the remainder of `a` divided by `b`

```
3 % 2 // returns 1 because the remainder of 3/2 is 1
```
<p class="fragment">What is `11 % 3`?</p>
<p class="fragment">2</p>
<p class="fragment">How do I check if the number is even?</p>

-

## The % operator

```javascript
// is number even?
3 % 2 == 0 // false because the remainder is 1
4 % 2 == 0 // true because the remainder is 0
```

<p class="fragment">How do I check if the number is odd?</p>

-

## The % operator

```javascript
// is number odd?
3 % 2 == 1 // true because the remainder is 1
4 % 2 == 1 // false because the remainder is 0
```

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
Because JavaScript uses quotes to begin and end strings, if you want to use quotes in a string, you need to *escape* it with `\`.

 ```javascript
 let sentence = 'Domi\'s shop is the best!';
 ```
<br>
Or you can use a different quote.

```javascript
let sentence = "Domi's shop is the best!";
```

Here I know I need a `'`, so I wrap it in `"`.

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
 let type = "donuts";


let stock = numberOfDonuts + " " + type; //2 donuts

 ```

-
## String operations

`.length` returns the how many character is in the string

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

`array[index]` to update the value

```javascript

let colors = ['Red', 'Orange', 'Yellow'];
colors[1] = 'Blue'; // ['Red', 'Blue', 'Yellow']

```
-
## Array - Update

`array[array.length - 1]` to update the last value


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

<p class="fragment">Is there a pattern here?</p>
<p class="fragment">Yes, you need to multiply the number 3 times.</p>
-

## Do not repeat yourself

create a function to do the thing that repeats

```javascript
cube(2);

function cube(number) {
          // 2    *   2    *    2
    return number * number * number;
}
```
-
## Do not repeat yourself

now you can use it for any number

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
// firstNum and secondNum act as aliases
// for values passed in later
function add(firstNum, secondNum) {
    console.log(firstNum + secondNum);
}

// invoke the function
add(2, 5) // firstNum is 2 and secondNum is 5
add(7, 10) // firstNum is 7 and secondNum is 10
```

-

## Parameters

You can have any number of argument. Try to limit it to 3.

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

let name1 = fullName("Jada", "Smith");
console.log(name1); //My name is Will Smith
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
## Task

- write a function to convert Fahrenheit to Celsius
- the formula is (°F - 32)/1.8
- convert(32) => 0°C
- convert(76) == 24.44444°C

-
-

# Control Flow

-

## The If Statement

Use ``if`` statements to decide which lines of code to execute, based on a condition.

```javascript
if(condition that evaluate to true or false) {
    // statements to excute
}
```

-
## The If Statement

Use ``if`` statements to decide which lines of code to execute, based on a condition.

```javascript
let age = 30;

// only log this message if the age is larger than 18
if (age > 18) {
  console.log('You are an adult');
}
```

-

## Comparison Operators

<table>
    <thead>
      <tr>
        <th>Example&nbsp;&nbsp;&nbsp;</th>
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
## The if and else statement

Use `else` for the other condition

```javascript
function message(pet) {
  if (pet == "dog") {
    //only execute this if pet is dog
    console.log("You love dogs!");
  } else {
    // default statement
    console.log("Don't you like pets?")
  }
}
```

Only one condition will be met.

-

## The if else statement

Use `else if` for multiple conditions.

```javascript
function message(pet) {
  if (pet == "dog") {
    //only execute this if pet is dog
    console.log("You love dogs!");
  } else if (pet == "cat") {
    //only execute this if pet is cat
    console.log("You love cats!");
  } else {
    // default statement
    console.log("Don't you like pets?")
  }
}
```

Only one condition will be met.

-
## Combining Conditionals

You can use logical operators to combine conditions

```javascript
function message(pet) {
  if (pet == "dog" || pet == "cat") {
    // print message if pet is dog or cat
    console.log("You love pets!");
  } else {
    console.log("Don't you like pets?");
  }
}
```

-
-

## Loops

-
## Loops

```javascript
let colors = ['red', 'green', 'blue', 'orange'];

console.log(colors[0]);
console.log(colors[1]);
console.log(colors[2]);
console.log(colors[3]);

```
Notice we are repeating ourselves.

What is the pattern?

<p class="fragment">the index increase by 1</p>

-

## Loops

```javascript
let colors = ['red', 'green', 'blue', 'orange'];


for(let i = 0; i < colors.length; i = i + 1) {
  console.log(colors[i]);
}

```

- `let i = 0;` means the first number is 0
- `i < colors.length` - do this loop as long as `i` is less than the length
- after every iteration, increate i by 1

-

## Loops

Another way to increment `i`

```javascript
let colors = ['red', 'green', 'blue', 'orange'];

// i++ is the same is i = i + 1
for(let i = 0; i < colors.length; i++) {
  console.log(colors[i]);
}

```
