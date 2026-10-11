# 🔗 Modul 3 - Abstract Data Type (ADT) & Data Structures

Repository ini berisi penyelesaian tugas dan latihan untuk **Modul 3** pada mata kuliah **Struktur Data**.

## 👤 Identitas

* **Nama :** Ihsanul Rizky Merdiansyah
* **NIM :** 109102500026
* **Prodi :** Sains Data

---

## 📁 Struktur Folder

```text
Modul3_Latihan/
├── Soal1_Mahasiswa/
│   └── main.cpp
├── Soal2_Pelajaran/
│   ├── pelajaran.h
│   ├── pelajaran.cpp
│   └── main.cpp
├── Soal3_Array2DPointer/
│   └── main.cpp
└── README.md

# Ringkasan Materi
A. Konsep dan Definisi Abstract Data Type (ADT)
Abstract Data Type (ADT) atau Tipe Data Abstrak merupakan sebuah model matematika yang mendefinisikan suatu tipe data bersama dengan sekumpulan operasi primitif yang dapat dieksekusi terhadap tipe data tersebut. Secara konseptual, ADT menekankan prinsip abstraksi data dan enkapsulasi, di mana perilaku fungsional dari tipe data dipisahkan secara tegas dari representasi fisik dan detail implementasi internalnya di dalam memori komputer. Hal ini memungkinkan pemrogram untuk fokus pada cara entitas data berinteraksi dan diproses tanpa harus terbebani oleh rincian teknis struktur data di tingkat memori tingkat rendah.

Dalam sebuah ADT yang lengkap, pendefinisian mencakup invarian tipe (batasan keadaan data yang valid) serta aksioma yang berlaku. Elemen-elemen operasi primitif di dalam ADT dikelompokkan ke dalam beberapa kategori fungsional, yaitu:

1. Konstruktor/Kreator (Creator): Operasi pembentuk nilai tipe data atau instansiasi objek, biasanya diawali dengan predikat create atau make.

2. Selektor (Getter): Operasi yang digunakan untuk membaca atau mengakses nilai dari komponen spesifik suatu tipe data.

3. Mutator (Setter): Prosedur yang bertugas memodifikasi atau memperbarui nilai dari komponen spesifik tipe data.

4. Validator: Operasi logika yang mengevaluasi apakah instansiasi nilai suatu tipe memenuhi aturan batasan atau domain yang ditentukan.

5. Destruktor/Dealokator: Operasi untuk membebaskan ruang memori yang dialokasikan untuk suatu entitas data saat sudah tidak lagi digunakan.

6. Fungsi Baca/Tulis: Komponen antarmuka yang menangani aliran masukan (input) dan keluaran (output) pada perangkat.

7. Operator Relasional dan Aritmatika: Operasi komparasi relasional (seperti kesetaraan atau perbandingan besar-kecil) serta operasi perhitungan matematis yang didefinisikan secara khusus untuk tipe bentukan tersebut.


B. Struktur Modular dan Implementasi ADT dalam Pemrograman C++
Dalam paradigma prosedural dan pemrograman modular menggunakan bahasa C++, konsep ADT diterjemahkan melalui pembagian arsitektur kode ke dalam tiga berkas (file) terpisah:

1. Berkas Header (.h): Berisi spesifikasi tipe bentukan (struct) dan prototipe primitif (deklarasi fungsi dan prosedur). Berkas ini bertindak sebagai kontrak antarmuka (interface). Di dalamnya disematkan preprocessor wrapper/guards (#ifndef, #define, #endif) untuk menghindari kesalahan deklarasi ganda saat proses kompilasi.

2. Berkas Realisasi/Implementasi (.cpp): Memuat tubuh atau definisi lengkap (body) dari masing-masing fungsi dan prosedur primitif yang telah dideklarasikan pada berkas header. Realisasi ini mengoptimalkan penggunaan konstruktor dan selektor untuk menjamin integritas manipulasi data.

3. Berkas Driver/Program Utama (main.cpp): Berisi alur logika eksekusi utama program yang menyertakan (include) berkas header ADT. Berkas ini berfungsi untuk menguji instansiasi data serta pemanggilan operasi-operasi primitif yang telah dibangun.

Penerapan modularitas ini tidak hanya meningkatkan keterbacaan (readability) dan modularitas program, tetapi juga memaksimalkan reusability, di mana pustaka ADT yang telah dirancang dapat diintegrasikan ke proyek lain tanpa mengubah implementasi dasarnya.

Contoh Input & Output Program
Input:
======================================
 PROGRAM PENGELOLAAN NILAI MAHASISWA
======================================
Masukkan jumlah mahasiswa (maksimal 10): 2

Data Mahasiswa ke-1:
Nama        : Rama
NIM         : 1091
Nilai UTS   : 999
Nilai UAS   : 999
Nilai Tugas : 999

Data Mahasiswa ke-2:
Nama        : Dani
NIM         : 02500013
Nilai UTS   : 987
Nilai UAS   : 987
Nilai Tugas : 987

======================================================================
No   Nama            NIM            UTS      UAS      Tugas    Akhir
======================================================================
1    Rama            1091           999.00   999.00   999.00   999.00
2    Dani            02500013       987.00   987.00   987.00   987.00
======================================================================
