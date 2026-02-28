# Exercises - Chapter 1

## Looping a triangle

```js
let s = "";
while (s.length < 7) {
  s = s + "#";
  console.log(s)
}
```

## FizzBuzz

```js
for (let i = 1; i <= 100; i++) {
  if (i % 3 === 0 && i % 5 === 0)
    {
      console.log("FizzBuzz")
    }
  else if (i % 3 === 0) {
    console.log("Fizz")
    }
  else if (i % 5 === 0) {
    console.log("Buzz")
    }
  else console.log(i);
  }
  ```

  ## Chessboard


```js
let size = 8
let s = ""

for (let x = 0; x < size; x++) {
  for (let i = 0; i < size; i++ ) {
    if (s.length % 2 === 0) {
      s = s + " ";
    } else {
      s = s + "#"
    } 
  }
  
  s = s + `\n`;
}

console.log(s)
```