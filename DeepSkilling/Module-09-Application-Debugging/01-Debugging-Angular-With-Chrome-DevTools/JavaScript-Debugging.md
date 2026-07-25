# Debugging JavaScript

## Sources Panel

The Sources panel allows developers to debug JavaScript code.

---

## Breakpoints

A breakpoint pauses program execution at a selected line.

Example

```javascript
let total = 100;

debugger;

total += 50;

console.log(total);
```

Execution stops at the `debugger` statement.

---

## Step Controls

- Resume
- Step Over
- Step Into
- Step Out

---

## Call Stack

The Call Stack shows the sequence of function calls leading to the current execution point.

Example

```javascript
function first(){

    second();

}

function second(){

    third();

}

function third(){

    debugger;

}

first();
```

Call Stack

```
third()

↓

second()

↓

first()
```

---

## Watch Expressions

Watch variables during debugging.

Example

```
studentName

courseCount

isLoggedIn
```

---

## Console During Debugging

Evaluate expressions while execution is paused.

Example

```javascript
course.length

student.name
```