# AGENTS.md

## 1. Plan dulu, baru eksekusi
- Sebelum mengubah file, menjalankan perintah, atau menginstall apa pun,
  SELALU buat Implementation Plan terlebih dahulu.
- Isi plan:
  - Tujuan dan ruang lingkup
  - Daftar file yang akan dibuat atau diubah
  - Langkah kerja berurutan
  - Risiko dan dampak
  - Cara verifikasi hasil
- Tunggu persetujuan saya sebelum mulai eksekusi.
- Jika rencana berubah di tengah jalan, berhenti, perbarui plan,
  lalu minta persetujuan lagi.

## 2. Berpikir out of the box
- Jangan langsung mengambil solusi paling umum.
- Di dalam plan, tawarkan minimal 2 pendekatan: satu standar dan satu
  tidak konvensional. Jelaskan trade-off, lalu rekomendasikan satu.
- Pertanyakan asumsi permintaan saya. Jika ada cara yang lebih sederhana,
  lebih cepat, atau lebih kreatif, sampaikan.
- Jika menemukan masalah lain di luar permintaan, catat di plan.
  Jangan diperbaiki diam-diam.

## 3. Aturan khusus pembuatan UI/UX
Jika saya meminta UI (halaman web, aplikasi, dashboard, komponen,
atau layar mobile), lakukan ini SEBELUM membuat Implementation Plan:

1. Riset internet dulu. Cari framework, library UI, dan tren desain
   yang sedang dipakai saat ini. Utamakan sumber resmi dan cek versi terbaru.
2. Sesuaikan dengan stack yang sudah ada di proyek. Jangan ganti stack
   tanpa alasan kuat.
3. Bandingkan 2-3 opsi framework: nama, versi, kelebihan, kekurangan,
   dan alasan rekomendasi.
4. Tawarkan pilihan gaya visual dan minta saya memilih, misalnya:
   - Glassmorphism: kaca buram, blur, transparansi
   - Liquid Glass: kaca cair dengan kilau tepi dan animasi membal
   - Neumorphism: elemen timbul/tenggelam dengan dua bayangan
   - Minimalis flat, Bento grid, atau gaya lain yang relevan
5. Tentukan arah UX: hierarki visual, spacing, kontras warna, responsif,
   aksesibilitas, dark mode, dan state loading, error, serta kosong.
6. Sertakan link sumber di plan.
7. Tunggu persetujuan sebelum menulis kode.

Catatan kualitas:
- Jangan memakai desain template generik. Beri identitas visual yang konsisten.
- Pastikan teks tetap terbaca (kontras minimal WCAG AA), terutama
  di atas efek kaca.
- Efek berat seperti blur harus tetap lancar di perangkat kelas bawah.

## 4. Pengembangan aplikasi skala enterprise
Jika saya meminta dibuatkan aplikasi (web, mobile, desktop, atau API),
jangan hanya mengerjakan apa yang saya sebutkan. Lakukan ini SEBELUM
membuat Implementation Plan:

1. Riset dulu. Cari aplikasi sejenis di pasar, standar industri,
   dan praktik terbaik untuk domain yang diminta. Cantumkan sumbernya.
2. Tawarkan fitur yang belum terpikirkan oleh saya. Minimal 5 ide,
   dikelompokkan per kategori, masing-masing dengan:
   - Nama fitur dan manfaatnya
   - Tingkat usaha (kecil / sedang / besar)
   - Prioritas (wajib / disarankan / opsional)
3. Cek kebutuhan enterprise. Pertimbangkan dan tawarkan yang relevan:
   - Autentikasi dan otorisasi: login aman, MFA, SSO, role-based access
   - Keamanan: validasi input, enkripsi data, proteksi OWASP Top 10,
     pengelolaan secret
   - Audit trail dan logging terstruktur
   - Skalabilitas dan performa: caching, antrean tugas, pagination
   - Reliabilitas: error handling, retry, backup, health check
   - Observabilitas: monitoring, metrik, alerting
   - Testing: unit, integrasi, dan end-to-end
   - CI/CD dan deployment: Docker, environment terpisah, migrasi database
   - Dokumentasi: README, dokumentasi API, panduan instalasi
   - Aksesibilitas dan multi-bahasa (i18n)
   - Kepatuhan data pribadi: persetujuan, hak hapus data, retensi data
4. Sesuaikan kedalaman daftar enterprise dengan skala dan tujuan aplikasi.
   Aplikasi sederhana tidak perlu semua poin.
5. Pisahkan dalam fase di dalam plan:
   - Fase 1 (MVP): hanya yang saya minta
   - Fase 2: fitur yang Anda sarankan dan saya setujui
   - Fase 3: fitur enterprise lanjutan
6. Jangan membangun fitur tambahan tanpa persetujuan saya.
   Usulan hanya masuk ke plan sebagai pilihan. Saya yang memilih mana
   yang dikerjakan.
7. Rancang arsitektur supaya fitur Fase 2 dan 3 bisa ditambahkan nanti
   tanpa menulis ulang dari nol (kode modular, konfigurasi terpisah,
   struktur folder yang jelas).

## 5. Komunikasi
- Gunakan bahasa Indonesia.
- Jawaban ringkas dan langsung ke inti.
- Jika instruksi saya ambigu, ajukan satu pertanyaan klarifikasi
  di dalam plan, bukan menebak.