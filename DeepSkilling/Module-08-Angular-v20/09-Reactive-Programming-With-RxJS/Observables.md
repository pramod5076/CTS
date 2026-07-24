# RxJS Observables

## What is an Observable?

An Observable is a stream of data that emits values over time. Components can subscribe to an Observable and react whenever new data is emitted.

---

## Creating an Observable

```typescript
import { Observable } from 'rxjs';

const numbers = new Observable(observer => {

  observer.next(1);

  observer.next(2);

  observer.complete();

});
```

---

## Subscribing to an Observable

```typescript
numbers.subscribe(value => {

  console.log(value);

});
```

---

## Why Use Observables?

- Supports asynchronous programming
- Multiple emitted values
- Lazy execution
- Easy cancellation using unsubscribe()

---

## Observable vs Promise

| Observable | Promise |
|------------|----------|
| Multiple values | Single value |
| Lazy execution | Executes immediately |
| Cancelable | Not cancelable |
| Supports operators | Limited support |