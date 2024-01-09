For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
var username, numbers;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage;

// Execution Phase

console.log(username, numbers);

username = 'Arya';
number = 21;

message = sayHello(username);
nextMessage = sayHello('Test');
```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
let username, numbers;
let number;
let sayHello;
let message;
var nextMessage;

// Execution Phase
console.log(username, numbers); // Error: Cannot access 'username' before initialization
username = 'Arya';
number = 21;

sayHello = function (name) {
  return `Hello ${name}`;
};

message = sayHello(username);
nextMessage = sayHello('Test');
```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
let username;
let numbers;
let number;
let message;
let sayHello;
var nextMessage;

// Execution Phase
username = 'Arya';
console.log(username, numbers); // undefined, undefined

number = 21;
message = sayHello(username); // TypeError: sayHello is not a function

sayHello = function (name) {
  return `Hello ${name}`;
};

nextMessage = sayHello('Test');
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
var name;
let age;

// Execution Phase
console.log(name); // undefined
console.log(age); // ReferenceError: age is not defined
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
// Your code goes here
function sayHi(name) {
  var name;
  let age;

  console.log(name); // undefined
  console.log(age); // ReferenceError: age is not defined

  name = 'Lydia';
  age = 21;
}

sayHi();
```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
// Your code goes here
//declaration phase
function sayHi(name);
var name;
let age;
//execution phase
sayHi(); // undefined, ReferenceError: age is not defined

function sayHi(name) {
  var name;
  let age;

  console.log(name); // undefined
  console.log(age); // ReferenceError: age is not defined

  name = 'Lydia';
  age = 21;
}
```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
let sayHi;

// Execution Phase
sayHi(); // TypeError: sayHi is not a function

sayHi = function (name) {
  var name;
  let age;

  console.log(name); // undefined
  console.log(age); // ReferenceError: age is not defined
}
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
// Your code goes here
// Declaration Phase
let num1;
var sum;
let num2;

// Execution Phase
num1 = 21;
console.log(sum); // undefined

sum = num1 + num2; // num2 is undefined here
num2 = 30;
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
// Your code goes here
var num1;
let sum2;
let add;
function addAgian;

// Execution Phase
num1 = 21;
num2 = 200;

sum2 = addAgain(num1, num2, 4, 5, 6);

add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};

addAgian = function (a, b) {
  return a + b;
};

let sum = add(num1, num2, 4, 5, 6);
```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
// Your code goes here
function test;
let sum;
let add;

// Execution Phase
test = function (a) {
  let num1 = 21;
  return add(a, num1);
};

sum = test(100);

add = (a, b) => {
  return a + b;
};
```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
// Your code goes here
//declaration phase
function test;
let sum;
function add;
//execution phase
test = function (a) {
  let num1 = 21;
  return add(a, num1);
};

sum = test(100);

add = function (a, b) {
  return a + b;
}
```
