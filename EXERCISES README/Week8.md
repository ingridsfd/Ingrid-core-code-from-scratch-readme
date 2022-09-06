# Week challenges (Monday) 💻
1. [x] Watch Object-Oriented Programming - Resume video
* Procedural programming: program divided in a set of functions.
* Too much interdependence functions is not good in programming. Object Oriented Programming solves this.
* Units are objects. Variables, properties. Functions are methods.
* Encapsulation: Is where everything is grouped.The variables and functions. Reduce complexity and re-use code.
* Objects with no parameters, are better.
* Abstraction: Hide the complex. Show the essentials.
* Inheritance: Avoid redundant code.
* Polymorphism: Refactor "ugly" switch/case statements.
# Week challenges (Tuesday) 💻
2. [ ] Develop typed functions by using TypeScript guided exercise, using Typescript
3. [x] Read Abstract Classes

Type 1: To add the properties as such. En este, la propiedad tiene que asignarse despues a la clase que se extiende también.

Type 2: The use of 'super()' to initialize it.

5. [x] Watch Abstract Classes vs Interfaces video

La diferencia entre clases abstractas e interfaces: The main difference is what they mean semantically.
Abstract classes generalize behavior. From the general to the particular.
Interfaces standarize behavior... so we do not break existing implementations.
Question to considerate: What happens if two parents have the same behavior but we want to extend or implement, which will it have?

# Week challenges (Wednesday) 💻
5. [ ] Make the Deadfish Swim exercise, using Typescript
6. [ ] Duplicate Encoder exercise, using Typescript
7. [ ] Find The Odd Int exercise, using Typescript
8. [x] Which Are In? exercise, using Typescript
```JavaScript
export function inArray(a1: string[], a2: string[]): string[] {
  
  // 0. Quitar repetidos de a1
  // 1. Recorrer a1
  // 1.1 Mientras recorro a1, filtro los elementos de a1
  // 1.1.1 Filtrar:
  // 1.1.1.1 Se quedan los elementos que son un substring de un string en a2
  // 1.1.2 sort sobre arreglo filtrado
  // 1.1.3 return de arreglo filtrado
  
  return [... new Set(a1)].filter((subStr:string) => {
    let result = a2.find((str:string) => str.includes(subStr));
    return result !== undefined;
  }).sort();
  
}
```

# Week challenges (Thursday) 💻
9. [ ] Define generics in TypeScript guided exercise, using Typescript
10. [ ] Generics exercise, using Typescript
11. [ ] Upload resume
