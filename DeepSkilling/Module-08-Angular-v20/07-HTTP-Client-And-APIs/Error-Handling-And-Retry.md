# Error Handling and Retry Strategies

## Error Handling

Use `catchError()` to handle API errors gracefully.

```typescript
this.http.get(url).pipe(
  catchError(error => {
    console.log(error);
    return throwError(() => error);
  })
);
```

---

## Retry Strategy

Retry failed requests automatically.

```typescript
this.http.get(url).pipe(
  retry(3)
);
```

---

## Common HTTP Status Codes

| Code | Meaning |
|------|---------|
| 200 | OK |
| 201 | Created |
| 400 | Bad Request |
| 401 | Unauthorized |
| 403 | Forbidden |
| 404 | Not Found |
| 500 | Internal Server Error |

---

## Best Practices

- Handle all API errors.
- Display user-friendly messages.
- Retry only temporary failures.
- Log errors for debugging.