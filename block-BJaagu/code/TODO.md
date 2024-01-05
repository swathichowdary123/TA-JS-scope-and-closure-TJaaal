Find the output of the code snippets below:

```js
console.log(numA + numB); -51
var numA = 21,
  numB = 30;
```

Find the output of the code snippets below:

```js
console.log(numA + numB); -numA is used before declared
let numA = 21,
  numB = 30;
```

Find the output of the code snippets below:

```js
let numA = 21,
  numB = 30;
console.log(numA + numB); -51
```

Find the output of the code snippets below:

```js
console.log(sayHello()); -hello
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}
```

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); -tyrion
function sayHello() {
  console.log(username);
}
```

Find the output of the code snippets below:

```js
sayHello(); -undefined
let username = "Tyrion";
function sayHello() {
  console.log(username);
}
```

Find the output of the code snippets below:

```js
let username = "Tyrion";
sayHello(); -in javascript variable declaration is not hoisted
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
sayHello(); -in javascript variable declaration is not hoisted
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
sayHello(); -in javascript variable declaration is not hoisted
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
sayHello(); -in javascript variable declaration is not hoisted
let sayHello = () => {
  console.log(username);
};
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); -undefined
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello();-john
```

Find the output of the code snippets below:

```js
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); -cannot access username before initialization
```