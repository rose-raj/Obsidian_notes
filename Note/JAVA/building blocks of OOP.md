[[Unit 1.5]]

#### *Inheritance* 
*When an object accusers the properties of a parent class and behaviors of a parent object is known as Inheritance*
*It uses parent child relation A class which inherits the behaviors and properties of an other class is called the ==child class==  and the other class is called ==Parent class==*
*it improves the re-usability*
#### *Encapsulation*
*It is the process of binding together code , data and variables in a class into a single unit to prevent further modification and to hide your data*
**Steps to Encapsulation**
1. Declaring variables of a  class as private 
2. Providing the public ==stter== and ==getter== methods to modify and view the variable values.
#### *Abstraction*
*It is the process of hiding the Implementations and details and showing only the functionality to the user*
**Steps to Abstraction**
1. Abstract class 
2. Interface
#### *Polymorphism*

*It  is the  ability of the object to take multiple forms so that 2 methods with same name behaves differently based on which object called the method (deto)*
```
The power swicth in a remote that turn on and trun of a device 
```
##### Compile time Polymorphism or method Overloading
*multiple methods with same name but behaves differently based on the parameters*
```
class MathUtils {
    int add(int a, int b) {
        return a + b;
    }

    int add(int a, int b, int c) { // Same method name, different parameters
        return a + b + c;
    }
}
```
##### Runtime Polymorphism or method overriding
*A child class can change the behavior of a method from the parent class*
```
class Animal {
    void sound() {
        System.out.println("Animals make sounds");
    }
}

class Dog extends Animal {
    @Override
    void sound() { 
        System.out.println("Dog barks");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myPet = new Dog(); 
        myPet.sound(); 
    }
}

```