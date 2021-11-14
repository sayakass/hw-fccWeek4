# Rest,Spread Operator (2ข้อ)

# Prerequisite

- Function
- Array

[1.Use the Rest Parameter with Function Parameters](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-the-rest-parameter-with-function-parameters)

```js
const sum = (...args) => {
  return args.reduce((a, b) => a + b, 0);
};
```

[2.Use the Spread Operator to Evaluate Arrays In-Place](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/use-the-spread-operator-to-evaluate-arrays-in-place)

```js
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;

arr2 = [...arr1]; // Change this line

console.log(arr2);
```
