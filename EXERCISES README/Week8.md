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
2. [x] Develop typed functions by using TypeScript guided exercise, using Typescript

This module consisted of understanding and practicing
* Default values
* Expressions
* Optional values
* Required values

4. [x] Read Abstract Classes

Type 1: To add the properties as such. En este, la propiedad tiene que asignarse despues a la clase que se extiende también.

Type 2: The use of 'super()' to initialize it.

5. [x] Watch Abstract Classes vs Interfaces video

La diferencia entre clases abstractas e interfaces: The main difference is what they mean semantically.
Abstract classes generalize behavior. From the general to the particular.
Interfaces standarize behavior... so we do not break existing implementations.
Question to considerate: What happens if two parents have the same behavior but we want to extend or implement, which will it have?

---
* la clase abstracta puede ser extendida solo una vez y es padre-hija, siempre
* compartir comportamientos, para generalizar comportamientos
* Extender la funcionalidad general que está en la clase
* extender comportamientos generales
* ya no se pueden tener padres abstractos
* por esto se prefieren las interfaces
* solo se puede tener 1 solo padre, sea abstracto o no
---
* las interfaces se pueden implementar muchas

* definir comportamientos UNICAMENTE no da extents

* Patrón a seguir
---
* clase generica: para definir clases de tipos. revisar que los tipos de variables corran bien durante el programa
* podemos enviar tipos a la clase
* Instance: When data is assigned and called along the object.

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

var a1 = ["live", "strong", "lyal", "lysh", "arp"]
var a2:string[] = ["lively", "alive", "harp", "sharp", "armstrong"]
//   r = ["live", "strong", "arp"] ==> ["arp","live", "strong" ]


console.log(inArray(a1, a2));
```

# Week challenges (Thursday) 💻
9. [x] Define generics in TypeScript guided exercise, using Typescript
10. [ ] Generics exercise, using Typescript
11. [ ] Upload resume
