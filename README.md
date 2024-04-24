# OOP pricniples with examples in TS

**Object-oriented programming** is a programming paradigm based on **classes** and **objects** rather than functions and logic. The software programs in object-oriented programming are structured into reusable pieces of code known as classes.

Although TypeScript is a superset of JavaScript, object-oriented programming in TypeScript differs from Object-oriented programming in JavaScript because, unlike JavaScript, TypeScript has full class support, has access modifiers, and type annotations like most object-oriented programming languages.

The primary principles of OOP include:

1. Inheritance
2. Encapsulation
3. Polymorphism
4. Abstraction

## What is the class and obeject?

**A class** is a blueprint for creating objects. It defines the structure and behavior of objects that will be instantiated based on the class. A class in TypeScript contains properties (also known as fields or attributes) and methods (functions associated with the class). It encapsulates the data and operations that are related to a particular concept or entity.

Here's the basic syntax for creating a class in TypeScript:
```
class ClassName {
  // Properties (attributes)
  propertyName1: type;
  propertyName2: type;

  // Constructor
  constructor(parameter1: type, parameter2: type) {
    this.propertyName1 = parameter1;
    this.propertyName2 = parameter2;
  }

  // Methods
  methodName1() {
    // Method implementation
  }

  methodName2() {
    // Method implementation
  }
}
```
Let's create a simple class in TypeScript representing a basic car:

```
class Car {
  // Properties
  make: string;
  model: string;
  year: number;

  // Constructor
  constructor(make: string, model: string, year: number) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  // Method
  start() {
    console.log(`Starting the ${this.make} ${this.model}.`);
  }
}

```
Now, an object is an instance of a class. Once you have defined a class, you can create objects based on that class blueprint. Objects represent specific instances of the entity described by the class. Each object has its own set of properties and can invoke methods defined in the class.

Here's how you create an object based on the Car class we defined earlier:
```
const myCar = new Car("Toyota", "Camry", 2022);
const anotherCar = new Car("Honda", "Accord", 2023);

myCar.start(); // Output: "Starting the Toyota Camry."
anotherCar.start(); // Output: "Starting the Honda Accord."

```
In this example, we created two separate instances of the Car class, myCar and anotherCar, each with its own set of properties (make, model, and year) and the ability to call the start method.

Using classes and objects in TypeScript allows you to structure your code more efficiently, promote code reuse through inheritance, and take advantage of object-oriented programming principles.
