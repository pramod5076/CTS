# Angular Validation

## Built-in Validators

```typescript
Validators.required

Validators.email

Validators.minLength(5)

Validators.maxLength(20)

Validators.pattern()
```

---

## Example

```typescript
name:['',Validators.required]
```

---

## Multiple Validators

```typescript
email:['',[

Validators.required,

Validators.email

]]
```

---

## Custom Validator

```typescript
export function ageValidator()
{
return(control:any)=>
{
return null;
}
}
```

---

## Error Message

```html
<div *ngIf="name.invalid">
Name is required
</div>
```

---

## Best Practices

- Validate on both client and server
- Display meaningful error messages
- Use Reactive Forms for complex applications