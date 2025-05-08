## 5. What is type inference in TypeScript? Why is it helpful?

Type inference in TypeScript automatically determines the type of a variable based on its value. Don't need to explicitly declare types. It helps reduce code duplication and makes the code cleaner and easier to maintain while providing type safety.

### Example
```typescript
let num = 5;  // TypeScript infers num as 'number'
num = "Hello"; // Error: Type 'string' is not assignable to type 'number'

let message = "Hello";  // TypeScript infers message as 'string'



## 6.How does TypeScript help in improving code quality and project maintainability?

TypeScript helps improve code quality by adding static typing, which catches errors early during development. It provides clear types for variables, functions, and objects, making the code more predictable. Features like interfaces and enums improve code structure and clarity. TypeScript’s integration with modern IDEs also offers autocompletion and error checking, making the code easier to read, debug, and maintain over time.

### Example
```typescript
// Static typing
let userName: string = "John";  // Error if changed to non-string value

// Interfaces for better structure
interface Person {
  name: string;
  age: number;
}

const person: Person = { name: "Alice", age: 30 };

// Enums for clarity
enum Role {
  Admin = "ADMIN",
  User = "USER"
}

const userRole: Role = Role.Admin;  // Type safety ensured