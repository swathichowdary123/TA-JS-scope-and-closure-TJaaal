1. What does thread of execution means in JavaScript?
javascript goes through code line by line and executes it known as thread of execution.
2. Where the JavaScript code gets executed?
 Global execution context
3. What does context means in Global Execution Context?
global execution context is created whwn a javascript script first starts to run,and it represents the global scope in javascript.
4. When do you create a global execution context.
global execuion context is running our code when javascript engine is running our code.
5. Execution context consists of what all things?
it contains information about the variables,functions,and objects that are available to the code beign executed.
6. What are the different types of execution context?
global and function execution context
7. When global and function execution context gets created?
the global execution context is created when a javacsript script first starts to run.a function execution context is created whenever a function is called.
8. Function execution gets created during function execution or while declaring a function.
it is created whenever a function is called.

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)