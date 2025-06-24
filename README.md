# Tanya Daku Apa Saja

Aplikasi Flutter sederhana yang berperan sebagai bola ajaib digital (magic ball) untuk membantu menjawab pertanyaan secara acak. Pengguna cukup mengetuk gambar bola di layar, lalu gambar dan "jawaban" akan berubah secara random, memberikan efek seolah-olah aplikasi memberikan jawaban spontan untuk setiap pertanyaan.

## Fitur Utama

- **Tampilan Bola Ajaib:** Gambar bola tampil besar di tengah layar dengan desain biru modern.
- **Respons Interaktif:** Setiap kali gambar bola diketuk, aplikasi secara otomatis menampilkan gambar bola baru yang dipilih secara acak dari lima pilihan.
- **User Experience Sederhana:** Tidak ada menu atau tombol rumit—cukup buka aplikasi dan langsung gunakan.

## Cara Kerja

  1. **Aplikasi memuat gambar `ball1.png` sebagai gambar default saat pertama kali dibuka.**
  2. **Setiap kali gambar bola diketuk (tap), aplikasi akan memilih angka acak 1 sampai 5.**
  3. **Angka tersebut menentukan gambar bola yang akan muncul selanjutnya, misalnya:**
     - Jika angka 3 terpilih, maka gambar yang muncul adalah `ball3.png` dari folder asset.
  4. **Gambar diambil dari folder `images/` yang sudah didefinisikan pada pubspec.yaml.**

**Jalankan perintah berikut di terminal project:**
    ```sh
    flutter pub get
    flutter run
    ```

## Struktur Project
tanya_daku/
├── images/
│ ├── ball1.png
│ ├── ball2.png
│ ├── ball3.png
│ ├── ball4.png
│ └── ball5.png
├── lib/
│ └── main.dart
├── pubspec.yaml
└── README.md


## Penjelasan Singkat Kode

- `main.dart` berisi kode utama aplikasi.
- Aplikasi menggunakan widget `StatefulWidget` untuk mengganti gambar bola secara acak saat ditekan.
- Gambar diambil dari asset lokal di folder `images/`.

