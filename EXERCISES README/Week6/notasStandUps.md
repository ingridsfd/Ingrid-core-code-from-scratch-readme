# Sobre Objetos:

Explicación de var "any":
```JavaScript
class User {
  age:number;
  email:string;
  name:string;

  constructor(name:string, age:number, email: string) {
    this.name = name;
    this.age = age;
    this.email = email;
  }

  profile(): void {
    console.log(`\n=======================\nName: ${this.name}\nAge: ${this.age}\nEmail: ${this.email}\n=======================\n`)
  }
}


const edy = new User('Edy', 23, 'edy@gmail.com');

const edy2 = {
  "name": "Edy",
  "age": 23,
  "email": "edy@gmail.com"
}

// edy.profile();

console.log(edy);

console.log(edy2);

// 1. Informacion
// 2. Hash (Java -->> toString)



// any
let x:any = 5;
x = 'Yosef';
x = 60;
```

Segundo ejemplo sobre Profile:
```JavaScript
class User {
  age:number;
  email:string;
  name:string;
  emailAndName: string;
  isLegal: boolean = false;

  constructor(name:string, age:number, email: string) {
    // super
    this.name = name;
    this.age = age;
    this.email = email;
    this.emailAndName = `${this.email} - ${this.name}`;
    if(this.age >= 21) {
      this.isLegal = true;
    }
  }

  profile(): void {
    console.log(`\n=======================\nName: ${this.name}\nAge: ${this.age}\nEmail: ${this.email}\n=======================\n`)
  }
}

const edy = new User('Edy', 23, 'edy@gmail.com');


console.log(edy.isLegal);
```
