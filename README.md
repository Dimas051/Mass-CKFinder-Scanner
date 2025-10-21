![alt text](https://d.top4top.io/p_3580tpzz81.png?raw=true)

🔍 Mass CKFinder Scanner 
Mendeteksi keberadaan CKFinder (sebuah file manager untuk web) yang mungkin tidak diproteksi dengan baik pada berbagai domain.

Apa itu CKFinder?
CKFinder adalah file manager yang sering digunakan bersama CKEditor (WYSIWYG editor) untuk mengupload dan mengelola file di website. Namun, jika tidak dikonfigurasi dengan benar, CKFinder dapat menjadi security risk karena memungkinkan:
 - Upload file arbitrary
 - Akses ke file sistem
 - Directory traversal

Security Implications:
   CKFinder yang terekspos dapat menyebabkan:
   - Arbitrary File Upload → RCE potential
   - Directory Traversal → Akses file sensitif
   - Information Disclosure → Struktur direktori
   - Unauthorized Access → File management tanpa autentikasi

📋 Cara Kerja
 - Membaca daftar domain dari file list.txt
 - Membaca daftar path CKFinder dari file path.txt
 - Menguji setiap kombinasi domain + path
 - Menyimpan hasil yang valid ke result.txt

🎨 Fitur
 - Multi-threading (20 threads) untuk scanning cepat
 - Color-coded output untuk readability
 - Error handling untuk koneksi bermasalah
 - Auto-save hasil scanning

   
