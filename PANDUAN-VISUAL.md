# 📸 PANDUAN VISUAL - Instrumen Monitoring dan Evaluasi

Panduan visual untuk memahami tampilan dan cara menggunakan sistem

---

## 🏠 HALAMAN UTAMA

### Tampilan Navigasi

```
┌─────────────────────────────────────────────────────────────────┐
│  [Form Evaluasi]  [Login Dashboard]        Jumat, 14 Nov 2024  │
└─────────────────────────────────────────────────────────────────┘
```

**Fungsi:**
- **Form Evaluasi**: Halaman untuk mengisi evaluasi
- **Login Dashboard**: Akses dashboard pimpinan (butuh password)
- **Tanggal**: Menampilkan tanggal hari ini

---

## 📝 HALAMAN FORM EVALUASI

### 1. Header

```
╔════════════════════════════════════════════════════════════════╗
║     INSTRUMEN MONITORING DAN EVALUASI                          ║
║     Penyelarasan Visi dan Misi dengan Pembelajaran Mendalam    ║
║     SMP Negeri 38 Maluku Tengah                               ║
╚════════════════════════════════════════════════════════════════╝
```

### 2. Informasi Evaluator

```
┌────────────────┬────────────────────┬────────────────────┐
│   Tanggal      │  Nama Evaluator    │    Jabatan         │
│  [14-11-2024]  │  [Input nama...]   │  [Pilih jabatan ▼] │
└────────────────┴────────────────────┴────────────────────┘
```

**Pilihan Jabatan:**
- Kepala Sekolah
- Wakil Kepala Sekolah
- Ketua Komite
- Pengawas
- Tim Monev
- Lainnya

### 3. Aspek Penilaian (Contoh 1 Aspek)

```
┌─────────────────────────────────────────────────────────────────┐
│ 1. Penerapan Visi dan Misi dalam Pembelajaran                  │
│ Sejauh mana visi dan misi sekolah diintegrasikan dalam         │
│ proses pembelajaran sehari-hari                                │
│                                                                 │
│ ○ 1  ○ 2  ○ 3  ○ 4  ○ 5     [Belum dinilai]                  │
└─────────────────────────────────────────────────────────────────┘
```

**Keterangan Skor:**
- ○ 1 = Sangat Kurang
- ○ 2 = Kurang  
- ○ 3 = Cukup
- ○ 4 = Baik
- ○ 5 = Sangat Baik

**Status akan berubah warna sesuai skor:**
- Merah (1-2): Kurang
- Kuning (3): Cukup
- Biru (4): Baik
- Hijau (5): Sangat Baik

### 4. Hasil Evaluasi (Real-time)

```
┌──────────────────────────────────────────────────────────────┐
│                    HASIL EVALUASI                            │
├──────────────┬──────────────┬──────────────────────────────┤
│ Total Skor   │ Persentase   │         Kategori             │
│   35/40      │    87.5%     │    🟢 SANGAT BAIK            │
└──────────────┴──────────────┴──────────────────────────────┘
```

**Perhitungan Otomatis:**
- Total Skor: Jumlah semua aspek
- Persentase: (Total Skor / Maks Skor) × 100%
- Kategori: Berdasarkan persentase

### 5. Catatan dan Rekomendasi

```
┌─────────────────────────────────────────────────────────────┐
│ Catatan dan Rekomendasi                                     │
│ ┌─────────────────────────────────────────────────────────┐ │
│ │ Tuliskan catatan, temuan, atau rekomendasi perbaikan... │ │
│ │                                                         │ │
│ │                                                         │ │
│ └─────────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────┘
```

### 6. Tombol Aksi

```
┌─────────────────────────────┬──────────┐
│   [Simpan Evaluasi]         │  [Reset] │
└─────────────────────────────┴──────────┘
```

**Fungsi:**
- **Simpan Evaluasi**: Submit data ke Google Sheets
- **Reset**: Mengosongkan form dan mulai dari awal

### 7. Notifikasi Sukses

```
┌─────────────────────────────────────────────────────────────┐
│ ✓ Data berhasil disimpan! Skor: 87.5% (Sangat Baik)       │
└─────────────────────────────────────────────────────────────┘
```

---

## 🔐 HALAMAN LOGIN DASHBOARD

### Tampilan Login

```
╔═══════════════════════════════════════════════════════════╗
║                                                           ║
║               Dashboard Pimpinan                          ║
║           SMP Negeri 38 Maluku Tengah                     ║
║                                                           ║
║  ┌─────────────────────────────────────────────┐         ║
║  │ Password                                     │         ║
║  │ [●●●●●●●●]                                  │         ║
║  └─────────────────────────────────────────────┘         ║
║                                                           ║
║            [ Login ]                                      ║
║                                                           ║
║  Hanya untuk pimpinan sekolah yang berwenang             ║
╚═══════════════════════════════════════════════════════════╝
```

**Password:** `SMPN38MT`

---

## 📊 HALAMAN DASHBOARD PIMPINAN

### 1. Header Dashboard

```
┌────────────────────────────────────────────────────────────┐
│ Dashboard Pimpinan                           [Logout]      │
│ SMP Negeri 38 Maluku Tengah                               │
└────────────────────────────────────────────────────────────┘
```

### 2. Statistik Cards

```
┌──────────────┬──────────────┬──────────────┬──────────────┐
│ Total        │ Rata-rata    │ Skor         │ Skor         │
│ Evaluasi     │ Skor         │ Tertinggi    │ Terendah     │
│              │              │              │              │
│    3         │   75.00%     │   87.50%     │   65.00%     │
│                                                           │
└──────────────┴──────────────┴──────────────┴──────────────┘
```

**Warna Cards:**
- Biru: Total Evaluasi
- Hijau: Rata-rata Skor
- Ungu: Skor Tertinggi
- Orange: Skor Terendah

### 3. Filter Kategori

```
┌─────────────────────────────────────────────┐
│ Filter Kategori: [Semua ▼]                  │
└─────────────────────────────────────────────┘
```

**Pilihan:**
- Semua
- Sangat Baik
- Baik
- Cukup
- Kurang

### 4. Tabel Data Evaluasi

```
┌───┬────────────┬─────────────────┬───────────┬──────┬────────┬──────────────┐
│No │ Tanggal    │ Evaluator       │ Jabatan   │ Skor │ %      │ Kategori     │
├───┼────────────┼─────────────────┼───────────┼──────┼────────┼──────────────┤
│ 1 │ 2024-11-01 │ Dr. Ahmad H.    │ Kepsek    │35/40 │ 87.50% │ 🟢 Sangat Baik│
│ 2 │ 2024-11-05 │ Siti N., M.Pd   │ Wakasek   │29/40 │ 72.50% │ 🔵 Baik      │
│ 3 │ 2024-11-10 │ Budi Santoso    │ Pengawas  │26/40 │ 65.00% │ 🟡 Cukup     │
└───┴────────────┴─────────────────┴───────────┴──────┴────────┴──────────────┘
```

**Fitur Tabel:**
- Hover untuk highlight baris
- Badge warna untuk kategori
- Data real-time dari Google Sheets

### 5. Link Google Sheets

```
┌─────────────────────────────────────────────────────────────┐
│ 📊 Akses Google Sheets                                      │
│ Data evaluasi tersimpan di Google Sheets dengan ID:        │
│ 1rCQKqknWFLz3dzl_zokATkUj8OITXjBikicn_GnaLU4              │
│                                                             │
│ [ Buka Google Sheets ]                                     │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎨 SKEMA WARNA

### Kategori Hasil

| Kategori | Warna | Badge |
|----------|-------|-------|
| Sangat Baik | Hijau | 🟢 |
| Baik | Biru | 🔵 |
| Cukup | Kuning | 🟡 |
| Kurang | Merah | 🔴 |
| Sangat Kurang | Merah Gelap | ⚫ |

### Elemen UI

| Elemen | Warna |
|--------|-------|
| Header | Gradient Ungu-Biru |
| Button Primary | Gradient Ungu |
| Button Secondary | Abu-abu |
| Success | Hijau |
| Warning | Kuning |
| Error | Merah |
| Info | Biru |

---

## 📱 RESPONSIVE DESIGN

### Desktop (>1024px)
- Form: 2-3 kolom untuk informasi evaluator
- Dashboard: 4 cards statistik dalam 1 baris
- Tabel: Full width dengan semua kolom

### Tablet (768px - 1024px)
- Form: 2 kolom
- Dashboard: 2 cards per baris
- Tabel: Scrollable horizontal

### Mobile (<768px)
- Form: 1 kolom, stack vertical
- Dashboard: 1 card per baris, stack vertical
- Tabel: Scrollable horizontal dengan kolom minimal

---

## 🔔 NOTIFIKASI

### Tipe Notifikasi

**Success (Hijau)**
```
┌─────────────────────────────────────────────┐
│ ✓ Data berhasil disimpan!                  │
└─────────────────────────────────────────────┘
```

**Error (Merah)**
```
┌─────────────────────────────────────────────┐
│ ✗ Gagal menyimpan data. Coba lagi.         │
└─────────────────────────────────────────────┘
```

**Info (Biru)**
```
┌─────────────────────────────────────────────┐
│ ℹ Mohon lengkapi semua aspek penilaian     │
└─────────────────────────────────────────────┘
```

**Posisi:** Kanan atas layar
**Durasi:** 3 detik (auto close)

---

## 🖱️ INTERAKSI USER

### Hover Effects
- Button: Opacity berubah, cursor pointer
- Tabel row: Background abu-abu muda
- Radio button: Scale sedikit membesar

### Loading States
- Submit: Button disabled + text "Menyimpan..."
- Dashboard: Spinner loading + text "Memuat data..."

### Validation
- Field wajib: Border merah jika kosong
- Password salah: Border merah + pesan error
- Form lengkap: Button aktif

---

## 📊 GOOGLE SHEETS DASHBOARD

### Tab "Data Evaluasi"
```
┌──────────────┬─────────┬──────────────┬─────────┬─────────┐
│ Timestamp    │ Tanggal │ Evaluator    │ Jabatan │ Aspek 1 │ ...
├──────────────┼─────────┼──────────────┼─────────┼─────────┤
│ 2024-11-01...│ 11/01   │ Dr. Ahmad    │ Kepsek  │    5    │ ...
│ 2024-11-05...│ 11/05   │ Siti N.      │ Wakasek │    4    │ ...
└──────────────┴─────────┴──────────────┴─────────┴─────────┘
```

### Tab "Dashboard"
```
┌──────────────────────────────────────┐
│ DASHBOARD MONITORING DAN EVALUASI    │
│ SMP Negeri 38 Maluku Tengah         │
├──────────────────────────────────────┤
│ STATISTIK KESELURUHAN                │
│ Total Evaluasi:        3             │
│ Rata-rata Persentase:  75.00%        │
│ Skor Tertinggi:        87.50%        │
│ Skor Terendah:         65.00%        │
├──────────────────────────────────────┤
│ DISTRIBUSI KATEGORI                  │
│ Sangat Baik:          1              │
│ Baik:                 1              │
│ Cukup:                1              │
│ Kurang:               0              │
├──────────────────────────────────────┤
│ RATA-RATA PER ASPEK                  │
│ Penerapan Visi Misi:     4.00        │
│ Keselarasan Kurikulum:   4.00        │
│ Metode Pembelajaran:     3.67        │
│ ... (8 aspek)                        │
└──────────────────────────────────────┘
```

---

## 💡 TIPS VISUAL

### Untuk Evaluator
1. **Gunakan indikator warna** untuk memahami status penilaian
2. **Perhatikan hasil real-time** saat mengisi form
3. **Lihat kategori** untuk mengetahui level capaian
4. **Gunakan catatan** untuk detail penting

### Untuk Pimpinan
1. **Cards statistik** untuk overview cepat
2. **Filter kategori** untuk analisis spesifik
3. **Tabel sortable** untuk detail per evaluasi
4. **Google Sheets** untuk analisis mendalam

---

## 🎯 BEST PRACTICES UI/UX

1. **Konsistensi Visual**: Warna dan layout konsisten
2. **Clear Navigation**: Mudah berpindah antar halaman
3. **Feedback Cepat**: Notifikasi langsung setelah aksi
4. **Mobile Friendly**: Responsive di semua ukuran layar
5. **Accessibility**: Kontras warna yang baik
6. **Loading States**: User tahu sistem sedang proses
7. **Error Handling**: Pesan error yang jelas dan membantu

---

**💡 Catatan:** Tampilan visual dapat sedikit berbeda tergantung browser dan resolusi layar yang digunakan.
