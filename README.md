# 🎓 Sistem Manajemen Nilai Mahasiswa

> Aplikasi berbasis **Java Console** untuk mengelola data nilai mahasiswa secara cepat, terstruktur, dan interaktif dengan fitur autentikasi multi-role, CRUD data, searching, sorting, statistik akademik, serta penyimpanan file otomatis.


---

## 📖 Deskripsi Program

**Sistem Manajemen Nilai Mahasiswa** merupakan aplikasi berbasis terminal/console yang digunakan untuk mengelola data akademik mahasiswa secara lengkap. Program ini menerapkan konsep **Object-Oriented Programming (OOP)** serta mengimplementasikan berbagai algoritma dasar seperti **Searching**, **Sorting**, dan **File Handling**.

Aplikasi mendukung dua jenis pengguna (**Admin** dan **User**) dengan hak akses yang berbeda untuk menjaga keamanan serta integritas data.

---

# ✨ Fitur Utama

## 🔐 Login Multi Role

Program menyediakan sistem autentikasi dengan dua jenis pengguna:

| Role | Hak Akses |
|--------|------------|
| Admin | Mengelola seluruh data mahasiswa |
| User | Melihat data miliknya sendiri |

### Fitur Login
- Login Admin
- Login User
- Logout Session
- Validasi Username dan Password
- Hak akses berbeda berdasarkan role

---

## 📋 Manajemen Data Mahasiswa (CRUD)

Admin dapat melakukan pengelolaan data mahasiswa secara penuh.

### Fitur:
- ➕ Tambah Data Mahasiswa
- 📄 Tampilkan Data Mahasiswa
- ✏️ Edit Data Mahasiswa
- 🗑️ Hapus Data Mahasiswa (Soft Delete)
- ♻️ Restore Data Mahasiswa

### Validasi Data:
- ID Mahasiswa harus unik
- Nilai berada pada rentang 0–100
- Input tidak boleh kosong

---

## 🔍 Searching Data

Program menyediakan fitur pencarian mahasiswa berdasarkan beberapa kriteria.

| Pencarian | Algoritma |
|------------|------------|
| Nama Mahasiswa | Sequential Search |
| ID Mahasiswa | Binary Search |
| Program Studi | Sequential Search |

---

## 📊 Sorting Data

Data mahasiswa dapat diurutkan menggunakan algoritma Quick Sort.

| Pengurutan | Algoritma |
|------------|------------|
| ID Mahasiswa | Quick Sort |
| Nama Mahasiswa | Quick Sort |
| Nilai Akhir | Quick Sort |

---

## 📈 Statistik Mahasiswa

Program dapat menghasilkan informasi statistik akademik secara otomatis.

### Informasi yang Ditampilkan:
- Total Mahasiswa Aktif
- Jumlah Mahasiswa Lulus
- Jumlah Mahasiswa Tidak Lulus
- Rata-rata Nilai
- Persentase Kelulusan
- Distribusi Grade (A, B, C, D, E)

---

## 💾 File Handling

Seluruh data mahasiswa disimpan secara permanen menggunakan file teks.

### Mekanisme:
- Auto Save setiap ada perubahan data
- Auto Load saat program dijalankan
- Penyimpanan menggunakan file `data.txt`

---

## 🖥️ Interface Interaktif

Untuk meningkatkan pengalaman pengguna, program dilengkapi dengan:

- ANSI Color Terminal
- ASCII Table
- Loading Animation
- Progress Bar
- Menu Navigasi Interaktif

---

# 🧮 Algoritma yang Digunakan

| Fitur | Algoritma |
|--------|------------|
| Cari Nama | Sequential Search |
| Cari ID | Binary Search |
| Cari Program Studi | Sequential Search |
| Sort ID | Quick Sort |
| Sort Nama | Quick Sort |
| Sort Nilai | Quick Sort |

---

# 🏗️ Struktur Data

Program menggunakan struktur data sederhana berbasis array dan object.

### Implementasi:
- Array of Object
- Class `Mahasiswa`
- Array `Mahasiswa[200]`

Contoh:

```java
Mahasiswa[] dataMahasiswa = new Mahasiswa[200];
```

---

# 📚 Perhitungan Nilai

Nilai akhir mahasiswa dihitung menggunakan rumus:

```text
Nilai Akhir = (Tugas × 30%)
             + (UTS × 30%)
             + (UAS × 40%)
```

## Konversi Grade

| Rentang Nilai | Grade |
|---------------|--------|
| ≥ 85 | A |
| ≥ 75 | B |
| ≥ 65 | C |
| ≥ 50 | D |
| < 50 | E |

## Status Kelulusan

| Nilai Akhir | Status |
|-------------|---------|
| ≥ 60 | LULUS |
| < 60 | TIDAK LULUS |

---

# 🚀 Cara Menjalankan Program

## Prasyarat

- Java JDK 8 atau versi yang lebih baru sudah terinstall.
- Terminal atau Command Prompt.
- File source code program berada dalam satu folder project.

## Langkah-langkah

### 1. Compile Program

```bash
javac SistemManajemenPenilianMahasiswa.java
```

### 2. Jalankan Program

```bash
java SistemManajemenPenilianMahasiswa
```

### 3. Login ke Sistem

Gunakan akun default yang tersedia:

**Admin**
```text
Username : admin
Password : 123
```

**User**
```text
Username : ID Mahasiswa
Password : 123
```

---

# 🔑 Akun Login Default

> ⚠️ Disarankan untuk mengganti password setelah pertama kali login.

## Admin

```text
Username : admin
Password : 123
```

## User

```text
Username : Gunakan ID Mahasiswa
Password : 123
```

---

# 📂 Struktur Project

```text
📦 Sistem-Manajemen-Nilai-Mahasiswa
│
├── SistemManajemenPenilaianMahasiswa.java
├── data.txt
├── README.md
└── .gitignore
```

---

# 📄 Deskripsi File

| File | Fungsi |
|--------|----------|
| `SistemManajemenPenilaianMahasiswa.java` | Source code utama program |
| `data.txt` | Penyimpanan data mahasiswa |
| `README.md` | Dokumentasi proyek |
| `.gitignore` | Konfigurasi file yang diabaikan Git |

---

# 🧠 Konsep Pemrograman yang Diterapkan

Program ini mengimplementasikan berbagai konsep dasar dalam pemrograman Java:

- Object Oriented Programming (OOP)
- Encapsulation
- Array of Object
- Searching Algorithm
- Sorting Algorithm
- File Handling
- Validasi Input
- Percabangan (Selection)
- Perulangan (Looping)
- Exception Handling
- Statistik Data Sederhana

---

# 🖼️ Tampilan Program

## Menu Utama

```text
====================================
   SISTEM MANAJEMEN NILAI MAHASISWA
====================================

1. Tambah Data Mahasiswa
2. Tampilkan Data
3. Edit Data
4. Hapus Data
5. Cari Nama
6. Cari ID
7. Cari Program Studi
8. Sort ID
9. Sort Nama
10. Sort Nilai
11. Statistik
12. Restore Data
13. Logout
0. Keluar

Pilih Menu :
```

---

# 👨‍💻 Tim Pengembang

### Kelompok Proyek UAS

- **Firman Hidayat**
- **Talitha Nailal Husna**
- **Radhin Ramadhan Hendestian**

---

## ⭐ Tujuan Pembelajaran

Proyek ini dibuat sebagai implementasi materi:

- Struktur Data
- Algoritma Searching
- Algoritma Sorting
- Object Oriented Programming


---

<div align="center">

### 🎓 Sistem Manajemen Nilai Mahasiswa
*Mengelola data akademik secara cepat, terstruktur, dan efisien.*

</div>
