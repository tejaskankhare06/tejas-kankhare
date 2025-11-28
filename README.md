Demonstration of Single Inheritance, Method Overriding & Reusability

This project demonstrates the concept of Inheritance in Java, one of the core principles of Object-Oriented Programming (OOP).
Inheritance allows one class (child/subclass) to acquire the properties and methods of another class (parent/superclass), promoting code reuse, maintainability, and polymorphism.

📁 Project Structure
/src
 ├── Animal.java
 ├── Dog.java
 └── InheritanceDemo.java
README.md

📌 Concepts Demonstrated
✔️ 1. Superclass (Parent Class)

A base class containing common properties and methods.

✔️ 2. Subclass (Child Class)

Inherits features from the parent class and can add its own functionalities.

✔️ 3. Method Overriding

The subclass provides its own implementation for a method defined in the parent class.

✔️ 4. Reusability

Common code is written once in the parent class and used by all child classes.

📘 Example Code
Animal.java – Parent Class
public class Animal {
    public void sound() {
        System.out.println("Animal makes a sound");
    }

    public void eat() {
        System.out.println("Animal eats food");
    }
}

Dog.java – Child Class (inherits Animal)
public class Dog extends Animal {

    // Method overriding
    @Override
    public void sound() {
        System.out.println("Dog barks");
    }

    public void fetch() {
        System.out.println("Dog fetches a ball");
    }
}

InheritanceDemo.java – Main Program
public class InheritanceDemo {
    public static void main(String[] args) {

        Dog dog = new Dog();

        dog.sound();   // Calls overridden method
        dog.eat();     // Inherited method
        dog.fetch();   // Dog-specific method
    }
}

▶️ How to Run

Clone or download this repository.

Open a terminal in the project folder.

Compile the Java files:

javac Animal.java Dog.java InheritanceDemo.java


Run the program:

java InheritanceDemo
