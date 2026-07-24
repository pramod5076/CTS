# Angular Router Guards

Router Guards protect routes before navigation.

---

## CanActivate

Controls access to a route.

```typescript
canActivate(): boolean
{
   return true;
}
```

---

## CanDeactivate

Prevents leaving a page with unsaved changes.

```typescript
canDeactivate()
```

---

## Resolve

Loads required data before the component is displayed.

```typescript
resolve()
```

---

## Register Guard

```typescript
{
 path:'admin',

 component:AdminComponent,

 canActivate:[AuthGuard]
}
```

---

## Router Events

Useful Events

- NavigationStart
- NavigationEnd
- NavigationCancel
- NavigationError

---

## Navigation Lifecycle

NavigationStart

↓

RoutesRecognized

↓

GuardsCheck

↓

Resolve

↓

NavigationEnd