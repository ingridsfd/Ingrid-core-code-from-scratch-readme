# Week challenges (Monday) 💻

Work on your project

# Week challenges (Tuesday) 💻

Work on your project

# Week challenges (Wednesday) 💻

Work on your project

# Week challenges (Thursday) 💻

1. [x] Check [S.O.L.I.D](https://www.youtube.com/watch?v=2X50sKeBAcQ) video

Tech branch to remember the name of 5 principles in programming:

1. Single Responsibility (Responsabilidad Única)

Be in charge of 1 part of the system exclusively.
Example: the class that creates the password of a user in a Website.

All classes have their own responsibility. This is encapsulation.
Don't let a class do all the job. Make a class for each function (can be the same one or different).

2. Open Closed (abierta - cerrado)

When the class is open to modification through polymorphism which looks like tis:

![image](https://user-images.githubusercontent.com/98929413/194915979-037c009e-fb77-48e6-b3ca-31f3ca7d538c.png)
![image](https://user-images.githubusercontent.com/98929413/194916096-7a5ac4f3-f323-48d5-869e-2652d9ff1f06.png)

Function is protected.
Write new code but doesn't have to change constantly.

However, we do this with heritance and polymorphism.

3. Liskov Substitution (Sustitución de Liskov)

Toda clase que debe ser hija de otra clase, debe utilizarse como si fuera el mismo padre. Tiene que ser individual.

In the end, we go to the same principle. There should be one function for individual classes. Use instances!

4. Interface Segregation

Tener una clase gigante que defina todas las funciones, it's not okay. That's why we would rather use interfaces.

5. Dependency Inversion

Abstraction: abstract layers. The communication among components is through interfaces. The individuality of the components allows to make changes without changing the system design. 

2. [x] Check another [S.O.L.I.D](https://www.youtube.com/watch?v=XzdhzyAukMM) video

1. Single Responsibility:

There's only one reason to change the design of the project, always remembering one thing is always in charge of only one.
And when change is necessary.

2. Open Closed:

Software entities should be open for extension but closed for modiciation.

3. Liskov Substitution principle:

Derived objects can be substited with their own functions and targets.

4. Interface Segregation Principle: 

Do interfaces so you don't have to build messed classes.

5. Dependency Inversion Principle:

Fathers should not depend on daugther classes, but depend on abstractions.
Details should not depend of abstractions.
