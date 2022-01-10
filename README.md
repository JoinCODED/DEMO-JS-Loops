# Loops Demo 🔁

This demo shows how to use loops and goes over the main topics of `while` and the C-`for` loop

## Objective

To show the importance of counter loops and transit from while to for

# Steps

## If VS While

```js
// 1. Create a variable, an if statement to see if the variable is less than a number
let counter = 0;
if (counter < 10) {
  console.log(`IF# counter is ${counter}, and I am inside the if statement`);
}
// 2. Create a while loop
// the code will crash here, force stop it (control + C)
while (counter < 10) {
  console.log(`WHILE# counter is ${counter}, and I am inside the while `);
}

// 3. As long as the condition is true, it's going to loop.
// How can we make it false?
// Let's increment the counter after every loop
// run, it should work!
while (counter < 10) {
  console.log(`WHILE# counter is ${counter}, and I am inside the while `);
  counter++;
}
```

## While VS For

The structure of while with the counter is as follows

1. counter initial point `let counter = 0`
2. condition to stop the counter (end point) `(counter < 10)`
3. increment statement to move the counter toward the end point (incrementally or decremental) `counter++`

Those 3 parts were conducted into one part, called `for`

```js
for (INITIAL_STATE; CONDITION; INCREMENT) {
  // code here will be looping from initial state to condition
}

// 1. Convert the while to a for
for (let counter2 = 0; counter2 < 10; counter2++) {
  console.log(`FOR# counter is ${counter2}, and I am inside the for `);
}
// Check that you have access to the counter at every single loop
```

## loop inside a loop ➿

```js
// 1. What happens if we add a for inside a for?

for (let i = 0; i < 3; i++) {
  console.log(`I: ${i}`);
  for (let j = 0; j < 3; j++) {
    console.log(`J: ${j}`);
  }
}
```
