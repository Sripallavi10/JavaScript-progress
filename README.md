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
