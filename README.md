"Three repositories: Write Java, Build Projects, Transform the Tech World!" ~('in Galadiel voice')

 "Here's the Java cheat sheet, your guiding light in the midst of coding challenges in the darkest of times. When there's no light except the white font colors of your code and the output full of erorrs"

```java
// Hello World Program
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!"); // Output: Hello, World!
    }
}
```

```java
// Comments
// This is a single-line comment

/*
This is a
multi-line
comment
*/
```

```java
// Variables and Data Types
int age = 25;
double salary = 5000.50;
char grade = 'A';
boolean isEmployed = true;
String name = "John Doe";

final double PI = 3.14;

int num = (int) 3.14;
```

```java
// Operators
int sum = 10 + 5; // 15
int difference = 10 - 5; // 5
int product = 10 * 5; // 50
int quotient = 10 / 5; // 2
int remainder = 10 % 5; // 0

int x = 10;
x += 5; // x = 15
x -= 5; // x = 10
x *= 5; // x = 50
x /= 5; // x = 10
x %= 5; // x = 0

boolean isEqual = (5 == 5); // true
boolean isNotEqual = (5 != 10); // true
boolean isGreater = (10 > 5); // true
boolean isLess = (5 < 10); // true
boolean isGreaterOrEqual = (10 >= 10); // true
boolean isLessOrEqual = (5 <= 10); // true

boolean result1 = true && false; // false
boolean result2 = true || false; // true
boolean result3 = !true; // false
```

```java
// Control Flow
int number = 10;
if (number > 0) {
    System.out.println("Positive"); // Output: Positive
} else if (number < 0) {
    System.out.println("Negative");
} else {
    System.out.println("Zero");
}

int day = 3;
switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday"); // Output: Wednesday
        break;
    default:
        System.out.println("Invalid day");
}

for (int i = 1; i <= 5; i++) {
    System.out.println(i); // Output: 1, 2, 3, 4, 5
}

int i = 1;
while (i <= 5) {
    System.out.println(i); // Output: 1, 2, 3, 4, 5
    i++;
}

int i = 1;
do {
    System.out.println(i); // Output: 1, 2, 3, 4, 5
    i++;
} while (i <= 5);

for (int i = 1; i <= 10; i++) {
    if (i == 5) {
        break; // exit the loop
    }
    if (i == 3) {
        continue; // skip current iteration
    }
    System.out.println(i); // Output: 1, 2, 4
}
```

```java
// Classes and Objects
public class Person {
    String name;
    int age;

    public Person(String name, int age) {
        this.name =

 name;
        this.age = age;
    }

    public void sayHello() {
        System.out.println("Hello, my name is " + name);
    }
}

Person person = new Person("John", 25);
person.sayHello(); // Output: Hello, my name is John
```

```java
// Inheritance
public class Animal {
    public void eat() {
        System.out.println("Eating...");
    }
}

public class Dog extends Animal {
    public void bark() {
        System.out.println("Barking...");
    }
}

Dog dog = new Dog();
dog.eat(); // Output: Eating...
dog.bark(); // Output: Barking...
```

```java
// Polymorphism
public class Animal {
    public void makeSound() {
        System.out.println("Animal is making a sound");
    }
}

public class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}

Animal animal = new Animal();
animal.makeSound(); // Output: Animal is making a sound

Animal dog = new Dog();
dog.makeSound(); // Output: Dog is barking
```

```java
// Encapsulation
public class Person {
    private String name;
    private int age;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}

Person person = new Person();
person.setName("John");
person.setAge(25);
String name = person.getName(); // John
int age = person.getAge(); // 25
```

```java
// Abstraction
public abstract class Animal {
    public abstract void makeSound();
}

public class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}

Animal dog = new Dog();
dog.makeSound(); // Output: Dog is barking
```

```java
// Interfaces
public interface Drawable {
    void draw();
}

public class Circle implements Drawable {
    @Override
    public void draw() {
        System.out.println("Drawing a circle");
    }
}

Drawable circle = new Circle();
circle.draw(); // Output: Drawing a circle
```

```java
// Exception Handling
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Division by zero error"); // Output: Division by zero error
} finally {
    System.out.println("Finally block"); // Output: Finally block
}
```

```java
// File Handling
import java.io.*;

public class FileExample {
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("file.txt");
            writer.write("Hello, World!");
            writer.close();

            FileReader reader = new FileReader("file.txt");
            int character;
            while ((character = reader.read()) != -1) {
                System.out.print((char) character); // Output: Hello, World!
            }
            reader.close();
        } catch (IOException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }
    }
}
```
