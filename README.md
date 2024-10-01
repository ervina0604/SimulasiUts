# 📚 Aplikasi CRUD Java Swing untuk Entitas Buku - Pertemuan Ketujuh

**Topik Utama:** Aplikasi CRUD Java Swing untuk mengelola informasi buku 📖

---

## 📑 Daftar Isi
- [🔗 Koneksi Database dengan JDBC](https://github.com/ervina0604/SimulasiUts/blob/main/Uts.java)
- [🛠️ DbUtils: Utilitas Database](https://github.com/ervina0604/SimulasiUts/blob/main/DbUtils.java)
- [🛠️ Implementasi CRUD](https://github.com/ervina0604/SimulasiUts/blob/main/Uts.java)

---

## 🔧 Fitur Utama
Aplikasi ini mengelola informasi buku dengan atribut berikut:
- **ISBN**: Nomor unik identifikasi buku 🔢.
- **Judul Buku**: Nama atau judul buku 📚.
- **Tahun Terbit**: Tahun buku diterbitkan 📅.
- **Penerbit**: Nama penerbit buku 🏢.

---

## 📋 Langkah-Langkah Penggunaan

### 1. Koneksi Database PostgreSQL
Pastikan telah menambahkan **library PostgreSQL JDBC** ke dalam proyek dan membuat koneksi ke database PostgreSQL yang berisi tabel **buku**. Ikuti langkah berikut:
- Tambahkan file JAR PostgreSQL JDBC ke dalam proyek Java Anda.
  ![Screenshot 2024-10-01 201030](https://github.com/user-attachments/assets/414e9c6d-3ab2-4c0a-8a39-7b4004809bce)
  
- Buat koneksi ke database menggunakan URL koneksi, username, dan password PostgreSQL 🔗.
  ![Screenshot 2024-10-01 200738](https://github.com/user-attachments/assets/d0c87ac3-b2c7-4c65-b51f-c446596ca2de)

---


### 2. Membuat Java DB Utils
Buat kelas `DbUtils` untuk mengkonversi objek **ResultSet** menjadi **TableModel** yang akan digunakan untuk menampilkan data dalam **JTable** 📊.

![Screenshot 2024-10-01 201040](https://github.com/user-attachments/assets/e188aa04-a3d7-49af-81bd-1a15f3cbdb13)

---

### 3. Membuat Desain GUI
Gunakan **Java Swing** untuk mendesain antarmuka pengguna. Komponen utama yang digunakan:
- **JTable**: Menampilkan data buku yang disimpan 📑.
- **JTextField**: Input untuk ISBN, Judul Buku, Tahun Terbit, Penerbit 🖊️.
- **JButton**: Tombol untuk operasi CRUD (Tambah, Update, Hapus, Clear) 🔘.
![Screenshot 2024-10-01 215018](https://github.com/user-attachments/assets/a9b621a6-c862-4549-becd-8f1d44dd3bf8)

---

### 4. Method Tampil dan TableMouseClicked
- **Method Tampil**: Menampilkan seluruh data buku yang tersimpan dalam database ke **JTable** 📋.
  ![Screenshot 2024-10-01 215115](https://github.com/user-attachments/assets/b94c39b6-560d-437c-bcc3-3b4f7460c83d)
- **TableMouseClicked**: Ketika pengguna memilih baris di **JTable**, data buku akan muncul di form input untuk diperbarui ✏️.
  ![Screenshot 2024-10-01 215134](https://github.com/user-attachments/assets/32ec9a2b-9a20-433d-9aaa-e8d01637f2bc)

---

### 5. Tambah Data (Button Add)
Pengguna dapat menambah buku baru ke dalam database. Data yang diinput melalui **JTextField** akan divalidasi dan kemudian disimpan.
![Screenshot 2024-10-01 215247](https://github.com/user-attachments/assets/7408679b-a4e8-4996-a61c-677e3a25f71b)
**Tampilan saat menambah data:**
Setelah menekan tombol **Tambah**, data akan tersimpan dan ditampilkan di **JTable** ✅.
![Screenshot 2024-10-01 215636](https://github.com/user-attachments/assets/7337c55d-7275-4f4d-8e2a-fe8a39a947dc)

---

### 6. Perbarui Data (Button Update)
Pengguna dapat memperbarui informasi buku yang sudah ada. Dengan memilih data dari **JTable**, data akan muncul di form input, dan pengguna dapat mengeditnya.
![Screenshot 2024-10-01 215329](https://github.com/user-attachments/assets/8c8852d9-1e25-42b4-b77b-ed9fb5c5597b)
**Tampilan saat memperbarui data:**
Setelah menekan tombol **Update**, perubahan data akan disimpan dan diperbarui di **JTable** 🔄.
![Screenshot 2024-10-01 215555](https://github.com/user-attachments/assets/30b33135-ace1-4dc3-9c88-141817a67242)

---

### 7. Hapus Data (Button Delete)
Pengguna dapat memilih buku dari **JTable**, dan kemudian menekan tombol **Hapus** untuk menghapus buku tersebut.
![Screenshot 2024-10-01 215304](https://github.com/user-attachments/assets/21a4289e-77b7-4fb1-9b64-502b29fc436d)
**Tampilan saat menghapus data:**
Setelah menghapus data, buku akan dihapus dari database dan **JTable** akan diperbarui ❌.
![Screenshot 2024-10-01 215705](https://github.com/user-attachments/assets/e9c5e95e-2305-4ffe-ab4f-52687cc6b38e)

---

### 8. Mengosongkan Input (Button Clear)
Tombol **Clear** digunakan untuk membersihkan semua field input agar siap untuk memasukkan data baru ✨.
![Screenshot 2024-10-01 215338](https://github.com/user-attachments/assets/861534e6-bb18-441f-b749-bf7c847b72d3)

---

### 🚀 Selamat Belajar dan Selamat Menerapkan Java Swing serta JDBC dalam Pengembangan Aplikasi! 💻

--- 
