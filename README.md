# ☕ Complete Java Guide for Termux

---

📌 1. Install Java on Termux

```bash
pkg update && pkg upgrade -y
pkg install openjdk-21
```

Check version:

```bash
java --version
javac --version
```

---

📝 2. Create Java File with Nano

```bash
nano Main.java
```

Write your Java code.
Save: CTRL+O → Enter → CTRL+X to exit.

---

🔨 3. Compile Java File

```bash
javac Main.java
```

If successful, a Main.class file will appear.

---

🚀 4. Run the Program

```bash
java Main
```

Note: Do not use .class or .java when running.

---

💻 5. Sample Java Code (For Practice)

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

---

⚡ 6. Quick Java Workflow

Command Function
nano Main.java Create / edit Java file
javac Main.java Compile (to .class)
java Main Run program

---

❌ 7. Common Java Errors

Error Cause Solution
javac: command not found Java not installed Install openjdk-21
class Main is public, should be declared in a file named Main.java Class name doesn't match file name Match file name and class name
cannot find symbol Typo or missing import Check code syntax

---

📊 C++ vs Java Comparison

Aspect C++ Java
Compile clang++ main.cpp -o main javac Main.java
Run ./main java Main
Extension .cpp .java
Compile Result Binary file main Bytecode file Main.class
Input cin >> Scanner
Output cout << System.out.println()
