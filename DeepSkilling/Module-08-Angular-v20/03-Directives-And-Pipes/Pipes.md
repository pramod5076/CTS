# Angular Pipes

## Built-in Pipes

### Uppercase

```html
{{name | uppercase}}
```

---

### Lowercase

```html
{{name | lowercase}}
```

---

### Date

```html
{{today | date}}
```

---

### Currency

```html
{{salary | currency}}
```

---

### Number

```html
{{marks | number:'1.2-2'}}
```

---

### Percent

```html
{{percentage | percent}}
```

---

## Custom Pipe

Create

```bash
ng generate pipe titlecase
```

Example

```typescript
transform(value:string)
{
   return value.toUpperCase();
}
```