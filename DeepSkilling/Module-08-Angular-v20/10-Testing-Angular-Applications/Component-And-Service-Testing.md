# Component and Service Testing

## Component Testing

Component Testing verifies component creation, rendering, and user interactions.

Example

```typescript
beforeEach(() => {

  TestBed.configureTestingModule({

    declarations: [AppComponent]

  });

});
```

---

## Verify Component Creation

```typescript
it('should create component', () => {

  expect(component).toBeTruthy();

});
```

---

## Service Testing

Service Testing verifies business logic inside Angular services.

Example

```typescript
it('should return users', () => {

  expect(service.getUsers()).toBeTruthy();

});
```

---

## TestBed

TestBed creates a testing environment similar to the Angular runtime.

---

## Best Practices

- Test one feature at a time.
- Keep tests independent.
- Use mocks for external dependencies.