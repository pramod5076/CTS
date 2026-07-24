# HTTP Interceptors

## What are HTTP Interceptors?

HTTP Interceptors intercept every outgoing request and incoming response. They are commonly used for authentication, logging, loading indicators, and centralized error handling.

---

## Create an Interceptor

```bash
ng generate interceptor auth
```

---

## Example

```typescript
intercept(req: HttpRequest<any>, next: HttpHandler) {

  const authReq = req.clone({

    setHeaders: {
      Authorization: 'Bearer TOKEN'
    }

  });

  return next.handle(authReq);
}
```

---

## Common Use Cases

- Add Authorization Headers
- JWT Authentication
- Global Error Handling
- Request Logging
- Response Logging
- Loading Spinner
- API Request Timing

---

## Benefits

- Centralized request handling
- Cleaner service code
- Improved security
- Reusable logic
- Better maintainability

---

## Best Practices

- Keep interceptors lightweight.
- Avoid business logic inside interceptors.
- Use separate interceptors for authentication, logging, and error handling.