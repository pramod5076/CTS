# Reactive Patterns in Angular

## Common Reactive Patterns

### HTTP Requests

```typescript
this.http.get(url).subscribe(data => {

  console.log(data);

});
```

---

### Form Value Changes

```typescript
this.form.valueChanges.subscribe(value => {

  console.log(value);

});
```

---

### Route Parameters

```typescript
this.route.params.subscribe(params => {

  console.log(params['id']);

});
```

---

### Search with switchMap

```typescript
searchControl.valueChanges.pipe(

  switchMap(term => this.http.get(url))

);
```

---

### Async Pipe

```html
<div>{{ users$ | async }}</div>
```

The `async` pipe automatically subscribes to and unsubscribes from an Observable.

---

## Best Practices

- Prefer Observables for asynchronous operations.
- Use the `async` pipe whenever possible.
- Unsubscribe from long-lived Observables to avoid memory leaks.
- Use `switchMap` for search and API calls that can be canceled.
- Handle errors with `catchError`.