# Exercises - Chapter 3

## Minimum

``` js
function min(x, y) {
  if (x <= y) 
    return x
  else 
    return y
  }
  
console.log(min(0, 10));
// → 0
console.log(min(0, -10));
// → -10
```

## Recursion

```js
function isEven(x) {
  if (x < 0)
    x = -x
  
  if (x === 1) 
    return false
  else if (x === 0)
    return true
  else 
    return isEven(x - 2)
  }

console.log(isEven(50));
// → true
console.log(isEven(75));
// → false
console.log(isEven(-1));
// → ??
```

## Bean counting

```js
function countBs(s) {
  return countChar(s, "B")
  }

function countChar(str, character) {
  let counter = 0
  for (let i = 0; i < str.length; i++) {
    if (str[i] === character)
      counter += 1
    }
  return counter
  }

console.log(countBs("BOB"));
// → 2
console.log(countChar("kakkerlak", "k"));
// → 4
```