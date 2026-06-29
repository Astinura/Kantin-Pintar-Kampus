# Kantin-Pintar-Kampus
# 📋 TEAM MANIFESTO
## Tim Konsultan IT — Proyek Aplikasi Mobile Kantin Pintar Kampus

> *"Kode yang baik dimulai dari komunikasi yang baik."*

---

## 👥 Profil Tim

| Nama | Peran | Kontak |
|------|-------|--------|
| Anggota A | UI/UX Developer | [isi email/WA] |
| Anggota B | Backend Dev + Scrum Master | [isi email/WA] |
| Anggota C | QA Tester + PO Representative | [isi email/WA] |

---

## 🎯 Nilai-Nilai Tim (Team Values)

1. **Komunikasi dulu, coding kemudian** — Sebelum mengubah apa pun yang menyangkut anggota lain, diskusikan terlebih dahulu.
2. **Tidak ada yang tahu segalanya** — Setiap anggota punya keahlian berbeda, saling menghargai dan belajar satu sama lain.
3. **Masalah kecil disampaikan segera** — Jangan tunggu sampai menjadi blocker besar. Sampaikan di Daily Standup.
4. **Dokumentasi adalah bagian dari pekerjaan** — Setiap fitur yang selesai wajib disertai dokumentasi singkat.

---

## 📝 SOP CODE REVIEW

### Tujuan
Code review bertujuan untuk meningkatkan kualitas kode secara kolektif, bukan untuk menilai kemampuan personal seseorang.

### Aturan Umum Code Review

- Setiap Pull Request (PR) wajib di-review oleh **minimal 1 anggota lain** sebelum di-merge ke branch `main`.
- Reviewer memberikan komentar dalam waktu **maksimal 1x24 jam** setelah PR dibuat.
- PR yang sudah di-approve dan tidak ada konflik wajib di-merge dalam **1x6 jam**.
- Penulis kode **tidak boleh meng-approve PR-nya sendiri**.

---

### ✅ Kalimat yang DIANJURKAN dalam Code Review

Gunakan bahasa yang berfokus pada kode, bukan pada orangnya. Berikan alasan dan solusi.

> ✅ **"Bagian ini mungkin bisa lebih efisien jika menggunakan fungsi `map()` daripada loop manual, karena lebih ringkas dan lebih mudah dibaca."**

> ✅ **"Sepertinya ada potensi null pointer di sini jika `userData` belum terisi. Apakah kita perlu menambahkan pengecekan awal?"**

> ✅ **"Variabel ini belum ada di dokumentasi API kita. Apakah ini format terbaru dari backend? Kalau iya, boleh tolong update di `API_DOCS.md`?"**

> ✅ **"Logikanya sudah benar! Ada satu saran kecil: apakah kita bisa memisahkan fungsi ini menjadi dua agar lebih mudah di-test nanti?"**

> ✅ **"Keren, implementasi ini sudah lebih clean dari sebelumnya. Hanya ada satu hal minor yang ingin aku tanyakan..."**

> ✅ **"Aku kurang paham maksud dari variabel `x` di baris 42. Bisa tolong diberi nama yang lebih deskriptif atau tambahkan komentar singkat?"**

---

### ❌ Kalimat yang DILARANG dalam Code Review

Kalimat-kalimat berikut merendahkan, tidak konstruktif, dan akan merusak kepercayaan tim.

> ❌ ~~"Kode ini jelek banget, gak jelas sama sekali."~~

> ❌ ~~"Masa begini aja gak bisa? Basic banget."~~

> ❌ ~~"Ini salah total, harus ditulis ulang dari awal."~~

> ❌ ~~"Aku udah bilangin berkali-kali caranya bukan seperti ini."~~

> ❌ ~~"Gak usah pakai cara ini, ini cara orang yang malas."~~

> ❌ ~~"Serius deh, belajar dulu sebelum push ke repo."~~

> ❌ ~~"Langsung approve aja, males review."~~ *(mengabaikan proses review)*

---

### Format Komentar PR yang Distandarisasi

Gunakan tag berikut di awal komentar agar mudah diprioritaskan:

| Tag | Artinya | Harus direspons? |
|-----|---------|-----------------|
| `[WAJIB]` | Bug atau error yang harus diperbaiki sebelum merge | Ya, sebelum merge |
| `[SARAN]` | Ide peningkatan, boleh diterapkan boleh tidak | Opsional |
| `[PERTANYAAN]` | Klarifikasi, tidak ada yang salah | Ya, jawab di thread |
| `[PUJIAN]` | Apresiasi terhadap kode yang bagus | Tidak perlu |

**Contoh penggunaan:**
```
[WAJIB] Fungsi ini tidak menangani kondisi error dari API. 
Kalau response 500, aplikasi akan crash. Tambahkan try-catch ya.

[SARAN] Mungkin kita bisa menggunakan React Query di sini untuk 
caching otomatis, tapi tidak urgent untuk sprint ini.

[PERTANYAAN] Kenapa kita menggunakan POST bukan PUT untuk 
update data di endpoint ini?
```

---

## 📡 PROTOKOL KOMUNIKASI TIM

### Jam Kerja & Komunikasi

| Aturan | Detail |
|--------|--------|
| **Jam koordinasi aktif** | 08.00 – 21.00 WIB |
| **Larangan chat koordinasi** | Di atas jam 21.00 WIB (kecuali sistem down / darurat produksi) |
| **Respon pesan wajib** | Maksimal 2 jam di jam kerja aktif |
| **Daily Standup** | Setiap hari kerja pukul 09.00 WIB (15 menit, via WA/Discord/Meet) |
| **Sprint Meeting** | Setiap awal dan akhir sprint (sesuai jadwal yang disepakati) |

### Platform Komunikasi

| Platform | Digunakan untuk |
|----------|----------------|
| **WhatsApp Group** | Update cepat, pengumuman, koordinasi harian |
| **GitHub Issues/PR** | Diskusi teknis, bug report, code review |
| **Google Meet/Zoom** | Daily Standup, Sprint Meeting, pair programming |
| **Google Drive** | Dokumen, desain, laporan |

### Aturan Channel Komunikasi

1. **Gunakan thread** untuk membalas pesan spesifik agar tidak membingungkan.
2. **Tidak boleh membahas masalah teknis di chat umum** tanpa membuka GitHub Issue terlebih dahulu.
3. **Mention spesifik** (`@NamaAnggota`) hanya jika membutuhkan respons dari orang tertentu.
4. **Tidak ada spam atau meme** di luar topik proyek di jam kerja aktif.

---

## 🚨 PROTOKOL KONFLIK & ESKALASI

### Jika Ada Perbedaan Pendapat Teknis

1. Sampaikan argumen dengan **data atau referensi**, bukan opini semata.
2. Jika tidak ada kesepakatan dalam 15 menit diskusi, **Scrum Master (Anggota B) membuat keputusan final**.
3. Keputusan yang sudah dibuat **dihormati oleh semua anggota** meski tidak semua setuju.

### Jika Ada Anggota yang Tidak Merespons / Tidak Progress

1. Tegur secara **private terlebih dahulu** (chat langsung, bukan di grup).
2. Jika tidak ada respons dalam 1x24 jam, Scrum Master mengambil alih atau meredistribusi task.
3. Masalah dicatat dalam Retrospective untuk perbaikan Sprint berikutnya.

### Jika Sistem/API Down di Luar Jam Kerja

- Boleh menghubungi via WhatsApp di atas jam 21.00 WIB.
- Tambahkan label **[DARURAT]** di awal pesan.
- Gunakan emoji 🚨 agar mudah dikenali.

---

## 🔄 FORMAT DAILY STANDUP (3 Pertanyaan)

Setiap anggota menjawab singkat setiap hari dalam 5 menit:

```
1. ✅ Kemarin aku selesaikan: [apa yang sudah dikerjakan]
2. 🔄 Hari ini aku akan: [rencana hari ini]  
3. 🚧 Blocker: [hambatan yang ada, atau "Tidak ada hambatan"]
```

**Contoh:**
```
1. ✅ Kemarin aku selesaikan: Form login sudah terhubung ke API, 
   token tersimpan di localStorage.
2. 🔄 Hari ini aku akan: Mengerjakan halaman daftar menu dan fetch data.
3. 🚧 Blocker: Endpoint GET /menus belum ready dari backend. 
   Perlu koordinasi dengan Anggota B hari ini.
```

---

## 📦 ATURAN GIT & BRANCHING

### Penamaan Branch

```
feature/[nama-fitur]     → contoh: feature/login-page
fix/[nama-bug]           → contoh: fix/payment-null-error
chore/[nama-task]        → contoh: chore/update-readme
```

### Aturan Commit Message

Format: `[tipe]: deskripsi singkat dalam bahasa Indonesia`

| Tipe | Digunakan untuk |
|------|----------------|
| `feat` | Fitur baru |
| `fix` | Perbaikan bug |
| `docs` | Perubahan dokumentasi |
| `style` | Perubahan formatting, tidak ada perubahan logika |
| `refactor` | Refactoring kode |
| `test` | Menambah atau memperbaiki test |

**Contoh commit yang benar:**
```
feat: tambahkan validasi form login
fix: perbaiki crash saat pembayaran gagal
docs: update dokumentasi endpoint API autentikasi
```

**Commit yang dilarang:**
```
❌ "fix"
❌ "update"  
❌ "asdfjkl"
❌ "coba coba"
❌ "WIP"  (kecuali di draft PR)
```

### Larangan Push Langsung ke `main`

- **Dilarang keras** melakukan `git push` langsung ke branch `main` atau `develop`.
- Semua perubahan wajib melalui **Pull Request**.
- Branch `main` hanya diperbarui oleh Scrum Master setelah Sprint Review.

---

## ✍️ PERSETUJUAN TIM

Dengan ditandatanganinya (atau disetujuinya secara digital) dokumen ini, seluruh anggota tim menyatakan memahami dan bersedia mengikuti semua aturan yang tercantum.

| Nama | Peran | Tanda Tangan / Persetujuan |
|------|-------|---------------------------|
| Anggota A | UI/UX Developer | ________________ |
| Anggota B | Backend Dev + Scrum Master | ________________ |
| Anggota C | QA Tester + PO Rep | ________________ |

**Tanggal dibuat:** _______________  
**Versi dokumen:** 1.0  
**Berlaku untuk:** Sprint 1 & Sprint 2 (2 Minggu)

---

*Dokumen ini dapat direvisi di awal setiap Sprint melalui kesepakatan bersama dalam Sprint Retrospective.*
