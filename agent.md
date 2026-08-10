# Panduan Redesain Website SAMHC (hericahyono.com)

Dokumen ini berfungsi sebagai panduan utama (*master blueprint*) pelaksanaan redesain website **Heri Cahyono (SAMHC)**. Website ini difokuskan sebagai **repositori artikel & berita kegiatan** dengan tampilan yang **elegan, minimalis, profesional, dan 100% Mobile-Friendly** berbasis WordPress.

---

## 1. Ringkasan Proyek & Spesifikasi Menu

* **Domain:** `https://hericahyono.com`
* **Tokoh / Brand:** Heri Cahyono (Sam HC)
* **Niche:** Website Personal Branding, Repositori Berita, & Program Inisiatif Sosial
* **Target Tampilan:** Elegan, Minimalis, High-Class Editorial, Fast-Loading, Fully Responsive (Mobile First)
* **CMS Target:** WordPress (menggunakan Block Editor / Gutenberg FSE atau Kadence/Blocksy)
* **Navigasi Header (Menu Utama):**
  1. **Profil** (`/profile/`)
  2. **Blog** (`/berita/`)
  3. **Pusat Curhat Rakyat** (`/pusat-curhat-rakyat/`)
  4. **Bank Ide** (`/bank-ide/`)

---

## 2. Style Guide & Sistem Desain Mobile-Friendly

### A. Skema Warna (*Color Palette*)
| Peran | Nama Warna | Kode Hex | Penggunaan |
| :--- | :--- | :--- | :--- |
| **Background Utama** | Light Warm Gray | `#FAFAFA` | Latar belakang halaman utama |
| **Text Utama** | Deep Charcoal | `#1A1A1A` | Judul, heading, dan teks utama |
| **Text Sekunder** | Slate Gray | `#64748B` | Subtitle, tanggal, metadata, caption |
| **Accent / Highlight** | Warm Amber Gold | `#D97706` | Aksen tombol, badge kategori, hover state |
| **Adventure Dark Theme** | Deep Navy Slate | `#0F172A` | Background khusus kanal "Sam HC Jelajah Bumi" |
| **Card / Surface** | Pure White | `#FFFFFF` | Latar belakang kartu artikel & modal |

### B. Tipografi Fluid (*Fluid Typography*)
* **Heading (H1, H2, H3):** `Lora` atau `Playfair Display` dengan CSS `clamp(22px, 3.5vw, 34px)` agar ukuran font otomatis menyesuaikan lebar layar smartphone hingga desktop tanpa merusak layout.
* **Body Text & Navigation:** `Plus Jakarta Sans` atau `Inter` (Font Sans-Serif modern yang sangat bersih, mudah dibaca, dan berbobot ringan di HP).

---

## 3. Optimasi Responsif Mobile (*Mobile Responsive Architecture*)

```
DESKTOP VIEW (Width > 900px)                 MOBILE VIEW (Width <= 900px)
+-------------------------------+             +-------------------------------+
| LOGO     Menu Links     Search|             | LOGO                  [ ☰ ]  |  <-- Mobile Hamburger
+-------------------------------+             +-------------------------------+
| Hero (Foto Left | Quote Right)|             | [ ☰ Drawer ]  Menu Dropdown   |
| 3-Column News Grid            |  =========> | Hero Photo (280px-320px)      |
| 4-Column Overland Stats Bar   |             | Quote + Full-Width Buttons    |
| 4-Column Program Grid         |             | 1-Column News Grid Stack      |
| Dual-Banner 2-Column Side     |             | Horizontal Scroll Filter Pills|
+-------------------------------+             | 2x2 Stats Bar Grid            |
                                              | 2/1-Column Program Grid       |
                                              | Full-Width Dual Banner Stack  |
                                              +-------------------------------+
```

### Key Mobile Enhancements:
1. **Header Navigation Drawer:** Tombol Hamburger `☰` otomatis muncul di layar HP. Ketika diklik, menampilkan drawer navigasi halus berisi 4 menu utama + pencarian.
2. **Horizontal Scroll Filter Pills:** Filter kategori berita di HP dapat digeser secara horizontal (*native touch drag*) tanpa memakan banyak tempat vertikal.
3. **Stacked Hero CTA:** Tombol CTA (*Kenal Lebih Dekat* & *Pusat Curhat Rakyat*) berubah menjadi 100% lebar layar di HP agar mudah ditap dengan jempol (*thumb-friendly*).
4. **Adaptive Stats & Program Grid:** Bar statistik 14 negara beradaptasi menjadi grid 2x2 pada layar HP. Grid Program Kerja menyesuaikan dari 4 kolom menjadi 2 atau 1 kolom.

---

## 4. Wireframe & Alur Konten Halaman Utama (*Homepage Flow*)

1. **Header (Mobile Drawer Enabled):** Logo SAMHC, 4 Menu Utama, Mobile Toggle `☰`.
2. **Hero Section:** Portrait Photo Sam HC + Quote Inspiratif *"Sebuah Kesadaran"* + Tombol CTA.
3. **Berita & Kegiatan Terbaru:** Repositori artikel berita terkini dengan **Live Instant Search** & **Touch Horizontal Filter Pills**.
4. **Kanal "Sam HC Jelajah Bumi":**
   * **Tajuk Utama:** *"From Indonesia to See Your Beautiful Country"*
   * **Stats Bar Mobile Grid (2x2):** *14 Negara • 2 Benua • Overland Journey • Misi Persaudaraan*.
   * **Artikel Overland:** Catatan perjalanan melintasi 14 Negara.
5. **Dokumentasi Video Highlight:** Pemutar video YouTube/TikTok embed yang *responsive height*.
6. **Program Kerja:** Grid kartu 8 program utama + Tombol CTA ke katalog penuh 16 program.
7. **Ruang Interaksi Warga (Dual Banner Stack):** Banner aspirasi (*Pusat Curhat Rakyat*) & gagasan (*Bank Ide*).

---

## 5. Checklist Perbaikan Data & Cleanup WordPress

- [x] **Revisi Header Menu:** Hanya tampilkan Profil, Blog, Pusat Curhat Rakyat, Bank Ide.
- [x] **Optimasi Mobile Friendly:** Drawer Mobile Menu, Responsive Spacing, Fluid Typography, Touch Scroll Pills.
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

## 6. Rekomendasi Tech Stack WordPress (Lightweight & Mobile-Optimized)

* **Theme Base:** Kadence Theme / Blocksy (Sangat responsive & mendukung mobile menu custom bawaan).
* **Page Builder:** Gutenberg / Native Block Editor + Kadence Blocks (Performa mobile tercepat tanpa bloated code).
* **Plugin Pencarian:** SearchXP / Ivory Search (AJAX Live Search).
* **Optimasi Gambar & Speed:** WP Rocket / LiteSpeed Cache + ShortPixel (auto WebP conversion).
* **SEO:** Rank Math / Yoast SEO.

---
*Dokumen ini diperbarui secara otomatis sesuai instruksi optimasi versi Mobile Friendly.*
