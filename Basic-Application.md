# Content

- Profile Lookup
- Generate Random Fractions with JavaScript
- Generate Random Whole Numbers with JavaScript
- Generate Random Whole Numbers within a Range
- Use the parseInt Function
- Use the parseInt Function with a Radix
- Use the Conditional (Ternary) Operator
- Use Multiple Conditional (Ternary) Operators
- Use Recursion to Create a Countdown
- Use Recursion to Create a Range of Numbers

[1.Profile Lookup](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/profile-lookup)

```js
// Setup
var contacts = [
  {
    firstName: 'Akira',
    lastName: 'Laine',
    number: '0543236543',
    likes: ['Pizza', 'Coding', 'Brownie Points'],
  },
  {
    firstName: 'Harry',
    lastName: 'Potter',
    number: '0994372684',
    likes: ['Hogwarts', 'Magic', 'Hagrid'],
  },
  {
    firstName: 'Sherlock',
    lastName: 'Holmes',
    number: '0487345643',
    likes: ['Intriguing Cases', 'Violin'],
  },
  {
    firstName: 'Kristian',
    lastName: 'Vos',
    number: 'unknown',
    likes: ['JavaScript', 'Gaming', 'Foxes'],
  },
];

function lookUpProfile(name, prop) {
  // Only change code below this line
  let checkHaveName = false;
  let checkHaveProp = false;
  for (let value of contacts) {
    if (value['firstName'] === name) {
      checkHaveName = true;
      for (let key in value) {
        if (key === prop) {
          checkHaveProp = true;
        }
      }
      if (checkHaveName && checkHaveProp) return value[prop];
      return 'No such property';
      break;
    }
  }
  return 'No such contact';
  // Only change code above this line
}

lookUpProfile('Kristian', 'lastName');
```

[2.Generate Random Fractions with JavaScript](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/generate-random-fractions-with-javascript)

```js
function randomFraction() {
  // Only change code below this line

  return Math.random() * 10 + 1;

  // Only change code above this line
}
```

[3.Generate Random Whole Numbers with JavaScript](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/generate-random-whole-numbers-with-javascript)

```js
function randomWholeNum() {
  // Only change code below this line

  return Math.floor(Math.random() * 10);
}
```

[4.Generate Random Whole Numbers within a Range](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/generate-random-whole-numbers-within-a-range)

```js
function randomRange(myMin, myMax) {
  // Only change code below this line
  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;
  // Only change code above this line
}
```

[5.Use the parseInt Function](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-the-parseint-function)

```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger('56');
```

[6.Use the parseInt Function with a Radix](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-the-parseint-function-with-a-radix)

```js
function convertToInteger(str) {
  return parseInt(str, 2);
}

convertToInteger('10011');
```

[7.Use the Conditional (Ternary) Operator](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-the-conditional-ternary-operator)

```js
// Finish and Paste your solution here
```

[8.Use Multiple Conditional (Ternary) Operators](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators)

```js
function checkSign(num) {
  return num > 0 ? 'positive' : num < 0 ? 'negative' : 'zero';
}

checkSign(10);
```

[9.Use Recursion to Create a Countdown](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-recursion-to-create-a-countdown)

```js
// Only change code below this line
// ใช้ recursive
function countdown(n) {
  if (n < 1) {
    return [];
  } else {
    const countArray = countdown(n - 1);
    countArray.unshift(n);
    return countArray;
  }
}
countdown(10);
countdown(5);
// Only change code above this line
```

[10.Use Recursion to Create a Range of Numbers](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-recursion-to-create-a-range-of-numbers)

```js
// Finish and Paste your solution here
```
