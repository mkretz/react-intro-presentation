*   flow (https://flowtype.org/)
    *   static type checker for Javascript
    *   checks pure Javascript or annotated code
    *   annotations are stripped using Babel

```javascript
/* @flow */
function add(num1, num2) {
  return num1 + num2;
}
var x = add(3, '0');
console.log(x);```

```javascript
/* @flow */
function add(num1: number, num2: number): number {
  return num1 + num2;
}
var x: number = add(3, '0');
console.log(x);```
