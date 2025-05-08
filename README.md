## Provide an example of using union and intersection types in TypeScript

##### Union Type

Union Types means there can be several type of variable type. If one type match then it will be ok
Example

```
let id: string | number = "123";
id = 123; // No error
```

In this example, the id accepts either a string or number.

##### Intersection Type

An intersection type combines multiple types into one. A variable of an intersection type will need to satisfy all the types combined.

- Example

```
type Person = { name: string };
type Employee = { employeeId: number };
let employee: Person & Employee = { name: "Alice", employeeId: 123 };
```

---

### What is type inference in TypeScript? Why is it helpful?

**Type Inference** is a powerful feature in TypeScript where the compiler **automatically infers the type** of a variable based on its assigned value — without needing an explicit type annotation.

- Example

```typescript
let name = "Alice"; // inferred as string
let age = 25; // inferred as number
```
---
### 