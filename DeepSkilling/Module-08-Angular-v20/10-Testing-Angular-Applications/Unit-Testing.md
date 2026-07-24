# Unit Testing with Jasmine and Karma

## What is Unit Testing?

Unit Testing tests individual units such as components, services, or pipes in isolation.

---

## Jasmine

Jasmine is a behavior-driven testing framework used for writing test cases.

---

## Karma

Karma is a test runner that executes Jasmine tests in browsers.

---

## Run Tests

```bash
ng test
```

---

## Sample Test

```typescript
describe('Calculator', () => {

  it('should add numbers', () => {

    expect(2 + 3).toBe(5);

  });

});
```

---

## Common Jasmine Functions

- describe()
- it()
- expect()
- beforeEach()
- afterEach()

---

## Benefits

- Fast execution
- Isolated testing
- Easy debugging