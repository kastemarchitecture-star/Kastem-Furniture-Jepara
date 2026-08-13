# Kastem Furniture Jepara — Landing Page

Situs satu halaman, siap pakai. Tidak perlu build step, tidak ada dependency server — cukup file statis (HTML + CSS + JS + gambar).

## Isi folder
```
index.html        ← halaman utama (semua CSS & JS ada di dalamnya)
assets/            ← 17 foto asli dari katalog PDF Kastem Furniture 2027
README.md          ← file ini
```

## Cara deploy (pilih salah satu, semuanya gratis)

### Opsi A — Netlify (paling cepat, drag & drop)
1. Buka https://app.netlify.com/drop
2. Seret seluruh folder `kastem-furniture-jepara` ke halaman itu
3. Selesai — dapat link `https://nama-acak.netlify.app` dalam hitungan detik
4. Bisa sambungkan domain sendiri (misal `kastemfurniturejepara.com`) lewat menu Domain settings

### Opsi B — Vercel
1. Buat akun di https://vercel.com
2. Pilih "Add New Project" → "Deploy without Git" / upload folder
3. Deploy — Vercel otomatis kasih link

### Opsi C — GitHub Pages
1. Upload isi folder ini ke repository GitHub baru
2. Masuk ke Settings → Pages → pilih branch `main` folder `/root`
3. Situs aktif di `https://username.github.io/nama-repo`

### Opsi D — Hosting cPanel / domain sendiri
1. Login ke cPanel / File Manager hosting Anda
2. Upload seluruh isi folder ini ke folder `public_html`
3. Selesai — situs langsung aktif di domain Anda

## Yang sudah terhubung otomatis
- **Tombol WhatsApp** (di navbar, hero, tiap koleksi, dan tombol mengambang) langsung membuka chat ke **+62 821-4777-7570** dengan pesan otomatis:
  > "halo, beri saya informasi tentang kastem furniture jepara"
- Tombol kategori (Meja, Kursi, dst.) mengirim pesan yang sama plus nama kategori, supaya tim langsung tahu produk yang ditanyakan.

## Mengubah nomor WhatsApp atau pesan otomatis
Cari kata `6282147777570` di `index.html` (muncul 7 kali) dan ganti dengan nomor baru dalam format `62` + nomor tanpa angka 0 di depan.
Untuk mengubah pesan otomatis, cari `BASE_MSG` di bagian `<script>` paling bawah dan tag `text=halo%2C...` di setiap tombol WhatsApp.

## Catatan
- Semua foto diambil langsung dari katalog PDF resmi (edisi 2027) — bukan foto stok.
- Font dimuat dari Google Fonts (Archivo Black, Fraunces, Inter) — perlu koneksi internet saat halaman dibuka.
