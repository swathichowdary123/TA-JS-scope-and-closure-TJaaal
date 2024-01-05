Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.

- Take in account the different phases of execution, different execution contexts

1.

```js
var species = 'human';

function change() {
  var species = 'vampire';
  console.log(species);
}

console.log(species); - undefined
change();
console.log(species); - vampire
```

<!-- Put your image below -->

![](./img/image-name.jpg)

- Create the execution context diagram
- What will be the value of species on 1 and 2

2.

```js
var topLevelVar = 'This is global scope!';

function topLevelFn() {
  var localVar = "This is local to topLevelFn's scope";

  function nestedFn() {
    var anotherLocalVar = "Local to nestedFn's scope.";

    console.log(localVar); -this is local scope
    console.log(topLevelVar); - undefined
  }

  nestedFn();
}

topLevelFn();
```

<!-- Put your image below -->

![](./img/image-name.jpg)

- Create the execution context diagram
- What will be the value of 1 and 2

3.

```js
var one = 'One';
var two = 'Two';

function main() {
  var three = 'Three';

  function inner() {
    var four = 'Four';

    console.log(one); - one
    console.log(two); - two
    console.log(three); -three
  }
  console.log(four); -four
  inner();
}

main();
console.log(one, two, three, four); -one,two,three,four
```

<!-- Put your image below -->

![](./img/image-name.jpg)

- Create the execution context diagram
- What will be the value of 1, 2, 3, 4 and 5 or error if the code does not work
