# 🎓 Sistem Manajemen Nilai Mahasiswa

> Aplikasi berbasis **Java Console** untuk mengelola data nilai mahasiswa secara cepat, terstruktur, dan interaktif dengan fitur autentikasi multi-role, CRUD data, searching, sorting, statistik akademik, serta penyimpanan file otomatis.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Console-blue?style=for-the-badge)
![OOP](https://img.shields.io/badge/Concept-OOP-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

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

## 1️⃣ Clone Repository

```bash
git clone https://github.com/username/repository.git
```

## 2️⃣ Masuk ke Folder Project

```bash
cd repository
```

## 3️⃣ Compile Program

```bash
javac SistemManajemenPenilaianMahasiswa.java
```

## 4️⃣ Jalankan Program

```bash
java SistemManajemenPenilaianMahasiswa
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
├
| Cari ID | Binary Search |

| Cari Prodi | Sequential Search |

| Sort ID | Quick Sort |

| Sort Nama | Quick Sort |

| Sort Nilai | Quick Sort |


# Struktur Data

Program menggunakan:

- Array of Object
- Class `Mahasiswa`
- Array `Mahasiswa[200]`

# Perhitungan Nilai

Nilai akhir dihitung menggunakan rumus:

Nilai Akhir = (Tugas × 0.3) + (UTS × 0.3) + (UAS × 0.4)

Grade:

| Nilai | Grade |

| ≥ 85 | A |

| ≥ 75 | B |

| ≥ 65 | C |

| ≥ 50 | D |

| < 50 | E |

Status:
- LULUS → nilai akhir ≥ 60
- TIDAK LULUS → nilai akhir < 60

#  Cara Menjalankan Program

## 1. Compile Program

javac SistemManajemenPenilianMahasiswa.java

## 2. Jalankan Program

java SistemManajemenPenilianMahasiswa

# Login Default

## Admin
Username : admin
Password : 123


## User
Username : gunakan ID mahasiswa
Password : 123

# File Project

| File | Fungsi |

| `SistemManajemenPenilianMahasiswa.java` | Source code utama |

| `data.txt` | Penyimpanan data mahasiswa |

| `README.md` | Dokumentasi project |

# Konsep Pemrograman yang Digunakan

- Object Oriented Programming (OOP)
- Array
- Searching Algorithm
- Sorting Algorithm
- File Handling
- Percabangan
- Perulangan
- Validasi Input
- Statistik Sederhana

# Tampilan Program

## Menu Utama
```text
1. Tambah Data Mahasiswa
2. Tampilkan Data
3. Edit Data
4. Hapus Data
5. Cari Nama
6. Cari ID
7. Cari Prodi
8. Sort ID
9. Sort Nama
10. Sort Nilai
11. Statistik
12. Restore Data
13. Logout
0. Keluar
