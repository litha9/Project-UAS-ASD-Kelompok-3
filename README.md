# Project-UAS-ASD-Kelompok-3

Program berbasis Java yang digunakan untuk mengelola data nilai mahasiswa secara interaktif melalui terminal/console.

#  Fitur Utama

## Login Multi Role
- Login Admin
- Login User
- Logout Session
- Hak akses berbeda antara admin dan user

## CRUD Data Mahasiswa
- Tambah data mahasiswa
- Tampilkan data mahasiswa
- Edit data mahasiswa
- Hapus data mahasiswa
- Restore data mahasiswa

## Searching Data
- Cari Nama → Sequential Search
- Cari ID → Binary Search
- Cari Program Studi → Sequential Search

## Sorting Data
- Sort ID → Quick Sort
- Sort Nama → Quick Sort
- Sort Nilai → Quick Sort

## Statistik Mahasiswa
- Total mahasiswa
- Jumlah lulus dan tidak lulus
- Rata-rata nilai
- Persentase kelulusan
- Distribusi grade

## File Handling
- Auto Save ke `data.txt`
- Auto Load saat program dijalankan

## Interface Interaktif
- ASCII Table
- ANSI Color
- Loading Animation
- Progress Bar


# Algoritma yang Digunakan

| Fitur | Algoritma |

| Cari Nama | Sequential Search |

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
