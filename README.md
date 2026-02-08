# JavaScript-progress
JavaScript is a high-level, interpreted programming language mainly used to make web pages interactive and dynamic. JavaScript is  a programming language that is used to create  webssite.
With JavaScript, you can:

Respond to user actions (clicks, typing, scrolling)

Change HTML and CSS dynamically

Validate forms

Create animations

Build web apps (with frameworks like React, Node.js, etc.)
Example:
When you click a button and a message pops up, that’s JavaScript at work.
<!DOCTYPE html>
<html>
<body>
  <h1>JS Console Example</h1>

  <script>
    console.log("JS running from HTML file");
  </script>
</body>
</html>
🔹 VARIABLES in JavaScript
What a variable actually is

A variable is just a named storage box for data in memory.

let score = 10;


You can:

read it

update it

use it in logic

The 3 ways to create variables (IMPORTANT)
1️⃣ let (use this most of the time)
let count = 0;
count = 5;


Can change value

Block scoped

✅ Best default choice

2️⃣ const (cannot be reassigned)
const PI = 3.14;


Value can’t be reassigned

Used for values that should not change

⚠️ Objects/arrays can still be modified

const arr = [1, 2];
arr.push(3); // allowed

3️⃣ var (avoid this)
var x = 10;


Function scoped

Causes bugs

🔹 FUNCTIONS in JavaScript
What a function really is
A function is a reusable block of logic.

Instead of repeating code, you wrap it.

Function Declaration (classic)
function add(a, b) {
    return a + b;
}
Call it:

add(2, 3); // 5
Function Expression
const multiply = function(a, b) {
    return a * b;
};
Used when assigning functions to variables.

Arrow Function (modern & common)
const subtract = (a, b) => {
    return a - b;
};
Short version:

const subtract = (a, b) => a - b;
🔹 Parameters vs Arguments (DON’T CONFUSE)
function greet(name) {   // parameter
    console.log(name);
}

greet("Pallavi");        // argument
🔹 Return vs Console.log (BIG beginner mistake)
function add(a, b) {
    console.log(a + b); // prints only
}
❌ You cannot use the result later.

Correct:

function add(a, b) {
    return a + b;
}
🔹 Scope (WHY your code breaks)
let x = 10;

function test() {
    let y = 5;
}
What is a Boolean?

A Boolean is a data type that has only two values:

true
false


That’s it. No in-between. Think YES / NO, ON / OFF, 1 / 0.

Creating Booleans
let isLoggedIn = true;
let isAdmin = false;


You don’t need quotes — "true" is a string, not a boolean ❌

Booleans from Comparisons

Most booleans come from comparisons:

5 > 3        // true
10 < 5       // false
5 == 5       // true
5 != 3       // true

Strict comparison (important!)
5 == "5"     // true  (checks value only)
5 === "5"    // false (checks value + type)


👉 Always prefer === in real projects.

Booleans in Conditions (Very Important)

Booleans are mainly used in if, else, and loops.

let age = 18;

if (age >= 18) {
    console.log("You can vote");
} else {
    console.log("You cannot vote");
}

Boolean Logical Operators
AND (&&)
true && true   // true
true && false  // false

OR (||)
true || false  // true
false || false // false

NOT (!)
!true   // false
!false  // true


Example:

let isLoggedIn = true;
let hasPermission = false;

if (isLoggedIn && hasPermission) {
    console.log("Access granted");
} else {
    console.log("Access denied");
}

Truthy and Falsy Values

Some values behave like false even if they’re not booleans.

Falsy values:
false
0
""
null
undefined
NaN


Everything else is truthy 😎

Example:

if ("hello") {
    console.log("This runs"); // true
}

if (0) {
    console.log("This won't run");
}

Boolean Function

You can convert values to boolean:

Boolean(1);        // true
Boolean(0);        // false
Boolean("Hi");     // true
Boolean("");       // false

Real-Life Example
let isDarkMode = false;

if (!isDarkMode) {
    console.log("Light mode is ON");
}

