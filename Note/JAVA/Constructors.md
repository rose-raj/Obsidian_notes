[[Unit 1.5]]

*A constructor is a special method in java used to initialize objects IT runs automatically  when an object of a class is created*
- same name as the class
- no return type
- Automatically called when an object is created 
- Constructor cannot be 
  `abstract` *they are not inherited so no overloading*
  `static` *They belong to object not the class *
  `final`  they cant be overridden
  `synchronized` *Each Objects has its own constructors so no need for synchronized*
```
class Car {
    String brand;

    
    Car(String b) {
        brand = b;
        System.out.println("Car brand is: " + brand);
    }

    public static void main(String[] args) {
        Car myCar = new Car("Toyota");
    }
}
```
Same code with out `Constructors`
```
class Car {
    String brand; 
    public static void main(String[] args) {
        Car myCar = new Car();  
        myCar.brand = "Toyota"; // Manually set the brand
        System.out.println("Car brand is: " + myCar.brand);
    }
}

```
#### Default Constructor (no parameters)
If no constructor are defined java provides a default one
#### Parameterized Constructor (with parameters)
Used to assign values while creating an object

