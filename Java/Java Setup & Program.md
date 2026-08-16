## 🔗 Links

1. [[#⚙️ Download JDK & How to Compile and Run Java Programs|Download JDK + Compile & Run Instructions]]
2. [[#1. Hello World|Hello World]]
3. [[#2. Room Area Demo|Room Area Demo]]
4. [[#3. Room Area from Input|Room Area from Input]]
5. [[#4. User Input|User Input]]

---

## ⚙️ Download JDK & How to Compile and Run Java Programs

### Download JDK

- **Oracle JDK:** [https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/)
- **Alternative (OpenJDK):** [https://jdk.java.net/](https://jdk.java.net/)
- **Adoptium (Eclipse Temurin JDK):** [https://adoptium.net/](https://adoptium.net/)

### Compile & Run Steps

1. **Install JDK** using one of the links above, then **open your terminal** (Command Prompt on Windows, or Terminal on Mac/Linux) and verify installation:

```bash
java -version
javac -version
```

2. **Write your program** in a file named exactly like the public class, e.g. `HelloWorld.java`.

3.  **Compile** the program:

```bash
javac HelloWorld.java
```

This creates a `HelloWorld.class` file (bytecode).

4. **Run** the compiled program:

```bash
java HelloWorld
```


---
## 1. Hello World

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

---
## 2. Room Area Demo

```java
// Room class - stores room data
class Room {
    float length, breadth;

    void setDimension(float length, float breadth){
        this.length = length;
        this.breadth = breadth;
    }
}

// Main class - calculates area
class RoomAreaDemo {
    public static void main(String args[]){
        Room room = new Room();
        room.setDimension(10.5f, 10.6f);

        float area = room.length * room.breadth;
        System.out.println("Area is: " + area);
    }
}
```

---
## 3. Room Area from Input

```java
// Room class - stores room data
class RoomData{
    float length, breadth;

    void setDimension(float length, float breadth){
        this.length = length;
        this.breadth = breadth;
    }
}

// Main class - takes input from command line
class RoomAreaProp{
    public static void main(String args[]){

        if(args.length < 2){
            System.out.println("❌ Please provide 2 values!");
            System.out.println("Usage: java RoomAreaFromInput 10.5 10.6");
            return;
        }

        // ✅ Parse command line arguments to float
        float length = Float.parseFloat(args[0])
        float breadth = Float.parseFloat(args[1])

        // Object created here!
        RoomData room = new RoomData();
        room.setDimension(length, breadth);

        float area = room.length * room.breadth;
        System.out.println("Room Area is: " + area);

    }

}
```

---
## 4. User Input

```java
import java.util.Scanner;

class UserInputDemo {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        // ✅ Reading Integer
        System.out.print("Enter an Integer value : ");
        int age = scanner.nextInt();
        System.out.println("Integer is = " + age);

        // ✅ Reading Double
        System.out.print("Enter a Double value : ");
        double salary = scanner.nextDouble();
        System.out.println("Double is = " + salary);

        scanner.nextLine(); // ✅ Fix: Consume leftover newline after nextDouble()

        // ✅ Reading String
        System.out.print("Enter your Name : ");
        String fullName = scanner.nextLine();
        System.out.println("Name is = " + fullName);

        scanner.close(); // ✅ Good practice: Always close scanner
    }
}
```

---

