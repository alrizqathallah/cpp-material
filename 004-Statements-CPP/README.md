# Statements dalam C++

## 1. Pengantar Pernyataan (Statements) dalam C++

**Statements** dalam C++ adalah elemen terkecil yang berdiri sendiri dan digunakan untuk menyampaikan instruksi atau tindakan kepada komputer.

**Statements** adalah instruksi lengkap yang diakhiri dengan titik kome ; (semicolon).

## 2. Jenis-Jenis Statements dalam C++

### 2.1 Expression Statements

Expression Statements melakukan operasi seperti pengisian nilai ke variabel (assignment) atau pemanggilan fungsi, dan selalu diakhiri dengan titik koma.

**Sintaks**:

```
expression;
```

**Contoh**:

```
int x = 5;        // Statement assignment
std::cout << x;   // Statement function call
```

### 2.2 Compound Statements

Pernyataan gabungan adalah kumpulan beberapa pernyataan yang dikelompokkan menggunakan tanda kurung kurawal {} dan diperlakukan sebagai satu unit.

**Sintaks**:

```
{
  statement1;
  statement2;
}
```

**Contoh**:

```
{
  int x = 10;
  int y = 20;

  std::cout << x + y;
}
```

### 2.3 Control Flow Statements

Statement ini digunakan untuk mengendalikan alur seleksi program.

**Selection Statements**

- Digunakan untuk membuat keputusan.

- Contoh: `if`, `if-else`, `switch`.

**Contoh**:

```
if (x > 0) {
  std::cout << "Positif";
} else {
  std::cout << "Negatif";
}
```

**Iteration Statements**

- Digunakan untuk melakukan perulangan.

- Contoh: `for`, `while`, `do-wile`.

**Contoh (`for`)**:

```
for (int i = 0; i < 5; i++) {
  std::cout << i << " ";
}
```

**Jump Statements**

- Digunakan untuk mengubah alur eksekusi normal.

- Contoh `break`, `continue`, `return`, `goto`.

**Contoh (`break` dan `continue`)**

```
for (int i = 0; i < 5; i++) {
  if (i == 3) break;
  if (i == 1) continue;
  std::cout << 1 << " ";
}
```

## 3. Menggabungkan Banyak Statements

Sebuah program biasanya terdiri dari banyak statements yang bekerja bersama.

Sehigga dapat menggabungkan:

- **Declaration Statements**: Untuk mendeklarasikan variabel atau konstanta.
- **Expression Statements**: Untuk mengisi atau melakuakn operasi
- **Control Flow Statements**: Untuk membuat keputusan atau melakukan perulangan.

**Contoh Penggunaan**:

```
#include <iostream>

int main() {
  // Declaration Statements
  int sum = 0;

  // Iteration Statements
  for (int i = 1; i <= 10; i++) {
    sum += i; // Expression Statements
  }

  //Decision Statements/Control Flow
  if (sum > 50) {
    std::cout << "Jumlah lebih besar dari 50: " << sum << std::endl;
  } else {
    std::cout << "Jumlah kurang dari atau sma dengan 50: " << sum << std::endl;
  }

  return 0; // Return Statements
}
```

**Hasil Output**:

```
Jumlah lebih besar dari 50: 55
```

## 4. Contoh dengan Penjelasan

**Contoh 1: Kalkulator Sederhana**

```
#include <iostream>

int main() {
  int a, b;
  char op;

  //Input Statements
  std::cout << "Masukan angka pertama: ";
  std::cin >> a;

  std::cout << "Masukan operator (+, -, *, /): ";
  std::cin >> op;

  std::cout << "Masukan angka kedua: ";
  std::cin >> b;

  //Control Flow dan Operation Statements
  if (op == '+') {
    std::cout << "Hasil: " << a + b << std::endl;
  } else if (op == '-') {
    std::cout << "Hasil: " << a - b << std::endl;
  } else if (op == '*') {
    std::cout << "Hasil: " << a * b << std::endl;
  } else if (op == '/') {
    if (b != 0) {
      std::cout << "Hasil: " << a / b << std::endl;
    } else {
      std::cout << "Pembagian dengan nol tidak diperbolehkan." << std::endl;
    }
  } else {
    std::cout << "Operator tidak valid!" << std::endl;
  }

  return 0;
}
```

## 5. Best Practice

- Selalu akhiri pernyataan dengan titik koma (semicolon).
- Gunakan komentar untuk menjelaskan pernyataan yang kompleks.
- Kelompokkan pernyataan terkait dalam blok {} untuk meningkatkan keterbacaan.
- Hindari penggunaan `goto` secara berlebihan karena dapat membuat kode sulit dibaca dan debug.

Dengan memahami jenis-jenis pernyataan dan cara kerjanya, akan dapat menulis program C++ yang efisien dan terstruktur dengan baik.
