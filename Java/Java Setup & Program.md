## 🔗 Links

1. [[#⚙️ Download JDK & How to Compile and Run Java Programs|Download JDK + Compile & Run Instructions]]
2. [[#1. Hello World|Hello World]]
3. [[#2. Room Area Demo|Room Area Demo]]

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
