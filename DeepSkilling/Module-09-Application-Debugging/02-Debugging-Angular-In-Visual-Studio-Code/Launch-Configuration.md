# launch.json Configuration

## What is launch.json?

The `launch.json` file defines how VS Code starts and attaches the debugger.

Location:

```
.vscode/launch.json
```

---

## Example Configuration

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "chrome",
            "request": "launch",
            "name": "Launch Chrome",
            "url": "http://localhost:4200",
            "webRoot": "${workspaceFolder}"
        }
    ]
}
```

---

## Start Debugging

1. Run

```bash
ng serve
```

2. Press

```
F5
```

3. Chrome launches automatically.

---

## Breakpoints

Click beside a line number.

A red dot indicates a breakpoint.

Execution pauses when that line executes.

---

## Watches

Watch variables such as:

```
course

student

isLoggedIn

selectedCourse
```

Watches automatically update during debugging.

---

## Variables Panel

Displays:

- Local Variables
- Global Variables
- Function Parameters