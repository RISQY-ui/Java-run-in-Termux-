# Java-run-in-Termux-

# ☕ RANGKUMAN LENGKAP JAVA DI TERMUX

1. Install Java di Termux

```bash
pkg update && pkg upgrade -y
pkg install openjdk-21
```

Cek versi:

```bash
java --version
javac --version
```

---

# 2. Membuat File Java dengan Nano

```bash
nano Main.java
```

Tulis kode Java-nya.
Simpan: CTRL+O → Enter → CTRL+X keluar.

---

# 3. Compile File Java

```bash
javac Main.java
```

Jika berhasil, muncul file Main.class.

---

# 4. Menjalankan Program

```bash
java Main
```

Catatan: Jangan pakai .class atau .java saat menjalankan.

---

# 5. Contoh Kode Java (Buat Latihan)

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan nilai ujian: ");
        int nilai = input.nextInt();

        if (nilai >= 75) {
            System.out.println("Lulus");
        } else if (nilai >= 50) {
            System.out.println("Remedial");
        } else {
            System.out.println("Tidak Lulus");
        }

        input.close();
    }
}
```

---

# 6. Alur Cepat Java

Perintah Fungsi
nano Main.java Buat / edit file Java
javac Main.java Kompilasi (jadikan .class)
java Main Jalankan program

---

# 7. Kesalahan Umum Java

Error Penyebab Solusi
javac: command not found Java belum terinstall Install openjdk-21
class Main is public, should be declared in a file named Main.java Nama class != nama file Samakan nama file dan class
cannot find symbol Typo atau lupa import Cek penulisan kode

---
```

📊 Perbandingan C++ vs Java

Aspek C++ Java
Compile clang++ main.cpp -o main javac Main.java
Run ./main java Main
Ekstensi .cpp .java
Hasil compile File biner main File bytecode Main.class
Input cin >> Scanner
Output cout << System.out.println()


