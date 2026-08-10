# Panduan Redesain Website SAMHC (hericahyono.com)

Dokumen ini berfungsi sebagai panduan utama (*master blueprint*) pelaksanaan redesain website **Heri Cahyono (SAMHC)**. Website ini difokuskan sebagai **repositori artikel & berita kegiatan** dengan tampilan yang **elegan, minimalis, dan profesional** berbasis WordPress.

---

## 1. Ringkasan Proyek & Spesifikasi Menu

* **Domain:** `https://hericahyono.com`
* **Tokoh / Brand:** Heri Cahyono (Sam HC)
* **Niche:** Website Personal Branding, Repositori Berita, & Program Inisiatif Sosial
* **Target Tampilan:** Elegan, Minimalis, High-Class Editorial, Fast-Loading
* **CMS Target:** WordPress (menggunakan Block Editor / Gutenberg FSE atau Kadence/Blocksy)
* **Navigasi Header (Menu Utama):**
  1. **Profil** (`/profile/`)
  2. **Blog** (`/berita/`)
  3. **Pusat Curhat Rakyat** (`/pusat-curhat-rakyat/`)
  4. **Bank Ide** (`/bank-ide/`)

---

## 2. Style Guide & Sistem Desain

### A. Skema Warna (*Color Palette*)
| Peran | Nama Warna | Kode Hex | Penggunaan |
| :--- | :--- | :--- | :--- |
| **Background Utama** | Light Warm Gray | `#FAFAFA` | Latar belakang halaman utama |
| **Text Utama** | Deep Charcoal | `#1A1A1A` | Judul, heading, dan teks utama |
| **Text Sekunder** | Slate Gray | `#64748B` | Subtitle, tanggal, metadata, caption |
| **Accent / Highlight** | Warm Amber Gold | `#D97706` | Aksen tombol, badge kategori, hover state |
| **Adventure Dark Theme** | Deep Navy Slate | `#0F172A` | Background khusus kanal "Sam HC Jelajah Bumi" |
| **Card / Surface** | Pure White | `#FFFFFF` | Latar belakang kartu artikel & modal |

### B. Tipografi (*Typography*)
* **Heading (H1, H2, H3):** `Lora` atau `Playfair Display` (Font Serif Editorial yang mencerminkan kedewasaan, wibawa, dan intelektualitas).
* **Body Text & Navigation:** `Plus Jakarta Sans` atau `Inter` (Font Sans-Serif modern yang sangat bersih dan nyaman dibaca).

---

## 3. Wireframe & Alur Konten Halaman Utama (*Homepage Flow*)

```
+-----------------------------------------------------------------------------------+
|  [LOGO SAMHC]        Profil     Blog     Pusat Curhat Rakyat     Bank Ide  [🔍 Cari]| <-- Header (4 Menu Utama)
+-----------------------------------------------------------------------------------+
|                                                                                   |
|  HERO SECTION: FOTO PERSONAL & QUOTE INSPIRATIF                                   |
|  +---------------------------------------+  +----------------------------------+  |
|  |                                       |  |  "SEBUAH KESADARAN"              |  |
|  |  [ FOTO PERSONAL PORTRAIT SAM HC ]    |  |  "Keberhasilan hidup bukan diukur|  |
|  |                                       |  |   dari apa yang kita miliki..."  |  |
|  |                                       |  |  - Heri Cahyono (Sam HC)         |  |
|  |                                       |  |  Bio Singkat & Button CTA        |  |
|  +---------------------------------------+  +----------------------------------+  |
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  SECTION 2: BERITA & KEGIATAN TERBARU                                             |
|  [ 🔍 Input Live Search ]  [ Filter Pills: Semua | Kegiatan | Opini | 2026 ]      |  <-- Live Search & Filter
|  +---------------------+  +---------------------+  +---------------------+        |
|  | [ Foto Artikel 1 ]  |  | [ Foto Artikel 2 ]  |  | [ Foto Artikel 3 ]  |        |
|  | Kunjungan Alumni    |  | Malang City Talents |  | Polemik Parkir      |        |
|  +---------------------+  +---------------------+  +---------------------+        |
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  SECTION 3: KANAL KHUSUS "SAM HC JELAJAH BUMI" (Style Dark Adventure)             |
|  Tajuk: "From Indonesia to See Your Beautiful Country"                            |
|  [ STATS BAR: 14 Negara • 2 Benua • Overland Journey • Misi Persaudaraan ]          |  <-- Travel Stats Bar
|  +---------------------+  +---------------------+  +---------------------+        |
|  | [ Foto Overland 1 ] |  | [ Foto Overland 2 ] |  | [ Foto Overland 3 ] |        |
|  | Asian Overland      |  | Perbatasan 14 Negara|  | Refleksi Kemandirian|        |
|  +---------------------+  +---------------------+  +---------------------+        |
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  SECTION 4: DOKUMENTASI VIDEO HIGHLIGHT                                           |
|  [ Player Video Youtube/TikTok Showcase - Liputan 14 Negara & Kegiatan ]          |  <-- Video Highlight Section
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  SECTION 5: PROGRAM KERJA & INISIATIF SOSIAL                                      |
|  Grid 8 Kartu Program Kerja Mandiri Utama                                         |
|  [ Button CTA: Lihat Seluruh 16 Program Kerja & Inisiatif Sosial → ]               |  <-- Program CTA Button
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  SECTION 6: INTERAKSI WARGA (DUAL BANNER CTA)                                     |
|  +---------------------------------------+  +----------------------------------+  |
|  | PUSAT CURHAT RAKYAT                   |  | BANK IDE RAKYAT                  |  |
|  | Sampaikan keluhan & aspirasimu.       |  | Sumbangkan ide inovatifmu.       |  |
|  | [ Tombol: Tulis Curhatan → ]          |  | [ Tombol: Kirimkan Ide → ]       |  |
|  +---------------------------------------+  +----------------------------------+  |
|                                                                                   |
+-----------------------------------------------------------------------------------+
|  FOOTER: Logo, Navigasi Utama, Legalitas, & Hak Cipta                             |
+-----------------------------------------------------------------------------------+
```

---

## 4. Rincian Fitur & Modul Halaman Utama

1. **Header Navigation:** Ditingkatkan fokusnya menjadi 4 menu utama saja (*Profil, Blog, Pusat Curhat Rakyat, Bank Ide*).
2. **Hero Section:** Foto personal portrait Sam HC + Quote Inspiratif *"Sebuah Kesadaran"*.
3. **Berita & Kegiatan:** Repositori artikel berita terkini dilengkapi dengan **Live AJAX Instant Search Box** dan **Pill Filters** berdasarkan topik/tahun.
4. **Kanal "Sam HC Jelajah Bumi":**
   * **Tajuk Utama:** *"From Indonesia to See Your Beautiful Country"*
   * **Stats Bar:** *14 Negara • 2 Benua • Overland Journey • Misi Persaudaraan*.
   * **Fokus Konten:** Dokumentasi naratif perjalanan *overland* Sam HC berkendara melintasi 14 Negara membawa misi kebudayaan dan persaudaraan antarbangsa.
5. **Dokumentasi Video Highlight:** Block pemutar video YouTube/TikTok embed untuk liputan perjalanan & aksi sosial.
6. **Program Kerja:** Showcase 8 program kerja utama dengan tombol tautan menuju katalog penuh 16 program kerja.
7. **Ruang Interaksi Warga (Dual Banner):** Call-to-Action interaktif untuk penyerapan aspirasi (*Pusat Curhat Rakyat*) dan penampungan gagasan (*Bank Ide*).

---

## 5. Checklist Perbaikan Data & Cleanup WordPress

- [x] **Revisi Header Menu:** Hanya tampilkan Profil, Blog, Pusat Curhat Rakyat, Bank Ide.
- [x] **Penambahan Interaksi Warga:** Dual Banner untuk Curhat Rakyat & Bank Ide di halaman depan.
- [x] **Penambahan Feature Jelajah Bumi:** Tajuk "From Indonesia to See Your Beautiful Country" & Stats Bar 14 Negara.
- [ ] **Koreksi Typo WordPress Title:**
  - `RUmah Dakwah` -> `Rumah Dakwah`
  - `God Mangement School` -> `God Management School`
- [ ] **Koreksi Duplikasi & Image Alt:**
  - Ganti judul "Kampung Duren" kedua menjadi "Pasar Berkeadilan" (sesuai logo `13.logo_pasar_berkeadilan-e.png`).
- [ ] **Pembersihan Dummy Theme Text:**
  - Hapus teks `© 2022 Foxiz News Network. Ruby Design Company...` pada mobile drawer menu.
- [ ] **Ganti Image Placeholder:**
  - Hapus penggunaan image `800x484.png` pada post blog, ganti dengan foto asli kegiatan.

---

## 6. Rekomendasi Tech Stack WordPress (Lightweight & Modern)

* **Theme Base:** Kadence Theme / Blocksy (Versi Gratis/Pro).
* **Page Builder:** Gutenberg / Native Block Editor + Kadence Blocks (Hindari Elementor jika ingin performa maksimal).
* **Plugin Pencarian:** SearchXP / Ivory Search (AJAX Live Search).
* **Optimasi Gambar & Speed:** WP Rocket / LiteSpeed Cache + ShortPixel (auto WebP conversion).
* **SEO:** Rank Math / Yoast SEO.

---
*Dokumen ini diperbarui secara otomatis sesuai instruksi revisi & analisis lengkap desainer.*
