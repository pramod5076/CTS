# Common RxJS Operators

## map

Transforms emitted values.

```typescript
numbers.pipe(
  map(value => value * 2)
);
```

---

## filter

Filters emitted values.

```typescript
numbers.pipe(
  filter(value => value > 5)
);
```

---

## switchMap

Switches to a new Observable and cancels the previous one.

```typescript
search.pipe(
  switchMap(value => this.http.get(url))
);
```

Useful for search boxes and autocomplete.

---

## mergeMap

Subscribes to multiple Observables simultaneously.

```typescript
items.pipe(
  mergeMap(item => this.http.get(url))
);
```

---

## catchError

Handles Observable errors.

```typescript
this.http.get(url).pipe(
  catchError(error => {
    console.log(error);
    return throwError(() => error);
  })
);
```

---

## Why Use Operators?

- Transform data
- Filter data
- Combine streams
- Handle errors
- Improve readability