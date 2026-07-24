# Angular Routing

## Enable Routing

```bash
ng new my-app --routing
```

---

## Route Configuration

```typescript
const routes: Routes = [
  {
    path: '',
    component: HomeComponent
  },
  {
    path: 'about',
    component: AboutComponent
  }
];
```

---

## Router Outlet

```html
<router-outlet></router-outlet>
```

---

## Navigation Link

```html
<a routerLink="/about">About</a>
```

---

## Route Parameters

```typescript
this.route.snapshot.paramMap.get('id');
```

Example URL

```
/employee/101
```

---

## Query Parameters

Example URL

```
/products?id=10&category=laptop
```

```typescript
this.route.snapshot.queryParams['id'];
```

---

## Passing Data

```typescript
this.router.navigate(
['employee',101]
);
```