# Angular Directives

## *ngIf

Displays or hides an element.

```html
<div *ngIf="isLoggedIn">
  Welcome
</div>
```

---

## *ngFor

Loops through collections.

```html
<li *ngFor="let emp of employees">
  {{emp}}
</li>
```

---

## *ngSwitch

Displays content based on conditions.

```html
<div [ngSwitch]="role">

<div *ngSwitchCase="'Admin'">
Admin Dashboard
</div>

<div *ngSwitchDefault>
User Dashboard
</div>

</div>
```

---

## ngClass

Adds CSS classes dynamically.

```html
<div [ngClass]="{'active': isActive}">
Angular
</div>
```

---

## ngStyle

Applies styles dynamically.

```html
<div [ngStyle]="{'color':'blue'}">
Angular
</div>
```

---

## ngModel

Two-way data binding.

```html
<input [(ngModel)]="username">
```

---

## Custom Directive

```bash
ng generate directive highlight
```