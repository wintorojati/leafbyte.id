# LeafByte Prima Nusantara — Landing Page

Perusahaan teknologi Indonesia yang tumbuh dengan semangat keberlanjutan, menghadirkan solusi digital unggul bagi masyarakat Nusantara.

Tagline: "Technology That Grows, Solutions That Thrive"

## Struktur
- `index.html` — Halaman utama
- `styles.css` — Styling modern & responsif
- `LeafByteId.png` — Logo/identitas visual
- `CNAME` — Konfigurasi domain custom untuk GitHub Pages (leafbyte.id)

## Cara Menjalankan Lokal
Cukup buka `index.html` di browser.

## Deploy ke GitHub Pages
1. Buat repository baru di GitHub (misal: `leafbyte.id` atau nama lain).
2. Commit & push file berikut ke root repo: `index.html`, `styles.css`, `LeafByteId.png`, `CNAME`, `README.md`.
3. Buka Settings → Pages → Build and deployment:
   - Source: "Deploy from a branch"
   - Branch: `main` / folder `/ (root)`
4. Bagian Custom domain: isi dengan `leafbyte.id` lalu Save. (Langkah ini biasanya membuat file `CNAME` otomatis. Karena kita sudah menyediakan `CNAME`, Anda bisa langsung Save.)
5. Aktifkan "Enforce HTTPS" jika sudah tersedia.

### Konfigurasi DNS
Tambahkan record di DNS provider domain `leafbyte.id`:
- APEX/root domain (leafbyte.id):
  - A 185.199.108.153
  - A 185.199.109.153
  - A 185.199.110.153
  - A 185.199.111.153
- Subdomain `www` (opsional, direkomendasikan):
  - CNAME `www` → `<username>.github.io`

Catatan:
- Ganti `<username>` dengan username GitHub Anda.
- Jika DNS mendukung ALIAS/ANAME untuk root, Anda bisa arahkan root `leafbyte.id` langsung ke `<username>.github.io` via ALIAS/ANAME sebagai alternatif A records.
- Setelah DNS dan Pages terset, propagasi bisa memerlukan waktu hingga 30 menit.

## Kustomisasi
- Ubah link kontak di bagian "Kontak" pada `index.html` (mis. `mailto:hello@leafbyte.id`).
- Perbarui logo `LeafByteId.png` jika dibutuhkan.
- Tambah bagian/section lain sesuai kebutuhan.

Jika ingin saya bantu otomatisasi deploy (GitHub Actions) atau menambahkan formulir kontak, beri tahu saya.
