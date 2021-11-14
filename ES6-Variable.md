# Declare Variable in ES6 (5ข้อ)

# Prerequisite

- declare variable with var
- scope
- basic Array

[1.Explore Differences Between the var and let Keywords](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/explore-differences-between-the-var-and-let-keywords)

```js
// Finish and Paste your solution here
```

[2.Compare Scopes of the var and let Keywords](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/compare-scopes-of-the-var-and-let-keywords)

```js
function checkScope() {
  let i = 'function scope';
  if (false) {
    i = 'block scope';
    console.log('Block scope i is: ', i);
  }
  console.log('Function scope i is: ', i);
  return i;
}
```

[3.Declare a Read-Only Variable with the const Keyword](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/declare-a-read-only-variable-with-the-const-keyword)

```js
// Finish and Paste your solution here
```

[4.Mutate an Array Declared with const](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/mutate-an-array-declared-with-const)

```js
// Finish and Paste your solution here
```

[5.Prevent Object Mutation](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/es6/prevent-object-mutation)

```js
function freezeObj() {
  const MATH_CONSTANTS = {
    PI: 3.14,
  };
  // Only change code below this line
  Object.freeze(MATH_CONSTANTS);

  // Only change code above this line
  try {
    MATH_CONSTANTS.PI = 99;
  } catch (ex) {
    console.log(ex);
  }
  return MATH_CONSTANTS.PI;
}
const PI = freezeObj();
```
