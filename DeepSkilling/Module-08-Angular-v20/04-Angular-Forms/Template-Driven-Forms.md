# Template-Driven Forms

## Import FormsModule

```typescript
import { FormsModule } from '@angular/forms';
```

---

## Two-Way Data Binding

```html
<input
type="text"
[(ngModel)]="username">
```

---

## Form Example

```html
<form #myForm="ngForm">

<input
name="username"
[(ngModel)]="username"
required>

<button type="submit">
Submit
</button>

</form>
```

---

## Form Submission

```typescript
submit()
{
    console.log(this.username);
}
```

---

## Advantages

- Easy to learn
- Less code
- Best for simple forms