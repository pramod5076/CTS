# Hierarchical Dependency Injection

Angular supports different levels of Dependency Injection.

---

## Root Level

```typescript
@Injectable({
  providedIn: 'root'
})
```

Available throughout the application.

---

## Module Level

```typescript
providers: [EmployeeService]
```

Service is available only within that module.

---

## Component Level

```typescript
@Component({
  providers: [EmployeeService]
})
```

Creates a new instance for that component and its child components.

---

## Comparison

| Level | Scope |
|--------|-------|
| Root | Entire Application |
| Module | Specific Module |
| Component | Component & Children |

---

## Best Practices

- Use Root-level services for shared data.
- Use Module-level services for feature-specific functionality.
- Use Component-level services when each component needs its own service instance.