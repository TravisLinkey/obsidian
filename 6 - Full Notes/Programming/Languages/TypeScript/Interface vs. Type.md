
2024-07-27 08:41

Tags: [[TypeScript]]

### Why use [[Interface]] over [[Type]]

1. Extendability
Interfaces are designed to be extended. This is useful when creating resuable and extendable structures.

2. Declaration Merging
If you define the same interface multiple times, [[TypeScript]] will merge their properties.

```typescript
interface Person {
    name: string;
}

interface Person {
    age: number;
}

const person: Person = {
    name: "Alice",
    age: 30;
}
```

### Why use [[Type]] over [[Interface]]

1. Type Alias Capabilities
Type aliases can define unions, intersections, and other complex types that interfaces cannot.

```typescript
type ID = string | number;
```

Interfaces can only describe the object shapes, but thyey can be extended and merged, which `type` cannot do in the same way.


### References
- [[Type]]
- [[Interface]]

