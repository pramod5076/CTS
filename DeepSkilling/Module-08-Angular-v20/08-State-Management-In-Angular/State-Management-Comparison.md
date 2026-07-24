# State Management Comparison

## Data Flow Using Services

Component A

↓

Service

↓

Component B

---

## Data Flow Using NgRx

Component

↓

Action

↓

Reducer

↓

Store

↓

Selector

↓

Component

---

## Services vs NgRx

| Feature | Services | NgRx |
|---------|----------|------|
| Learning Curve | Easy | Moderate |
| Boilerplate | Low | High |
| Best For | Small & Medium Apps | Large Enterprise Apps |
| Shared State | Yes | Yes |
| Predictable Updates | Limited | Excellent |
| Debugging | Moderate | Excellent |

---

## When to Use Services

- Small projects
- Few shared components
- Simple state management

---

## When to Use NgRx

- Large enterprise applications
- Complex state
- Multiple API calls
- Advanced debugging
- Large development teams