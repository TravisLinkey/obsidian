
2024-07-27 08:44

Tags: [[TypeScript]]

### Syntax
```typescript
interface User = {
    id: string;
    name: string;
    age: number;
}

let user: User = {
    id: "1",
    name: "Alice",
    age: 21
}

```

### Extending Interfaces
```typescript
interface Name {
    firstName: string;
    lastName: string;
}

interface Contact extends Name {
    email: string;
    phone: string;
}
```


### References
- [[Interface vs. Type]]

