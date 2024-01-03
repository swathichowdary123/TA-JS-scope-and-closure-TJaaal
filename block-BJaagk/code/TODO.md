1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
 return(marks*100)/total;
}

// Your code goes here
const percentage=function(marks,total){
   return(marks*100)/total;
}
//Arrow function
const percentage=(marks,total)=>return(marks*100)/total;
//named function
const percentage=function calculatePercentage(marks,total){
  return(marks*100)/total;
};
```


2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
}; 
function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
function defintion
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
function expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
In javascript ,function definitions are expressions because it results a value.This allows function to be assignmed to variables,passed as arguments to other functions ,or used in various expression.
const multiply=function(x,y){
  return x*y;
};

4. Why is a function call an expression in JavaScript?
In javascript function call is considered an expression because it produces a value.when you invoke a function ,it returns an result ,and this result can be used in assignments ,calculations and other expressions.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); - valid
five = add; -valid
five = five(10, 11); -invalid
five = function () {
  return 'Hello';
}; -valid
```

6. What is the difference between function definition and function call? Explain with an example.
Function defintion involves declaring the structure and behaviour of a function.In example add is defined as function that takes two parameters a and b and return their sum.
function add(a,b){
  return a+b;
} 
function call is the actual inovocation or execution of a function.In this example add(2,3) calls the previously defined add function with arguments 2 and 3.the result is then assigned to the variable result.
let result=add(2,3);

7. What is the similarities between function definition and function call?
Name usage,Parenthesis,Code block,Function as a named entity.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
valid.
the code is valid.In javascript ,functions are first-class-citizens,meaning they can have properties just like an other object.In this case,the function hello is defined ,and then a property name user is assigned to it with the value sam.
```

9. What is higher order function explain with an example.
A function that accepts a function definition as an argument is known as higher order function.
function filterEven(arr){
  return function(){};
}

10. Explain what is callback function. Why you can pass a function inside a function?
A callback function is a function that is passed as an argument to another function and is executed after the completion of a specific task.In javascript you can pass a function into another function becuse functions are the first class citizens.This means functions can be treated like any other value-assigned to variables,passed as an arguments to other functions,and returned as a values from other functions.
