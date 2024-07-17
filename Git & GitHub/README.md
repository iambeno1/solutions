# Problems
repo untuk menyimpan penyelesaian masalah yg dialami seputar coding

## ERROR : refusing to merge unrelated histories
Pesan kesalahan "refusing to merge unrelated histories" biasanya terjadi karena repositori lokal Anda dan repositori remote tidak memiliki sejarah commit yang sama. Ini bisa terjadi jika Anda menginisialisasi repositori lokal secara terpisah dari repositori remote.

Untuk mengatasi masalah ini, Anda bisa menggunakan opsi `--allow-unrelated-histories` saat melakukan `git pull`. Berikut adalah langkah-langkah yang bisa Anda ikuti:

1. **Tarik perubahan dari repositori remote dengan opsi `--allow-unrelated-histories`:**
   ```sh
   git pull origin main --allow-unrelated-histories
   ```

2. **Selanjutnya, dorong perubahan lokal Anda ke repositori remote:**
   ```sh
   git push -u origin main
   ```

Langkah-langkah tersebut seharusnya memungkinkan Anda untuk menggabungkan sejarah commit dari kedua repositori dan kemudian melakukan push. Dan Berhasil.
