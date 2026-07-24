# Angular HttpClient

## Import HttpClientModule

```typescript
import { HttpClientModule } from '@angular/common/http';
```

Add it to the application imports.

---

## Inject HttpClient

```typescript
constructor(private http: HttpClient) {}
```

---

## GET Request

```typescript
this.http.get('https://api.example.com/users');
```

---

## POST Request

```typescript
this.http.post('https://api.example.com/users', user);
```

---

## PUT Request

```typescript
this.http.put('https://api.example.com/users/1', user);
```

---

## DELETE Request

```typescript
this.http.delete('https://api.example.com/users/1');
```

---

## Using Observables

```typescript
this.http.get(url).subscribe(data => {
  console.log(data);
});
```

---

## Using Promises

```typescript
const data = await firstValueFrom(
  this.http.get(url)
);
```