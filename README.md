# Undangan Wisuda (Elegan Hitam–Gold)

## Cara pakai
1. Buka `index.html`, cari teks dalam tanda kurung siku seperti `[Nama Wisudawan/i]`, `[Hari, Tanggal Bulan Tahun]`, `[Nama Gedung/Rumah]`, dll — ganti dengan data asli Anda.
2. Ganti link Google Maps: cari lokasi Anda di Google Maps, klik "Bagikan" → "Sematkan peta", salin bagian `src="..."` ke `iframe` di bagian PETA LOKASI. Ganti juga link "BUKA DI GOOGLE MAPS".
3. Foto galeri: ganti setiap `<div class="ph">...</div>` di bagian GALERI dengan `<img src="foto1.jpg" alt="...">`, lalu taruh file foto di folder yang sama.
4. Musik: taruh file `musik.mp3` (instrumental milik Anda sendiri / royalty-free) di folder yang sama, sejajar dengan `index.html`.
5. Form ucapan saat ini hanya menyimpan ucapan di browser tamu masing-masing (localStorage), belum terkirim ke Anda. Untuk menerima semua ucapan tamu ke email/dashboard, daftar gratis di formspree.io, lalu ikuti komentar di dalam `<script>` pada `index.html` untuk menyambungkannya.

## Deploy ke Vercel
**Cara termudah (tanpa install apa pun):**
1. Buka https://vercel.com → New Project → Deploy → pilih "Deploy without Git" / drag & drop folder ini (semua file dalam folder `undangan-project`).
2. Tunggu proses build selesai, Vercel akan memberi Anda link seperti `https://nama-project.vercel.app`.

**Cara via CLI (jika sudah punya Node.js):**
```
npm i -g vercel
cd undangan-project
vercel --prod
```

Situs ini murni HTML/CSS/JS statis, jadi 100% kompatibel dengan hosting statis Vercel — tidak perlu konfigurasi build khusus.
