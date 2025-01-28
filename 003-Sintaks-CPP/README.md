# Sintaks C++

## 1. Pendahuluan ke Sintaks C++

Sintaks C++ adalah seperangkat aturan yang mendefinisikan cara program C++ ditulis dan diinterpretasikan oleh compiler. Memahami sintaks sangat penting agar kode dapat terstruktur dengan baik dan dapat dijalankan tanpa kesalahan.

## 2. Struktur Dasar Sintaks C++

Setiap program C++ mengikuti struktur standar yang melibatkan fungsi, pernyataan (statements), dan cara tertentu mengorganisasi kode.

### Struktur Umum Program C++

```
include <iostream>                     // Menyertakan pustaka input/output

using namspace std;                   // Memungkinkan penggunaan namspace standar (opsional)

int main() {                         // Fungsi utama tempat eksekusi dimulai

  cout << "Hello, World! << endl;   // Pernyataan untuk mencetak output

  return 0;                        // Menandakan eksekusi berhasil
}
```

## 3. Penjelasan Contoh Program

Mari bahas komponen dari program C++ sederhana berikut:

### Contoh Program

```
include <iostream>
using namespace std;

int main() {
  cout << "Hello, World!" << endl;

  return 0;
}
```

### Penjelasan

1. `#include <iostream>`

   - Direktif preprocessor untuk menyertakan pustak input/output.
   - Diperlukan untuk menggunakan fungsi seperti `cout` dan `cin`.

2. `using namespace std;`

   - Memungkinkan penggunaan namespace `std` tanpa harus menulisnya secara eksplisit.
   - Contoh: Daripada menulis `std::cout`, cukup menulis `cout`.

3. `int main()`

   - Fungsi `main` adalah titik masuk program C++. Wajib ada dalam setiap program dan tempat eksekusi dimulai

4. `cout << "Hello, World!" << endl;`

   - `cout`: Singkatan dari "character output", digunakan untuk mencetak teks ke konsol.
   - `<<`: Operator penyisipan untuk mengarahkan output ke `cout`.
   - `"Hello, World!"`: Teks yang akan dicetak.
   - `endl;`: Mengakhiri baris dan membersihkan buffer output.

5. `return 0;`
   - Menandakan program selesai dijalankan dengan sukses.
   - `return 0`: adalah konvensi di C++ untuk menunjukan eksekusi berhasil.

## 4. Menghilangkan Namspace

Dalam C++, bisa menghilangkan pernyataan `using namespace std;`, tetapi harus menggunakan namespace `std` secara eksplisit untuk fitur pustaka standar seperti `cout` dan `cin`.

### **Kode Tanpa** `using namespace std;`

```
#include <iostream>

int main() {
  std::cout << "Hello, World!" << std::endl;   // Menggunakan namespace std secara eksplisit

  return 0;
}
```

### Perbedaan Utama

- **Dengan** `using namespace std;`:
  - Kode lebih pendek dan lebih mudah dibaca untuk program kecil.
  - Contoh: `cout << "Hello, World!;`
- \*\*Tanpa `using namespace std;`:
  - Menghindari "polusi namespace", berguna untuk program besar dengan banyak pustaka.
  - Contoh: `std::cout << "Hello";`

## 5. Contoh Sintaks Lengkap

Berikut adalah program yang lebih kompleks menggunakan berbagai elemen sintaks:

```
#include <iostream>

int main() {
  // Deklarasi variabel
  int age = 25;
  double pi = 3.14;
  char grade = 'A';

  // Output
  std::cout << "Umur: " << age << std::endl;
  std::cout << "Nilai PI: " << pi << std::endl;
  std::cout << "Nilai: " << grade << std::endl;

  // Pernyataan Kondisional
  if (age > 18) {
    std::cout << "Anda adalah seorang dewasa." << std::endl;
  }

  // Perulangan
  for (int i = 0; i < 5; i++) {
    std::cout << "Iterasi perulangan: " << i << std::endl;
  }

  return 0;
}
```

### Penjelasan

1. **Variabel**: Menunjukan penggunaan berbagai tipe data (`int`, `double`, `char`).

2. **Output**: Menggunakan `std::cout` untuk mencetak nilai dan teks.

3. **Pernyataan Kondisional**: Blok `if` memeriksa kondisi dan menjalankan kode jika kondisi benar.

4. **Perulangan**: Perulangan `for` berjalan lima kali, mencetak iterasi saat ini.

## 6. Kesimpulan

- Sintaks C++ mendefinisikan cara menulis kode C++ dengan benar.

- Program C++ dasar mencakup:

  - Direktif preprocessor seperti `#include <iostream>`.
  - Fungsi utama (`main`) sebagai titik awal.
  - Pernyataan dan ekspresi untuk melakukan aksi.

- Pernyataan `using namespace std;` bersifat opsional, tetapi memengaruhi cara penulisan kode.

- Latih penulisan dengan program kecil untuk memahami elemen sintaks dan komponennya.
