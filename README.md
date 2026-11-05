PETUALANGAN TKA BAHASA INDONESIA - SD NEGERI 3 MUARA RUPIT

FILE:
- index.html : aplikasi kuis dan dasbor guru.
- firestore.rules : contoh aturan keamanan database.

PENTING: Aplikasi belum tersambung ke Firebase sampai konfigurasi diisi.
1. Buka https://console.firebase.google.com/ dan buat proyek.
2. Tambahkan aplikasi Web, salin konfigurasi Firebase.
3. Di index.html, ganti GANTI_API_KEY, GANTI_PROJECT, GANTI_PROJECT_ID,
   GANTI_SENDER_ID, dan GANTI_APP_ID sesuai Firebase Console.
4. Authentication > Sign-in method: aktifkan Email/Password.
5. Authentication > Users: buat akun guru.
6. Salin UID akun guru, ganti GANTI_UID_GURU di firestore.rules.
7. Buat Firestore Database, lalu terapkan isi firestore.rules.
8. Uji login guru dan simpan satu hasil kuis.

PUBLIKASI GITHUB PAGES:
1. Buat repositori GitHub (mis. tka-bahasa-indonesia).
2. Upload index.html dan firestore.rules (README opsional) ke root repositori.
3. Settings > Pages > Deploy from a branch > main > /(root) > Save.
4. Tunggu proses selesai; alamat situs akan tampil di halaman Pages.

CATATAN:
- GitHub Pages hanya meng-host file statis; Firebase menyediakan autentikasi dan cloud database.
- Jangan pernah memasukkan password guru ke dalam HTML.
- Ganti UID guru dalam Firestore Rules. Aturan contoh hanya mengizinkan satu UID guru.
- Siswa bisa mengirim hasil, tetapi tidak bisa membaca rekap. Hanya UID guru yang diizinkan dapat membaca.
- Bentuk benar-salah dan pilihan kompleks adalah latihan tambahan, bukan format lengkap TKA resmi.
- Untuk kelas V dan VI, materi dibuat bertingkat; bank soal dapat ditambah dan ditelaah guru.
