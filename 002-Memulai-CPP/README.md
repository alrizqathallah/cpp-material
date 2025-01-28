# Memulai dengan C++

## 1. Memulai dengan C++

C++ adalah bahasa pemrograman yang banyak digunakan untuk membangun aplikasi yang efisien dan berperforma tinggi.

Sebelum mulai menulis program, penting untuk menyiapkan lingkungan pengembangan terlebih dahulu.

## 2. Instal IDE untuk Pengembangan C++

Untuk menulis, mengompilasi dan men-debug kode C++, Anda memerlukan **Integrated Development Environment (IDE)** atau **Text Editor** dengan dukungan untuk C++.

### IDE dan Text Editor Populer untuk C++

1. **Visual Studio (Windows)**
   - IDE lengkap buatan Microsoft dengan dukungan penuh untuk C++.
   - Menyediakan debugger bawaan dan IntellisSense.
   - Unduh lewat halaman Visual Studio.
2. **CLion (Cross-platform)**
   - IDE professional dari JetBrains dengan fitur canggih.
   - Membutuhkan lisensi setelah masa percobaan gratis.
   - Unduh CLion lewat halaman resmi JetBrains.
3. **Visual Studio Code (Cross-platform)**
   - Kode editor ringan yang sangat dapat dikostumisasi.
   - Memerlukan ekstensi untuk pengembangan C++.
   - Unduh mealului halaman resmi Visual Studio Code.
4. **Neovim (Cross-platform)**
   - Teks editor berbasis terminal dengan konfigurasi yang kuat.
   - Cocok untuk pengguna yang menyukai pengaturan minimalis.
   - Situs web: Neovim.

## 3. Mengatur C++ di Visual Studio Code

\*Visual Studio Code\*\* adalah editor ringan dan serbaguna untuk pemrograman C++.

Berikut langkah-langkah untuk menyiapkannya:

**Langkah 1: Instal VSCode**

1. Unduh dan instal **VSCode**, lewat halaman resmi.
2. Buka VSCode setelah instalasi selesai.

**Langkah 2: Instal Ekstensi C++**

1. Buka **Ekstension View** dengan mengklik ikon kotak di sidebar atau tekan `Ctrl+Shift+X`.
2. Cari dan instal ekstensi berikut:
   - **C/C++** oleh Microsoft (menyediakan IntelliSense dan dukungan debugging).
   - (Opsional) **Code Runner** untuk menjalankan kode C++ dengan cepat.

**Langkah 3: Instal Compiler C++**

- Untuk **Windows**: Instal **MinGW** atau **MSYS2**.
  - MinGW: Unduh MinGW.
  - Tambahkan folder `bin` ke PATH sistem.
- Untuk **Linux**: Instal g++ melalui manajer paket:
  ```
  sudo apt install g++
  ```
- Untuk **MacOS**: Instal **Xcode Command Line Tools**:
  ```
  xcode-select --install
  ```

**Langkah 4: Konfigurasi Build Task**

1. Buka folder untuk proyek.
2. Tekan `Ctrl+Shift+B` dan pilih `C++: g++.exe build active file` untuk menghasilkan file `tasks.json`.
3. Pastikan `tasks.json` menunjuk ke compiler dengan benar.

**Langkah 5: Menulis dan Menjalankan Kode**

1. Buat file baru dengan ekstensi `.cpp` (contoh: `main.cpp`).
2. Tulis kode dan simpan file.
3. Gunakan `Ctrl+Alt+N` (dengan Code Runner) atau konfigurasi file launch untuk debugging.

## 4. Mengatur C++ di Neovim

Neovim adalah editor berbasis terminal yang sangat kuat dan cocok untuk pengembangan yang menyukai pengaturan minimalis.

Berikut adalah langkah-langkah untuk mengatur Neovim untuk pemrograman C++.

**Langkah 1: Instal Neovim**

1. Unduh Neovim dari neovim.io dan instal.
2. Verifikasi instalasi
   ```
   nvim --version
   ```

**Langkah 2: Instal Compiler C++**

Ikuti langkah instalasi compiler yang sama seperti pada pengaturan di VSCode.

**Langkah 3: Instal Plugin Manager**

1. Gunakan **lazy.nvim** (atau plugin manager lainnya).
2. Tambahkan plugin manager ke file `init.lua` atau `init.vim`.

**Langkah 4: Tambahkan Plugin untuk C++**

Instal plugin untuk highlighting, IntelliSense, dan debugging:

- **nvim-treesitter**: Untuk highlighting sintaks.
- **nvim-lspconfig**: Untuk Language Server Protocol (LSP) yang menyediakan IntelliSense.
- **coc.nvim** atau **cmp-nvim**: Untuk autocompletion.

Contoh konfigurasi di init.lua:

```
require('nvim-treesitter.configs').setup {
  ensure_installed = {"cpp"},
  highlight = { enable = true }
}

require('lspconfig').clangd.setup {} -- Mengatur language server untuk C++
```

**Langkah 5: Kompilasi dan Jalankan**

1. Gunakan `:!g++ % -o %:r && ./%:r` untuk mengompilasi dan menjalankan file saat ini.
2. Otomatiskan dengan keybinding khusus di konfigurasi Neovim.

## 5. C++ Quickstart

### Program C++ Sederhana

Berikut adalah contoh program "Hello, World!" dalam C++.

```
include <iostream>                    // Dibutuhkan untuk operasi input/output
using namespace std;

int main() {
  cout << "Hello, World!" << endl; // Menampilkan teks ke konsol
  return 0;                       // Menunjukan eksekusi berhasil
}
```

### Langkah untuk Menjalankan

1. **Di VSCode**:
   - Tulis program di file .cpp (contoh: hello.py).
   - Kompilasi menggunakan `Ctrl+Shift+B` atau terminal:
     ```
     g++ hello.cpp -o hello
     ./hello
     ```
2. **Di Neovim**:
   - Tulis kode dalam file `.cpp` dan simpan.
   - Kompilasi dan jalankan dengan:
     ```
     g++ hello.cpp -o hello && ./hello
     ```

## 6. Kesimpulan

- **VSCode** dan **Neovim** adalah alat yang hebat untuk pengembangan C++, masing-masing melayani prefensi yang berbeda.
- Instal compiler seperti `g++` sangat penting untuk mengompilasi dan menjalankan kode.
- Mulailah dengan program sederhana seperti "Hello, World!" untuk memahami pengaturan dan alur kerja.
- Seiring waktu, eksplorasi alat debugging dan konfigurasi lanjutan untuk lingkungan pengembangan.
