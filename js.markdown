---
layout: page
title: "Javascript Tutorial"
permalink: /js/
comments: false
linked: true
---

<!-- Complete the course, then summarize! -->
This tutorial was contributed by [Debashish Reang](https://reangdeba.github.io/). Get in touch with me if you want to contribute, suggest improvements etc.

I plan to implement some of the common machine learning algorithms, and paradigms that can be viewed on any modern Web Browser (inspired by [@karpathy](https://twitter.com/karpathy) and his [convnetJS](http://convnetjs.com)) and do not require tedious setting up of libraries, environments, and what not!

I recently completed [Introduction to JavaScript on Codecademy](https://www.codecademy.com/courses/introduction-to-javascript/) as an early step towards executing my plan. **Why JavaScript, though?** JavaScript is primarily known as the language of most modern web browsers. The language continued to evolve and improve despite its initial quirks. JavaScript is a powerful, flexible, and fast programming language that is now being used for increasingly complex web development and beyond!

This tutorial **assumes** that the reader knows the basics of Programming, and Programming paradigms. You may want to check the full course (*link above*) in case this is the first time you are programming. God! Disclaimers are boring. Let's get to the fun part!

The Table of contents:
- [Basics](#basics)
- [Variables](#vars)
- [Conditionals](#cons)

<a name="basics"></a>
### Basics
**Numbers.** Integers and floats work as you'd expect them to:

```javascript
let x = 7;
console.log(typeof x); // output: number
console.log(x); // output: 7
console.log(x + 1); // output: 8
console.log(x - 1); // output: 6
console.log(x * 2); // output: 14
console.log(x--); // output: 6
console.log(x++); // output: 8
x += 1;
console.log(x); // output: 8
x *= 2;
console.log(x); // output: 16
x -= 2;
console.log(x); // output: 14
x /= 2;
console.log(x); // output: 7
// exponentiation using Math method and dot operator
let s = 3.5;
let y = Math.pow(s, 2);
console.log(y); // output: 12.25
console.log(typeof y); // output: number
```
For more gory details on Number Object, callable methods etc. etc., you can refer to [this documentation on Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number).

**Booleans.** JavaScript implements all of the usual operators for Boolean logic:
There are three logical operators: and (&&), or (||), not or bang operator (!).

```javascript
t = true;
f = false;
console.log(typeof t); // output: boolean
console.log(t && f); // output: false
console.log(t || f); // output:  true
console.log(!t); // output: false
console.log(t != f); // output: true
let cat = 'meow';
let sillycat = 'meou';
console.log(cat < sillycat); // output: false
```

**Strings.** JavaScript allows us to play around and manipulate strings quite neatly:

```javascript
let hello = 'hello';
let world = "world";
console.log(hello); // output: hello
console.log(hello.length); // output: 5
let hw = hello + ' ' + world;
console.log(hw); // output: hello world 
let r = 10
console.log(hw, 10); // output: hello world 10 
console.log(hello, world, r); // output: hello world 10
```

String objects have a bunch of neat methods:
```javascript
let hello = 'hello';
console.log(hello.toUpperCase()); // output: HELLO
console.log('      world'.trim()); // output: world
var str1 = 'Hello';
var str2 = 'World';
console.log(str1.concat(' ', str2)); // output: Hello World
console.log(str2.concat(', ', str1)); // output: World, Hello
// output: My name is Hello. My favorite city is World.
console.log(`My name is ${str1}. My favorite city is ${str2}.`);
```

As usual you can read up more about Strings, and String methods [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String).

**Ternary operator.** Take note of the `:`
```javascript
let favoritePhrase = 'Love That!';
// use === for checking equality. :P
favoritePhrase === ('Love That!') ?
console.log('I love that!') :
console.log("I don't love that!");
// prints "I love that!"
```

**`switch...case`** A switch statement provides an alternative syntax to `if...else` that is easier to read and write.

```javascript
let groceryItem = 'papaya';
switch (groceryItem) {
  case 'tomato':
    console.log('Tomatoes are $0.49');
    break;
  case 'lime':
    console.log('Limes are $1.49');
    break;
  case 'papaya':
    console.log('Papayas are $1.29');
    break;
  default:
    console.log('Invalid item');
    break;
}
// Prints 'Papayas are $1.29'
```
<!-- 
```javascript
// let allows variables to be re-assigned
let changeMe = true;
changeMe = false;
console.log(changeMe); // output: false

// const value cannot be changed. must initialize to a value.
const entree = 'Enchiladas';
console.log(entree); // output: Enchiladas
entree = 'Tacos'; // TypeError: Assignment to constant variable.
const testing; // SyntaxError: Missing initializer in const declaration
```
<a name="vars"></a>
### Variables
#### Declaration, and assignment
Variables can be declared using **var, let, & const**. The assignments works the same as you'd expect from other languages.

```javascript
var favoriteFood = 'pizza';
var numOfSlices = 8;
console.log(favoriteFood); // output: pizza
console.log(numOfSlices); // output: 8

// let allows variables to be re-assigned
let changeMe = true;
changeMe = false;
console.log(changeMe); // output: false

// const value cannot be changed. must initialize to a value.
const entree = 'Enchiladas';
console.log(entree); // output: Enchiladas
entree = 'Tacos'; // TypeError: Assignment to constant variable.
const testing; // SyntaxError: Missing initializer in const declaration
```

#### A few operations
Like many other languages, JavaScript has unary increment (x++) or decrement (x--) operators (*Python does not have these :P*).

```javascript
let levelUp = 10;
let powerLevel = 9001;
let multiplyMe = 32;
let quarterMe = 1152;

levelUp += 5;
powerLevel -= 100;
multiplyMe *= 11;
quarterMe /= 4;
 
console.log('levelUp:', levelUp); // output: 15
console.log('powerLevel:', powerLevel); // output: 8901 
console.log('multiplyMe:', multiplyMe); // output: 352
console.log('quarterMe:', quarterMe); // output: 288

let gainedDollar = 3;
let lostDollar = 50;

gainedDollar++; // 4
lostDollar--; // 49

let favoriteAnimal = 'dog';
console.log('My favorite animal:' + favoriteAnimal); // output: My favorite animal:dog

let myName = 'Reang';
let myCity = 'IITK';
// output: My name is Reang. My favorite city is IITK.
console.log(`My name is ${myName}. My favorite city is ${myCity}.`);

let newVariable = 'Playing around with typeof.';
console.log(typeof newVariable); // output: string
newVariable = 1;
console.log(typeof newVariable); // output: number
```

<a name='cons'></a>
### Conditionals

```javascript
let sale = true;
sale = false;

if(sale) {
  console.log('Time to buy!');
} 
else {
  console.log('Time to wait for a sale.');
}
``` -->

**Functions.** Some important concepts about functions.

**A function is a reusable block of code that groups together a sequence of statements to perform a specific task.**

A function declaration:

```javascript
function greet() {
  console.log('Hello, world!');
}

greet(); // prints 'Hello, world!'
```