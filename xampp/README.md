# Problems
Berikut adalah masalah-masalah yang mungkin ditemukan saat menggunakan XAMPP dan cara menyelesaikannya (_Berdasarkan pengalaman pribadi_)

## ERROR : MySQL shutdown unexpectedly
![image](https://github.com/user-attachments/assets/92532e8c-d5a5-43ff-816f-93c37d875f32)

Berikut adalah cara mengatasi error "MySQL shutdown unexpectedly" pada XAMPP:

---

**Solusi untuk Error "MySQL shutdown unexpectedly" pada XAMPP:**

1. **Buka XAMPP Control Panel:**
   - Jalankan aplikasi XAMPP di komputer Anda.

2. **Gunakan XAMPP Shell:**
   - Klik tombol "Shell" pada XAMPP Control Panel untuk membuka command prompt (shell) XAMPP.

3. **Jalankan MySQL tanpa grant tables dan external locking:**
   - Ketik perintah berikut di shell XAMPP dan tekan Enter:
     ```sh
     mysqld --console --skip-grant-tables --skip-external-locking
     ```
   - Ini akan menjalankan MySQL tanpa mengecek grant tables dan external locking. Jangan tutup jendela shell ini, cukup minimalkan.

4. **Buka Shell Baru di XAMPP:**
   - Buka shell baru dengan mengklik tombol "Shell" lagi pada XAMPP Control Panel.

5. **Perbaiki Database MySQL:**
   - Di shell baru, ketik perintah berikut dan tekan Enter:
     ```sh
     mysqlcheck -r --databases mysql --use-frm
     ```
   - Perintah ini akan memeriksa dan memperbaiki tabel di database `mysql` menggunakan file `.frm`.

6. **Mulai Ulang MySQL:**
   - Kembali ke XAMPP Control Panel dan coba klik tombol "Start" pada MySQL. MySQL seharusnya sekarang bisa berjalan dengan normal.

---
## ERROR : MySQL shutdown unexpectedly (Cara 2)
nonton ini <a href="https://www.youtube.com/watch?v=84IOtc05TuA">youtube</a> <br><br>
langkah 1: hapus semua file yg dipilih (ikut jalur direktori yg sesuai)<br><br>
![image](https://github.com/user-attachments/assets/4c509254-a724-4af6-948b-09762cfdbb66)

langkah 2: setelah semuanya dihapus, sekarang tinggal ambil (Copy) file dari direktori backup dan paste di dalam direktori data<br><br>
![image](https://github.com/user-attachments/assets/1515792e-eb35-4989-9bc8-2be4f02fa454)

paste disini:
![image](https://github.com/user-attachments/assets/defde1be-785e-4aca-a2d7-b2abf35104b8)



