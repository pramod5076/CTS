# Reactive Forms

## Import Module

```typescript
import { ReactiveFormsModule } from '@angular/forms';
```

---

## FormBuilder

```typescript
constructor(private fb:FormBuilder){}
```

---

## Create Form

```typescript
employeeForm=this.fb.group({

name:[''],

email:['']

});
```

---

## FormControl

Represents a single form field.

---

## FormGroup

Represents a collection of FormControls.

---

## FormArray

Represents a dynamic list of controls.

---

## Submit

```typescript
submit()
{
console.log(this.employeeForm.value);
}
```

---

## Advantages

- Scalable
- Better validation
- Easier testing
- Suitable for enterprise applications