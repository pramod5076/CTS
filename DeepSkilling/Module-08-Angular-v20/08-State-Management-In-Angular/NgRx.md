# NgRx State Management

## What is NgRx?

NgRx is a Redux-inspired state management library for Angular. It stores the application state in a centralized Store and updates it using Actions and Reducers.

---

## Install NgRx

```bash
ng add @ngrx/store
```

---

## Core Concepts

### Store

A centralized container that holds the application's state.

---

### Actions

Actions describe events that request a state change.

```typescript
export const loadUsers = createAction(
  '[User] Load Users'
);
```

---

### Reducers

Reducers are pure functions that update the Store based on Actions.

```typescript
export const userReducer = createReducer(
  initialState
);
```

---

### Effects

Effects handle asynchronous operations like HTTP requests.

---

### Selectors

Selectors retrieve specific pieces of data from the Store.

```typescript
this.store.select(selectUsers);
```

---

## Benefits

- Centralized state
- Predictable state updates
- Better debugging
- Scalable for enterprise applications