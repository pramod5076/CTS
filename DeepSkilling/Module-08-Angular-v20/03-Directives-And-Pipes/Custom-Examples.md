# Custom Directive Example

```typescript
@Directive({
 selector:'[appHighlight]'
})
```

Apply

```html
<p appHighlight>
Hello Angular
</p>
```

---

# Custom Pipe Example

```typescript
@Pipe({
 name:'reverse'
})
```

Usage

```html
{{name | reverse}}
```

---

## Benefits

- Reusable
- Cleaner Templates
- Better Maintainability