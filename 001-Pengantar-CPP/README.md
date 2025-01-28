# Pengantar C++

## 1. Apa itu C++?

C++ adalah **bahasa pemrograman tingkat tinggi dan serbaguna** yang dikembangkan oleh **Bjarne Stroustrup** pada tahun 1983 sebagai pengembangan dari bahasa pemrograman C.

C++ sering disebut sebagai "C dengan Kelas" karena menambahkan fitur **pemrograman berorientasi objek (Object-Oriented Programming/OOP)** pada kemampuan prosedural yang dimiliki oleh C.

### Karakteristik Utama

1. **Multi-Paradigma**: Mendukung pemrograman prosedural, berorientasi objek, dan generik.

2. **Bahasa Terkompilasi**: Membutuhkan compiler seperti GCC atau MSVC untuk mengonversi kode sumber menjadi kode mesin.

3. **Platform-Independent**: Kode dapat ditulis di satu platform dan dijalankan di platform lain dengan sedikit perubahan (jika didukung oleh compiler).

4. **Berorientasi Performa**: Menggabungkan kecepatan dan kontrol memori tingkat rendah dari C dengan abastraksi tingkat tinggi.

### Penggunaan Umum

- Sistem perangkat lunak (misalnya, sistem operasi).
- Game development
- Embedded System
- Aplikasi GUI
- Aplikasi yang membutuhkan performa tinggi (Contoh: sistem keuangan, simulasi perangkat lunak).

## 2. Mengapa Menggunakan C++?

### Keuntungan C++

1. **Pemrograman Berorientasi Objek (OOP)**:
   - Mendukung prinsip utama seperti **encapsulation**, **inheritance**, dan **polymorphism**, yang membuat kode lebih modular dan dapat digunakan kembali.
2. **Performa Tinggi**:
   - Menyediakan kontrol memori tingkat rendah dengan menggunakan **pointer** dan **manajemen memori manual**.
   - Ideal untuk lingkungan dengan ketebatasan sumber daya.
3. **Library Standar yang Kaya**:
   - Menyediakan berbagai library seperti **Standard Template Library (STL)** untuk struktur data dan algoritma.
4. **Kompatibilitas Antar-Platform**:
   - Tulis sekali, kompilasi di mana saja dengan sedikit perubahan.
5. **Kompatibilitas dengan C**:
   - Dapat menggunakan libarary C yang sudah ada tanpa hambatan, sehingga cocok untuk pemrograman sistem.
6. **Digunakan Secara Luas di Industri**:
   - Penting di bidang seperti pengembangan game, embedded system dan system programming.

### Kekurangan

- Sintaks lebih kompleks dibandingkan bahasa tingkat tinggi modern seperti Python.
- Manajemen memori manual dapat menyebabkan kebocoran memori.

## 3. Perbedaan Antara C dan C++

1. **Paradigma**:
   - C : Prosedural
   - C++ : Prosedural + OOP
2. **Rilis**:
   - C : 1972, oleh Dennis Ritchie
   - C++ : 1983, oleh Bjarne Stroustrup
3. **Fokus**
   - C : Berorientasi fungsi
   - C++ : Beriorientasi objek
4. **Kelas dan Objek**:
   - C : Tidak didukung
   - C++ : Didukung
5. **Library Standar**:
   - C : Terbatas (Contoh: stdio.h)
   - C++ : Luas (STL: algoritma, kontainer)
6. **Manajemen Memori**:
   - C : Manual
   - C++ : Manual + Pointer Pintar (otomatis)
7. **Enkapsulasi**:
   - C : Tidak tersedia
   - C++ : Tersedia
8. **Pewarisan**:
   - C : Tidak Tersedia
   - C++ : Didukung
9. **Ekstensi File**:
   - C : .c
   - C++ : .cpp, .cc, .cxx

### Perbandingan Kode

**Kode C**:

```
#include <stdion.h>

void greet() {
  printf("Hello, World C!\n");
}

int main() {
  greey();
  return 0;
}
```

**Kode C++**:

```
#include <iostream>
using namespace std;

class Greeter {
  public:
    void greet() {
      cout << "Hello, World C++!" << endl;
    }
};

int main() {
  Greeter greeter;
  greeter.greet();
  return 0;
}
```

**Perbedaan Utama**:

1. **C** menggunakan `printf`, sedangkan **C++** menggunakan `cout`.
2. **C++** mengorganisasi fungsionalitas dalam kelas, mendukung modularitas dan penggunaan ulang kode.

## 4. Kesimpulan

C++ adalah pengembangan dari C yang menggabungkan paradigma prosedural dan berorientasi objek untuk menawarkan fleksibilitas, performa dan skalabilitas.

C++ tetap mempertahankan kesederhanaan dan kecepatan C sambil menambahkan fitur modern seperti kelas, pewarisan, dan library standar yang kuat.

Memahami perbedaan antara C dan C++ membantu kita memahami mengapa C++ cocok untuk pengembangan perangkat lunak yang kompleks dan berperforma tinggi.
