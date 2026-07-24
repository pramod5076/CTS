# Lazy Loading

## What is Lazy Loading?

Lazy Loading loads feature modules only when required instead of loading everything during application startup.

---

## Benefits

- Faster Application Startup
- Reduced Bundle Size
- Better Performance
- Improved User Experience

---

## Generate Module

```bash
ng generate module admin --route admin --module app.module
```

---

## Route Configuration

```typescript
{
 path:'admin',

 loadChildren:()=>

 import('./admin/admin.module')

 .then(m=>m.AdminModule)
}
```

---

## Nested Routes

```typescript
{
 path:'employee',

 children:[
 {
 path:'details',
 component:EmployeeDetailsComponent
 }
 ]
}
```

---

## Best Practices

- Lazy load feature modules.
- Protect routes using guards.
- Use route parameters for dynamic pages.
- Keep routing modules modular.