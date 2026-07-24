
---

# 📄 Dependency-Injection.md

````md
# Dependency Injection

## Constructor Injection

```typescript
constructor(private employeeService: EmployeeService) {}
```

Angular automatically injects the required service.

---

## Types of Dependencies

- Services
- HTTP Client
- Router
- FormBuilder

---

## Advantages

- Loose Coupling
- Better Testing
- Easy Maintenance
- Code Reusability