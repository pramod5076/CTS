# Debugging Angular in VS Code

## Debugging Components

Example

```typescript
export class HomeComponent {

  title = "Student Portal";

  ngOnInit(){

      console.log("Loaded");

  }

}
```

Place a breakpoint inside `ngOnInit()`.

Run the debugger.

Execution pauses at the breakpoint.

---

## Debugging Services

Example

```typescript
getCourses(){

   return this.http.get<Course[]>(url);

}
```

Inspect:

- URL
- Response
- Variables
- Returned Observable

---

## Debugging TypeScript

Angular generates Source Maps.

Source Maps allow debugging original TypeScript instead of compiled JavaScript.

---

## Debugging State Management

Inspect Angular Services

Example

```typescript
courseService.courses
```

Inspect values during runtime.

---

## Debugging NgRx Store

Inspect

- Actions
- Reducers
- Selectors
- Effects
- Store State

Example

```
Courses Loaded

↓

Reducer Executes

↓

Store Updated

↓

Selector Emits

↓

Component Updated
```

---

## Debug Console

Evaluate expressions while paused.

Example

```typescript
this.courseService

this.selectedCourse

this.courses.length
```

---

## Best Practices

- Use breakpoints instead of excessive `console.log()`.
- Keep Source Maps enabled.
- Watch important variables.
- Debug TypeScript files instead of compiled JavaScript.
- Inspect services before checking UI issues.
- Use Redux DevTools alongside VS Code for NgRx applications.

---

## Summary

VS Code debugging helps developers inspect Angular components, services, TypeScript code, and NgRx state efficiently using breakpoints, watches, and the Debug Console.