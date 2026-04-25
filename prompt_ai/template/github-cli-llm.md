# Panduan Prompting (Bahasa Manusia) untuk Mengelola GitHub via AI
Dokumen ini berisi kumpulan *template prompt* (perintah dalam bahasa manusia sehari-hari) yang bisa Anda gunakan saat menyuruh AI untuk mengelola GitHub Anda. Anda tidak perlu menghafal syntax command line (seperti `gh issue create...`), cukup gunakan atau modifikasi instruksi bahasa natural di bawah ini.

## 1. Autentikasi (Login & Status)
- "Tolong cek apakah saat ini saya sudah login ke GitHub di terminal ini."
- "Saya belum login, tolong bantu saya login ke akun GitHub menggunakan web browser."
- "Bantu saya login ke GitHub menggunakan Personal Access Token (PAT) yang sudah saya siapkan."

## 2. Manajemen Repositori
- **Membuat Repositori Baru:** "Tolong buatkan repositori GitHub [pilih: publik / privat] baru dari folder proyek ini, dan langsung push kode yang ada sekarang ke sana."
- **Clone Repositori:** "Tolong clone repositori `[nama-owner]/[nama-repo]` ke folder ini."
- **Forking:** "Tolong fork repositori `[nama-owner]/[nama-repo]` ke akun saya dan langsung clone ke komputer ini."
- **Info Repositori:** "Tolong tampilkan ringkasan informasi dan deskripsi tentang repositori yang sedang aktif ini."

## 3. Manajemen Issue
- **Melihat Issue:** "Tolong tampilkan daftar semua issue yang masih open di repositori ini."
- **Membuat Issue Baru:** "Tolong buatkan issue baru dengan judul '[Tulis Judul Issue]' dan deskripsinya '[Tulis Penjelasan Detail]'. Tolong *assign* issue ini ke saya."
- **Membaca Issue:** "Tolong bacakan percakapan dan detail dari issue nomor #[nomor-issue]."
- **Memberi Komentar:** "Tolong tambahkan komentar pada issue nomor #[nomor-issue] dengan pesan '[Isi Komentar Anda]'."
- **Menutup Issue:** "Bug ini sudah diperbaiki, tolong tutup issue nomor #[nomor-issue]."

## 4. Manajemen Pull Request (PR)
- **Membuat PR:** "Saya sudah selesai mengerjakan fitur ini. Tolong buatkan Pull Request dari branch ini ke branch `main`. Judulnya '[Judul PR]' dan tolong buatkan rangkuman otomatis untuk deskripsinya."
- **Melihat Daftar PR:** "Ada berapa Pull Request yang sedang menunggu untuk direview? Tolong tampilkan daftarnya."
- **Review PR:** "Tolong berikan komentar '[Komentar Review]' pada PR nomor #[nomor-pr] dan langsung *approve* PR tersebut."
- **Merge PR:** "Semuanya sudah oke, tolong *merge* Pull Request nomor #[nomor-pr] menggunakan metode squash, lalu hapus branch-nya."

## 5. CI/CD (GitHub Actions)
- **Melihat Daftar:** "Tolong tampilkan daftar GitHub Actions (workflow) yang ada di repositori ini."
- **Mengecek Status:** "Tolong cek status pipeline workflow yang terakhir kali berjalan, apakah gagal atau berhasil?"
- **Menjalankan Manual:** "Tolong jalankan manual workflow '[nama-workflow]' sekarang juga."

## 6. Manajemen Release & Gist (Snippet)
- **Membuat Release:** "Aplikasi sudah stabil. Tolong buatkan GitHub Release baru untuk versi `v[angka-versi]` dengan catatan rilis '[Tulis Catatan Singkat]'. Ambil dari branch main."
- **Membuat Gist:** "Tolong simpan file `[nama-file]` ini sebagai GitHub Gist publik agar saya bisa membagikan *snippet* kodenya ke orang lain."

---

### Tips Berinteraksi dengan AI untuk Tugas GitHub:
1. **Berikan Konteks Posisi:** Karena AI paham terminal Anda, Anda cukup menyebutkan *"di repositori ini"* atau *"dari folder ini"*.
2. **Gabungkan Tugas:** Anda bisa menggabungkan instruksi. Contoh: *"Tolong commit semua perubahan saya dengan pesan 'fix header', lalu buatkan Pull Request ke main."*
3. **Minta Rangkuman:** AI sangat bagus untuk membaca log panjang. Contoh: *"Tolong baca log dari pipeline yang gagal kemarin dan beri tahu saya file mana yang menyebabkan error."*
