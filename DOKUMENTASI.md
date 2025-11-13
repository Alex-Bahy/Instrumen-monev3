# DOKUMENTASI SISTEM MONITORING DAN EVALUASI
## Penyelarasan Visi dan Misi dengan Pembelajaran Mendalam
### SMP Negeri 38 Maluku Tengah

---

## 📋 DAFTAR ISI

1. [Gambaran Umum](#gambaran-umum)
2. [Fitur Utama](#fitur-utama)
3. [Panduan Setup Google Sheets](#panduan-setup-google-sheets)
4. [Panduan Penggunaan](#panduan-penggunaan)
5. [Aspek Penilaian](#aspek-penilaian)
6. [Interpretasi Hasil](#interpretasi-hasil)
7. [FAQ](#faq)
8. [Troubleshooting](#troubleshooting)

---

## 🎯 GAMBARAN UMUM

Sistem Instrumen Monitoring dan Evaluasi ini dirancang untuk membantu SMP Negeri 38 Maluku Tengah dalam:

- Mengevaluasi penyelarasan visi dan misi sekolah dengan praktik pembelajaran
- Memantau implementasi pembelajaran mendalam (deep learning)
- Memberikan data berbasis bukti untuk pengambilan keputusan
- Memfasilitasi perbaikan berkelanjutan

### Komponen Sistem

1. **Form Evaluasi**: Interface untuk melakukan evaluasi
2. **Dashboard Pimpinan**: Panel kontrol untuk melihat hasil (password protected)
3. **Google Sheets**: Database untuk penyimpanan dan analisis data

---

## ✨ FITUR UTAMA

### 1. Form Evaluasi
- 8 aspek penilaian komprehensif
- Skala penilaian 1-5 (Sangat Kurang - Sangat Baik)
- Perhitungan otomatis skor dan persentase
- Kategori hasil evaluasi otomatis
- Field catatan untuk rekomendasi

### 2. Dashboard Pimpinan
- Statistik keseluruhan (total evaluasi, rata-rata, tertinggi, terendah)
- Filter berdasarkan kategori
- Tabel data lengkap
- Password protection: **SMPN38MT**

### 3. Integrasi Google Sheets
- Penyimpanan data otomatis
- ID Sheet: `1rCQKqknWFLz3dzl_zokATkUj8OITXjBikicn_GnaLU4`
- Dashboard otomatis dengan formula
- Laporan bulanan

---

## 🔧 PANDUAN SETUP GOOGLE SHEETS

### Langkah 1: Persiapan Google Sheets

1. Buka Google Sheets dengan ID: `1rCQKqknWFLz3dzl_zokATkUj8OITXjBikicn_GnaLU4`
2. Atau buat sheet baru dengan struktur yang sama

### Langkah 2: Membuat Sheet "Data Evaluasi"

Buat sheet dengan nama **"Data Evaluasi"** dan kolom berikut:

| Kolom | Nama Field | Keterangan |
|-------|------------|------------|
| A | Timestamp | Waktu pengisian otomatis |
| B | Tanggal | Tanggal evaluasi |
| C | Nama Evaluator | Nama lengkap evaluator |
| D | Jabatan | Jabatan evaluator |
| E | Aspek 1: Penerapan Visi Misi | Skor 1-5 |
| F | Aspek 2: Keselarasan Kurikulum | Skor 1-5 |
| G | Aspek 3: Metode Pembelajaran | Skor 1-5 |
| H | Aspek 4: Pengembangan Kompetensi | Skor 1-5 |
| I | Aspek 5: Penilaian Autentik | Skor 1-5 |
| J | Aspek 6: Sarana Prasarana | Skor 1-5 |
| K | Aspek 7: Keterlibatan Stakeholder | Skor 1-5 |
| L | Aspek 8: Budaya Sekolah | Skor 1-5 |
| M | Total Skor | Jumlah skor |
| N | Maksimal Skor | Skor maksimal (40) |
| O | Persentase | Persentase capaian |
| P | Kategori | Kategori hasil |
| Q | Catatan | Catatan dan rekomendasi |

### Langkah 3: Setup Google Apps Script

1. Di Google Sheets, klik **Extensions** → **Apps Script**
2. Copy paste kode dari file `google-apps-script.js`
3. Simpan dengan nama "Monitoring Evaluasi Script"
4. Klik **Run** → Pilih fungsi `setupSheet`
5. Berikan izin akses yang diperlukan
6. Jalankan fungsi `setupDashboard` untuk membuat dashboard

### Langkah 4: Deploy Web App (Untuk Integrasi Real-time)

1. Di Apps Script Editor, klik **Deploy** → **New deployment**
2. Pilih **Web app**
3. Atur:
   - Description: "Monitoring Evaluasi API"
   - Execute as: Me
   - Who has access: Anyone
4. Klik **Deploy**
5. Copy URL Web App yang dihasilkan
6. Update URL di file HTML (bagian submit form)

### Langkah 5: Test Integrasi

1. Buka file `monitoring-evaluasi.html`
2. Isi form evaluasi
3. Submit data
4. Cek apakah data masuk ke Google Sheets

---

## 📖 PANDUAN PENGGUNAAN

### Untuk Evaluator

#### A. Mengisi Form Evaluasi

1. **Buka aplikasi** `monitoring-evaluasi.html` di browser
2. **Isi Informasi Evaluator**:
   - Tanggal evaluasi
   - Nama lengkap
   - Jabatan (pilih dari dropdown)

3. **Berikan Penilaian** untuk setiap aspek:
   - Baca deskripsi aspek dengan teliti
   - Pilih skor 1-5 sesuai kondisi aktual
   - Lihat kategori otomatis untuk setiap aspek

4. **Perhatikan Hasil Evaluasi**:
   - Total skor otomatis terhitung
   - Persentase capaian ditampilkan
   - Kategori hasil muncul otomatis

5. **Tambahkan Catatan**:
   - Tulis temuan penting
   - Berikan rekomendasi perbaikan
   - Catat hal-hal yang perlu tindak lanjut

6. **Submit**:
   - Klik tombol "Simpan Evaluasi"
   - Tunggu konfirmasi berhasil
   - Data otomatis tersimpan di Google Sheets

#### B. Skala Penilaian

| Skor | Kategori | Kriteria |
|------|----------|----------|
| 5 | Sangat Baik | Implementasi optimal, sistematis, dan berkelanjutan |
| 4 | Baik | Implementasi baik dengan beberapa aspek yang perlu ditingkatkan |
| 3 | Cukup | Implementasi dasar terpenuhi namun perlu banyak perbaikan |
| 2 | Kurang | Implementasi minimal dan belum sistematis |
| 1 | Sangat Kurang | Belum ada implementasi atau sangat tidak memadai |

### Untuk Pimpinan Sekolah

#### A. Mengakses Dashboard

1. **Klik "Login Dashboard"** di menu navigasi
2. **Masukkan password**: `SMPN38MT`
3. **Dashboard terbuka** menampilkan:
   - Statistik keseluruhan
   - Tabel data evaluasi
   - Filter berdasarkan kategori

#### B. Menganalisis Data

1. **Statistik Keseluruhan**:
   - Total Evaluasi: Jumlah evaluasi yang telah dilakukan
   - Rata-rata Skor: Performa keseluruhan
   - Skor Tertinggi & Terendah: Rentang capaian

2. **Filter Data**:
   - Gunakan dropdown kategori
   - Lihat evaluasi per kategori hasil
   - Identifikasi area yang perlu perhatian

3. **Analisis Tren**:
   - Buka Google Sheets untuk analisis lebih dalam
   - Lihat perkembangan dari waktu ke waktu
   - Identifikasi pola dan tren

#### C. Mengakses Google Sheets

1. Klik link **"Buka Google Sheets"** di dashboard
2. Atau buka langsung: 
   ```
   https://docs.google.com/spreadsheets/d/1rCQKqknWFLz3dzl_zokATkUj8OITXjBikicn_GnaLU4/edit
   ```
3. Lihat tab **"Dashboard"** untuk ringkasan
4. Lihat tab **"Data Evaluasi"** untuk data lengkap

---

## 📊 ASPEK PENILAIAN

### 1. Penerapan Visi dan Misi dalam Pembelajaran

**Fokus Evaluasi:**
- Integrasi visi misi dalam RPP
- Implementasi dalam proses pembelajaran
- Pemahaman guru dan siswa tentang visi misi
- Konsistensi penerapan di semua mata pelajaran

**Indikator Sangat Baik (Skor 5):**
- Visi misi terintegrasi di semua RPP
- Guru dan siswa memahami dan menerapkan
- Ada bukti konkret implementasi
- Evaluasi berkala dilakukan

### 2. Keselarasan Kurikulum dengan Visi Misi

**Fokus Evaluasi:**
- Kesesuaian struktur kurikulum
- Muatan lokal yang relevan
- Kegiatan pengembangan diri
- Program khusus yang mendukung visi misi

**Indikator Sangat Baik (Skor 5):**
- Kurikulum dirancang selaras visi misi
- Muatan lokal mendukung pencapaian
- Program pengembangan diri terstruktur
- Ada inovasi kurikulum

### 3. Metode Pembelajaran Mendalam (Deep Learning)

**Fokus Evaluasi:**
- Penggunaan metode pembelajaran aktif
- Pendekatan konstruktivisme
- Higher Order Thinking Skills (HOTS)
- Project-based dan problem-based learning
- Kolaborasi dan komunikasi

**Indikator Sangat Baik (Skor 5):**
- Metode pembelajaran bervariasi
- Siswa aktif dan terlibat
- HOTS terintegrasi dalam pembelajaran
- Ada proyek nyata yang bermakna

### 4. Pengembangan Kompetensi Siswa

**Fokus Evaluasi:**
- Kompetensi akademik
- Kompetensi non-akademik (soft skills)
- Kreativitas dan inovasi
- Karakter dan nilai-nilai
- Kecakapan abad 21

**Indikator Sangat Baik (Skor 5):**
- Program pengembangan komprehensif
- Keseimbangan akademik dan non-akademik
- Pencapaian prestasi siswa meningkat
- Kompetensi terukur dan terdokumentasi

### 5. Penilaian Autentik

**Fokus Evaluasi:**
- Variasi metode penilaian
- Penilaian berbasis kinerja
- Portfolio siswa
- Penilaian formatif dan sumatif
- Feedback yang konstruktif

**Indikator Sangat Baik (Skor 5):**
- Penilaian holistik (kognitif, afektif, psikomotor)
- Menggunakan rubrik yang jelas
- Portfolio terdokumentasi dengan baik
- Feedback mendorong perbaikan

### 6. Sarana dan Prasarana Pembelajaran

**Fokus Evaluasi:**
- Ketersediaan fasilitas
- Kondisi dan kualitas
- Pemanfaatan optimal
- Inovasi penggunaan
- Aksesibilitas

**Indikator Sangat Baik (Skor 5):**
- Fasilitas lengkap dan layak
- Pemanfaatan optimal dan efektif
- Pemeliharaan rutin dilakukan
- Ada inovasi penggunaan teknologi

### 7. Keterlibatan Stakeholder

**Fokus Evaluasi:**
- Partisipasi guru dalam pengembangan
- Keterlibatan siswa dalam pengambilan keputusan
- Peran orang tua dan komite
- Kerjasama dengan masyarakat
- Komunikasi yang efektif

**Indikator Sangat Baik (Skor 5):**
- Semua stakeholder terlibat aktif
- Komunikasi dua arah berjalan baik
- Program melibatkan stakeholder
- Ada bukti kontribusi nyata

### 8. Budaya Sekolah

**Fokus Evaluasi:**
- Iklim pembelajaran positif
- Budaya kolaborasi
- Nilai-nilai yang dianut
- Kebiasaan positif
- Lingkungan kondusif

**Indikator Sangat Baik (Skor 5):**
- Iklim sekolah sangat kondusif
- Budaya kolaborasi kuat
- Nilai-nilai tertanam dalam keseharian
- Inovasi dan kreativitas berkembang

---

## 📈 INTERPRETASI HASIL

### Kategori Hasil Evaluasi

| Persentase | Kategori | Interpretasi | Rekomendasi |
|------------|----------|--------------|-------------|
| 85% - 100% | Sangat Baik | Penyelarasan visi misi dengan pembelajaran mendalam sangat optimal. Praktik terbaik dapat dijadikan model. | Pertahankan dan tingkatkan. Dokumentasikan best practices untuk disebarluaskan. |
| 70% - 84% | Baik | Penyelarasan berjalan baik dengan beberapa aspek yang perlu perbaikan. | Identifikasi aspek dengan skor rendah dan buat rencana perbaikan spesifik. |
| 55% - 69% | Cukup | Penyelarasan dasar terpenuhi namun banyak aspek perlu peningkatan signifikan. | Lakukan analisis mendalam, buat program perbaikan terstruktur dengan timeline jelas. |
| 40% - 54% | Kurang | Penyelarasan belum optimal, perlu intervensi segera. | Prioritaskan perbaikan pada aspek kritis, libatkan semua stakeholder, monitoring intensif. |
| < 40% | Sangat Kurang | Penyelarasan sangat minim, memerlukan redesain sistem. | Evaluasi menyeluruh visi misi dan sistem pembelajaran, buat rencana transformasi komprehensif. |

### Analisis Hasil

#### 1. Analisis Per Aspek
- Identifikasi aspek dengan skor terendah
- Cari pola atau tren dari evaluasi berbeda
- Bandingkan dengan target atau benchmark

#### 2. Analisis Temporal
- Bandingkan hasil evaluasi dari waktu ke waktu
- Lihat perkembangan per aspek
- Evaluasi efektivitas program perbaikan

#### 3. Analisis Evaluator
- Bandingkan perspektif evaluator berbeda
- Identifikasi konsensus dan perbedaan
- Gunakan untuk validasi

### Tindak Lanjut

#### Prioritas Tinggi (Skor < 3)
1. Segera buat rencana perbaikan
2. Alokasikan sumber daya
3. Tentukan penanggung jawab
4. Set target dan timeline
5. Monitor progress mingguan

#### Prioritas Sedang (Skor 3-4)
1. Identifikasi area peningkatan spesifik
2. Buat program pengembangan
3. Libatkan stakeholder terkait
4. Monitor progress bulanan

#### Pertahankan (Skor > 4)
1. Dokumentasikan best practices
2. Share dengan tim lain
3. Jaga konsistensi
4. Terus inovasi

---

## ❓ FAQ (FREQUENTLY ASKED QUESTIONS)

### Q1: Seberapa sering evaluasi harus dilakukan?

**A:** Disarankan minimal:
- **Evaluasi Rutin**: Setiap bulan oleh tim monev internal
- **Evaluasi Komprehensif**: Setiap semester oleh kepala sekolah
- **Evaluasi Eksternal**: Setiap tahun oleh pengawas atau komite

### Q2: Siapa yang berhak menjadi evaluator?

**A:** Evaluator yang dapat menggunakan instrumen ini:
- Kepala Sekolah
- Wakil Kepala Sekolah
- Ketua Komite Sekolah
- Pengawas Sekolah
- Tim Monitoring dan Evaluasi yang ditunjuk
- Pihak eksternal yang diberi akses

### Q3: Apakah data evaluasi bersifat rahasia?

**A:** 
- Dashboard pimpinan dilindungi password
- Data dapat dibagikan sesuai kebijakan sekolah
- Sebaiknya hasil digunakan untuk perbaikan, bukan sanksi
- Transparansi dengan stakeholder dianjurkan

### Q4: Bagaimana jika ada ketidaksesuaian hasil antar evaluator?

**A:** 
- Diskusikan temuan dengan semua evaluator
- Lakukan observasi bersama untuk validasi
- Gunakan triangulasi data (dokumen, observasi, wawancara)
- Fokus pada fakta dan bukti, bukan persepsi

### Q5: Apakah instrumen ini bisa dimodifikasi?

**A:** Ya, instrumen dapat disesuaikan dengan:
- Konteks dan kebutuhan sekolah
- Visi misi spesifik sekolah
- Prioritas pengembangan
- Namun pastikan tetap valid dan reliabel

### Q6: Bagaimana menindaklanjuti hasil evaluasi?

**A:** 
1. Analisis hasil secara komprehensif
2. Identifikasi prioritas perbaikan
3. Buat rencana aksi dengan timeline
4. Alokasikan sumber daya
5. Implementasi dan monitor progress
6. Evaluasi ulang untuk melihat perbaikan

### Q7: Apakah ada biaya untuk menggunakan sistem ini?

**A:** Sistem ini gratis menggunakan:
- Google Sheets (gratis untuk pendidikan)
- Browser web standar
- Tidak perlu software khusus

---

## 🔧 TROUBLESHOOTING

### Masalah 1: Form tidak bisa dibuka

**Solusi:**
- Pastikan menggunakan browser modern (Chrome, Firefox, Edge)
- Enable JavaScript di browser
- Clear cache dan cookies
- Coba browser lain

### Masalah 2: Data tidak tersimpan ke Google Sheets

**Penyebab & Solusi:**
- **Belum setup Google Apps Script**: Ikuti langkah setup di dokumentasi
- **URL Web App salah**: Pastikan URL sudah diupdate di file HTML
- **Izin akses belum diberikan**: Jalankan fungsi di Apps Script dan berikan izin
- **Sheet name tidak sesuai**: Pastikan nama sheet "Data Evaluasi"

### Masalah 3: Password dashboard tidak diterima

**Solusi:**
- Pastikan password: **SMPN38MT** (case-sensitive)
- Tidak ada spasi sebelum/sesudah
- Refresh halaman dan coba lagi
- Jika masih gagal, ganti password di kode HTML

### Masalah 4: Dashboard tidak menampilkan data

**Solusi:**
- Periksa koneksi internet
- Pastikan ada data di Google Sheets
- Refresh halaman dashboard
- Cek console browser untuk error (F12)

### Masalah 5: Formula di dashboard Google Sheets error

**Solusi:**
- Jalankan fungsi `setupDashboard` di Apps Script
- Periksa nama sheet sudah benar
- Pastikan kolom data sesuai
- Manual perbaiki formula jika perlu

### Masalah 6: File HTML tidak bisa dibuka

**Solusi:**
- Pastikan file tersimpan dengan ekstensi .html
- Klik kanan → Open with → Browser
- Atau drag-drop file ke browser

---

## 📞 KONTAK DAN DUKUNGAN

Untuk pertanyaan lebih lanjut atau bantuan teknis:

**SMP Negeri 38 Maluku Tengah**
- Email: smpn38malteng@education.id
- Telepon: (0xx) xxxx-xxxx
- Alamat: [Alamat Lengkap]

**Tim IT/Admin Sistem:**
- Nama: [Nama Admin]
- Email: [Email Admin]
- Telepon: [No Telepon]

---

## 📝 CATATAN PENTING

1. **Backup Data**: Lakukan backup Google Sheets secara berkala
2. **Update Berkala**: Tinjau dan update instrumen sesuai kebutuhan
3. **Training**: Berikan training kepada evaluator baru
4. **Konsistensi**: Gunakan standar yang sama untuk semua evaluasi
5. **Tindak Lanjut**: Hasil evaluasi harus ditindaklanjuti dengan aksi nyata

---

## 📄 VERSI DAN RIWAYAT PERUBAHAN

**Versi 1.0** (November 2024)
- Rilis awal sistem monitoring dan evaluasi
- 8 aspek penilaian
- Integrasi Google Sheets
- Dashboard pimpinan dengan password

---

**© 2024 SMP Negeri 38 Maluku Tengah**
**Sistem Monitoring dan Evaluasi - Pembelajaran Mendalam**
