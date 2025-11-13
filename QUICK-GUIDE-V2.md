# 🚀 QUICK GUIDE - Fitur Multi-Role (V2.0)

## Update Terbaru: Dropdown Role Pengguna dengan Field Dinamis!

---

## 📝 CARA MENGGUNAKAN

### 1️⃣ Buka Form Evaluasi

Buka file `monitoring-evaluasi.html` di browser

---

### 2️⃣ Pilih "Saya adalah"

Di bagian atas form, Anda akan melihat dropdown **"Saya adalah"**:

```
┌────────────────────────────────┐
│ Saya adalah *                  │
│ [-- Pilih Role Anda -- ▼]     │
└────────────────────────────────┘
```

**Pilihan yang tersedia:**
- 👨‍🎓 **Siswa**
- 👨‍🏫 **Guru**
- 👔 **Komite Sekolah**
- 🎓 **Kepala Sekolah**
- 📋 **Wakil Kepala Sekolah**
- 🔍 **Pengawas**
- 📊 **Tim Monitoring & Evaluasi**
- ➕ **Lainnya**

---

### 3️⃣ Isi Field yang Muncul

Field yang muncul akan berbeda tergantung role yang Anda pilih:

#### 🎓 UNTUK SISWA

Akan muncul dropdown **Kelas**:
```
┌────────────────────────────────┐
│ Kelas *                        │
│ [-- Pilih Kelas -- ▼]         │
│                                │
│ Pilihan:                       │
│ • VII A, VII B, VII C, VII D   │
│ • VIII A, VIII B, VIII C, VIII D│
│ • IX A, IX B, IX C, IX D       │
└────────────────────────────────┘
```

**Contoh:**
- Nama: Andi Wijaya
- Kelas: IX A

---

#### 👨‍🏫 UNTUK GURU

Akan muncul field **Mata Pelajaran**:
```
┌────────────────────────────────────────┐
│ Mata Pelajaran yang Diampu *          │
│ [Matematika...]                        │
└────────────────────────────────────────┘
```

**Contoh:**
- Nama: Siti Nurhaliza, M.Pd
- Mata Pelajaran: Matematika

**Tips:** Bisa tulis multiple mapel, contoh: "Matematika & IPA"

---

#### 👔 UNTUK KOMITE SEKOLAH

Tidak ada field tambahan! Hanya perlu isi nama.

```
┌────────────────────────────────────────┐
│ ✓ Terima kasih atas partisipasi Anda  │
│   sebagai anggota Komite Sekolah      │
└────────────────────────────────────────┘
```

**Contoh:**
- Nama: Hj. Fatimah

---

#### 🎓📋🔍📊 UNTUK PIMPINAN & TIM MONEV

Akan muncul field **Jabatan/Posisi**:
```
┌────────────────────────────────────────┐
│ Jabatan/Posisi *                       │
│ [Wakasek Kurikulum...]                 │
└────────────────────────────────────────┘
```

**Contoh untuk Wakil Kepala:**
- Nama: Dr. Budi Santoso
- Jabatan: Wakasek Kurikulum

**Contoh untuk Tim Monev:**
- Nama: Ahmad Hidayat
- Jabatan: Ketua Tim Monev

**Contoh untuk Pengawas:**
- Nama: Drs. Ruslan
- Jabatan: Pengawas Sekolah

---

### 4️⃣ Lanjutkan Evaluasi

Setelah mengisi informasi di atas:
1. ✅ Beri penilaian untuk 8 aspek (skala 1-5)
2. ✅ Tambahkan catatan dan rekomendasi
3. ✅ Klik "Simpan Evaluasi"

---

## 📊 TAMPILAN DASHBOARD

Dashboard pimpinan sekarang menampilkan kolom tambahan:

```
┌────────┬──────────┬─────────────┬──────────────┐
│ Nama   │ Role     │ Kelas/Mapel │ Persentase   │
├────────┼──────────┼─────────────┼──────────────┤
│ Andi   │ Siswa    │ IX A        │ 78.0%        │
│ Siti   │ Guru     │ Matematika  │ 72.5%        │
│ Fatimah│ Komite   │ -           │ 82.5%        │
│ Budi   │ Pengawas │ Pengawas Sklh│ 65.0%       │
└────────┴──────────┴─────────────┴──────────────┘
```

---

## ❓ FAQ - Fitur Role

### Q: Apakah siswa boleh mengisi evaluasi?
**A:** Boleh! Ini justru salah satu tujuan update ini - melibatkan semua stakeholder termasuk siswa.

### Q: Saya guru yang mengajar banyak mapel, bagaimana?
**A:** Tulis semua mapel yang Anda ajar, contoh: "Matematika, IPA, TIK"

### Q: Saya wakasek, pilih role apa?
**A:** Pilih "Wakil Kepala Sekolah", lalu di jabatan tulis spesifik Anda (Wakasek Kurikulum, Wakasek Kesiswaan, dll)

### Q: Field yang muncul salah/tidak muncul?
**A:** Pastikan Anda sudah memilih role di dropdown "Saya adalah". Field akan muncul otomatis setelah role dipilih.

### Q: Bisakah saya mengisi tanpa memilih role?
**A:** Tidak. Role adalah field wajib. Sistem akan validasi dan tidak bisa submit jika role belum dipilih.

---

## ✅ CHECKLIST SEBELUM SUBMIT

Pastikan sudah:
- [ ] Pilih role yang sesuai
- [ ] Isi nama lengkap
- [ ] Isi field tambahan sesuai role (kelas/mapel/jabatan)
- [ ] Beri penilaian semua 8 aspek
- [ ] Tambahkan catatan (opsional tapi sangat direkomendasikan)

---

## 🎯 MANFAAT FITUR INI

### Untuk Sekolah:
✅ Evaluasi lebih komprehensif dari berbagai perspektif
✅ Melibatkan semua stakeholder (siswa, guru, komite, pimpinan)
✅ Data lebih kaya untuk analisis

### Untuk Analisis:
✅ Bisa bandingkan persepsi antar role
✅ Identifikasi gap antara guru dan siswa
✅ Lihat pola per kelas atau mata pelajaran

### Untuk Perbaikan:
✅ Tindak lanjut lebih spesifik per kelompok
✅ Program perbaikan yang targeted
✅ Monitoring yang lebih detail

---

## 💡 TIPS & BEST PRACTICE

### Untuk Siswa:
- 💬 Jujur dalam memberikan penilaian
- 💬 Berikan catatan konstruktif
- 💬 Fokus pada pengalaman belajar Anda

### Untuk Guru:
- 💬 Evaluasi dari perspektif pembelajaran Anda
- 💬 Catat kendala dan kebutuhan
- 💬 Berikan masukan untuk perbaikan

### Untuk Komite:
- 💬 Lihat dari sudut pandang orangtua/masyarakat
- 💬 Fokus pada keterlibatan stakeholder
- 💬 Evaluasi komunikasi sekolah-komite

### Untuk Pimpinan:
- 💬 Evaluasi implementasi kebijakan
- 💬 Identifikasi area yang perlu support
- 💬 Catat progress dan tantangan

---

## 🔄 PERBANDINGAN VERSI

### Versi Lama (V1.0):
```
Informasi Evaluator:
├── Tanggal
├── Nama
└── Jabatan (dropdown fix)
```

### Versi Baru (V2.0):
```
Informasi Evaluator:
├── Tanggal
├── Saya adalah (dropdown role)
├── Nama
└── Field Dinamis:
    ├── Kelas (untuk siswa)
    ├── Mata Pelajaran (untuk guru)
    └── Jabatan (untuk pimpinan/lainnya)
```

---

## 🎬 VIDEO TUTORIAL (Coming Soon)

Kami sedang menyiapkan video tutorial penggunaan fitur ini. Stay tuned!

---

## 📞 BUTUH BANTUAN?

Jika mengalami kesulitan:
1. Baca dokumentasi lengkap di `DOKUMENTASI.md`
2. Cek update log di `UPDATE-LOG-V2.md`
3. Hubungi admin IT sekolah

---

**Selamat menggunakan fitur baru! 🎉**

Mari ciptakan evaluasi yang lebih inklusif dan komprehensif dengan melibatkan seluruh stakeholder pendidikan!

---

*Update: 14 November 2024*
*Version: 2.0*
