# Uji-Kompetensi-2

# Sistem Kuisioner Akademik Berbasis Web  
Uji Kompetensi Akhir Praktikum – Pemrograman Web  
Semester Ganjil 2025/2026

## Deskripsi Proyek
Proyek ini merupakan aplikasi **Sistem Kuisioner Akademik** berbasis web yang dikembangkan sebagai bagian dari **Uji Kompetensi Akhir Praktikum Mata Kuliah Pemrograman Web (INF11010)**.

Aplikasi ini digunakan untuk mengelola dan mengisi kuisioner akademik dengan beberapa peran pengguna, yaitu:
- **Admin**
- **Kaprodi**
- **Mahasiswa**
- **Pimpinan**

Sistem dibangun menggunakan **framework CodeIgniter 4 (CI4)** dan menerapkan konsep **role-based access control**, pengelolaan data terstruktur, serta relasi basis data sesuai dengan ketentuan soal.

---

## Fitur Utama

### 1. Admin
- Manajemen user dan role (admin, kaprodi, mahasiswa, pimpinan)
- Manajemen fakultas, jurusan, dan program studi
- Penentuan kaprodi untuk setiap prodi
- Manajemen data mahasiswa

### 2. Kaprodi
- Membuat periode kuisioner
- Menambahkan pertanyaan kuisioner (pilihan ganda)
- Melihat jawaban mahasiswa
- Melihat ringkasan (summary) hasil kuisioner per periode

### 3. Mahasiswa
- Melihat daftar periode kuisioner
- Mengisi kuisioner sesuai periode
- Melihat kembali jawaban yang telah diisi sebelumnya

### 4. Pimpinan
- Melihat summary pengisian kuisioner
- Rekap jawaban mahasiswa per periode dan per pertanyaan

---

## Teknologi yang Digunakan
- **Backend**: PHP 8.x
- **Framework**: CodeIgniter 4
- **Database**: MySQL / MariaDB
- **Frontend**: HTML, CSS, JavaScript
- **Tools**: Composer

---

## Struktur Database
Sistem ini menggunakan beberapa tabel utama, antara lain:
- `user`
- `fakultas`
- `jurusan`
- `prodi`
- `periode_kuisioner`
- `pertanyaan`
- `pilihan_jawaban_pertanyaan`
- `pertanyaan_periode_kuisioner`
- `mahasiswa`
- `jawaban`

Relasi tabel dirancang untuk mendukung:
- Pertanyaan berbeda pada setiap periode
- Riwayat jawaban mahasiswa pada periode yang berbeda
