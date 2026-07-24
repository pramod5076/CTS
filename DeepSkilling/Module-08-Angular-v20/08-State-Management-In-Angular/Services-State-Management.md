# Using Services for State Management

## What is a Service?

A Service is an injectable class used to share business logic and data between components.

---

## Generate a Service

```bash
ng generate service shared/data
```

or

```bash
ng g s shared/data
```

---

## Example Service

```typescript
@Injectable({
  providedIn: 'root'
})
export class DataService {

  private username = 'Pramod';

  getUser() {
    return this.username;
  }

  setUser(name: string) {
    this.username = name;
  }
}
```

---

## Using the Service

```typescript
constructor(private dataService: DataService) {}

ngOnInit() {
  console.log(this.dataService.getUser());
}
```

---

## Advantages

- Easy to implement
- Shared across components
- Less boilerplate
- Suitable for small and medium-sized applications