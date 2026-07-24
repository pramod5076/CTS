# Dependency Injection and Services in Angular

## What is Dependency Injection?

Dependency Injection (DI) is a design pattern where Angular provides the required dependencies (services) to a class instead of the class creating them itself.

---

## Why Dependency Injection?

- Promotes loose coupling
- Improves code reusability
- Simplifies testing
- Makes applications easier to maintain

---

## What are Services?

Services are reusable classes used to share business logic, data, or functionality across multiple components.

Examples:

- Authentication Service
- Employee Service
- Product Service
- Logging Service
- API Service

---

## Injectable Decorator

Angular uses the `@Injectable()` decorator to define a service that can participate in Dependency Injection.

Example:

```typescript
@Injectable({
  providedIn: 'root'
})