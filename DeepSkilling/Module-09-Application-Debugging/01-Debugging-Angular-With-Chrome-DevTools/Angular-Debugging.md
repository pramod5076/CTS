# Debugging Angular Applications

## TypeScript Source Maps

Angular generates Source Maps during development.

Source Maps allow developers to debug TypeScript instead of compiled JavaScript.

---

## Run Angular

```bash
ng serve
```

---

## Debug Components

Example

```typescript
export class HomeComponent {

  title = "Student Portal";

}
```

Place a breakpoint on

```typescript
title = "Student Portal";
```

Chrome DevTools pauses execution at that line.

---

## Debug Lifecycle Hooks

```typescript
ngOnInit(){

   console.log("Component Loaded");

}
```

Add a breakpoint inside `ngOnInit()`.

---

## Debug Services

```typescript
getCourses(){

   return this.http.get(...);

}
```

Pause execution before the HTTP request.

---

## Debug HTTP Requests

Use the **Network** panel to inspect:

- Request URL
- Method
- Status Code
- Response Body
- Response Time

---

## Best Practices

- Use breakpoints instead of excessive `console.log()`.
- Keep Source Maps enabled during development.
- Check the Console for runtime errors first.
- Use the Network panel for API debugging.
- Remove unnecessary debug statements before production builds.

---

## Summary

Angular debugging combines Chrome DevTools, TypeScript Source Maps, and Angular CLI to efficiently identify and resolve issues in components, services, and HTTP requests.