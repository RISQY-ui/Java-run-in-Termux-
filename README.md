# ☕ Complete Java Guide for Termux

---

## 📌 1. Install Java on Termux

```bash
pkg update && pkg upgrade -y
pkg install openjdk-21
```

### Check version:

```bash
java --version
javac --version
```

#### Expected Output

```
openjdk version "21.0.x"
javac 21.0.x
```

✅ **If both commands show version numbers, Java is ready.**

---

## 📝 2. Create Java File with Nano

```bash
nano Main.java
```

### Steps

| Step | Action |
|------|--------|
| 1 | Write your Java code in the editor |
| 2 | Save file | `CTRL + O` → `Enter` |
| 3 | Exit editor | `CTRL + X` |

---

## 🔨 3. Compile Java File

```bash
javac Main.java
```

### Result

| Status | Description |
|--------|-------------|
| ✅ Success | A `Main.class` file will appear |
| ❌ Error | Check code syntax and try again |

---

## 🚀 4. Run the Program

```bash
java Main
```

⚠️ **Important:** Do not use `.class` or `.java` when running — just the class name.

---

## 💻 5. Sample Java Code (For Practice)

### Simple Grade Checker

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter exam score: ");
        int score = input.nextInt();

        if (score >= 75) {
            System.out.println("Passed");
        } else if (score >= 50) {
            System.out.println("Remedial");
        } else {
            System.out.println("Failed");
        }

        input.close();
    }
}
```

### Code Breakdown

| Part | Explanation |
|------|-------------|
| `import java.util.Scanner;` | Import Scanner class for input |
| `Scanner input = new Scanner(System.in);` | Create Scanner object for keyboard input |
| `input.nextInt()` | Read integer from keyboard |
| `if-else` | Check score and print grade |
| `input.close()` | Close Scanner (good practice) |

### Sample Execution

```
Enter exam score: 85
Passed
```

---

## ⚡ 6. Quick Java Workflow

| Command | Function |
|---------|----------|
| `nano Main.java` | Create / edit Java file |
| `javac Main.java` | Compile (to `.class`) |
| `java Main` | Run program |

### Combined Command

```bash
nano Main.java && javac Main.java && java Main
```

---

## ❌ 7. Common Java Errors

| Error | Cause | Solution |
|-------|-------|----------|
| `javac: command not found` | Java not installed | Install openjdk-21 with `pkg install openjdk-21` |
| `class Main is public, should be declared in a file named Main.java` | Class name doesn't match file name | Match file name and class name (case-sensitive) |
| `cannot find symbol` | Typo or missing import | Check code syntax carefully |
| `';' expected` | Missing semicolon | Add `;` at end of statements |
| `Exception in thread "main"` | Runtime error | Debug code logic |

---

## 📊 C++ vs Java Comparison

| Aspect | C++ | Java |
|--------|-----|------|
| **Compile** | `g++ main.cpp -o main` | `javac Main.java` |
| **Run** | `./main` | `java Main` |
| **File Extension** | `.cpp` | `.java` |
| **Compiled Result** | Binary executable file | Bytecode (`.class` file) |
| **Input** | `cin >>` | `Scanner` |
| **Output** | `cout <<` | `System.out.println()` |
| **Case Sensitive** | Yes | Yes |
| **OOP Support** | Yes | Yes (everything is class) |

---

## 🎯 Your First Steps

### Step 1: Install Java

```bash
pkg install openjdk-21
java --version
```

### Step 2: Create & Edit File

```bash
nano Main.java
```

**Paste this code:**

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello from Termux!");
    }
}
```

### Step 3: Compile

```bash
javac Main.java
```

### Step 4: Run

```bash
java Main
```

### Expected Output

```
Hello from Termux!
```

🎉 **Congratulations! Your first Java program works!**

---

## 💡 Key Differences from C++

| Concept | C++ | Java |
|---------|-----|------|
| **Platform** | Native (machine-specific) | JVM (Universal) |
| **Memory** | Manual (`new`, `delete`) | Automatic (Garbage Collector) |
| **Speed** | Faster | Slightly slower (JVM overhead) |
| **Compilation** | Direct to machine code | To bytecode (JVM interprets) |
| **Learning Curve** | Steeper | Gentler |

---

## 📂 File Organization on Termux

```
/data/data/com.termux/files/home/
├── Main.java          (Source code)
├── Main.class         (Compiled bytecode)
└── OtherPrograms/
    ├── Calculator.java
    └── Calculator.class
```

---

## 🔄 Complete Java Workflow Summary

```
1. WRITE   → nano Main.java
             ↓
2. COMPILE → javac Main.java
             ↓ (creates Main.class)
             ↓
3. RUN     → java Main
             ↓
4. OUTPUT  → Result displayed on terminal
```

---

## ✅ Final Checklist

| Item | Status |
|------|--------|
| Java installed | ✅ openjdk-21 |
| Nano editor working | ✅ Can create files |
| javac compiler working | ✅ Can compile `.java` files |
| java runtime working | ✅ Can execute `.class` files |
| Sample code tested | ✅ Runs successfully |
| Error handling documented | ✅ Common issues covered |
| Workflow understood | ✅ Write → Compile → Run |

---

## 🚀 Next Steps for Learning

### Basic Level
- Variables and data types
- Input/Output with Scanner
- Conditional statements (if-else)
- Loops (for, while)

### Intermediate Level
- Arrays and Collections
- Methods and Functions
- Object-Oriented Programming (Classes)
- Exception Handling

### Advanced Level
- Inheritance and Polymorphism
- Interfaces and Abstract Classes
- File I/O Operations
- Multithreading

---

**Last Updated:** June 2026
