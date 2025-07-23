# 📋 Proyek To-Do List Flutter: KerjainAja

## 🏷️ Nama Proyek
KerjainAja

## 🎯 Tujuan
Aplikasi ini dibuat untuk keperluan pribadi dalam:
- Mencatat dan mengelola tugas dengan indikator prioritas berdasarkan deadline.
- Menandai kehadiran kelas secara manual (absensi pribadi) berdasarkan jadwal harian.
- Mengatur waktu dan tanggung jawab akademik secara ringkas, offline, dan efisien.

## 👤 Stakeholder
- **Pengguna utama:** Angga (pengembang sekaligus pengguna tunggal)
- **Pengguna lain:** Tidak ada

## 💻 Teknologi yang Digunakan
| Komponen         | Teknologi                                  |
|------------------|---------------------------------------------|
| Framework        | Flutter                                     |
| Output Target    | Windows (.exe)                              |
| Penyimpanan      | Hive (local, offline, ringan)               |
| Bahasa & Zona    | Bahasa Indonesia, Waktu: GMT+7              |
| Versi OS Utama   | Windows 10/11 (laptop), iOS (referensi, tidak digunakan) |

## 📦 Dependencies Flutter
```yaml
dependencies:
  flutter:
    sdk: flutter
  hive: ^2.2.3
  hive_flutter: ^1.1.0
  path_provider: ^2.0.15
  intl: ^0.18.1
  flutter_slidable: ^3.0.0
  fluttertoast: ^8.2.2
```

## 🧩 Fitur Utama

### 1. Manajemen Tugas
- Input tugas dengan:
  - Nama tugas
  - Tanggal deadline
- Indikator warna:
  - 🟥 Merah = Sudah lewat deadline
  - 🟨 Kuning = Deadline 1–2 hari lagi
  - 🟩 Hijau = Deadline lebih dari 2 hari
- Aksi:
  - Tambah tugas
  - Edit tugas
  - Hapus tugas
  - Centang tugas selesai

### 2. Jadwal & Kehadiran Kelas
- Tabel harian yang menampilkan:
  - Hari (Senin–Minggu)
  - Jam kelas
  - Mata kuliah
  - Dosen
  - Jenis kelas: Offline / Online / Mandiri
  - Status hadir: ✅/❌ (cek manual)

### 3. Feedback & Notifikasi
- Menampilkan pesan:
  - Sukses simpan data
  - Gagal input data
  - Hapus data konfirmasi
- Implementasi via `Snackbar`, `Toast`, atau `Dialog` Flutter.

### 4. Offline Storage
- Semua data disimpan di device menggunakan Hive (No internet required).

## 📁 Struktur Folder (awal)
```
lib/
├── main.dart
├── models/
│   ├── task_model.dart
│   └── schedule_model.dart
├── screens/
│   ├── home_screen.dart
│   ├── task_screen.dart
│   └── schedule_screen.dart
├── widgets/
│   ├── task_card.dart
│   └── schedule_card.dart
├── utils/
│   └── hive_utils.dart
```

## 🔜 Tahapan Selanjutnya
- [ ] Inisialisasi project Flutter
- [ ] Setup Hive & konfigurasi box
- [ ] Buat model data (Task & Schedule)
- [ ] Desain UI awal (Home, Input, List)
- [ ] Implementasi fitur tugas
- [ ] Implementasi fitur kelas & absensi
- [ ] Penambahan validasi & feedback
- [ ] Build ke .exe (Windows)

## 📅 Timeline Perkiraan
| Hari Ke | Progres                                |
|--------:|-----------------------------------------|
| 1       | Dokumentasi & Riset awal                |
| 2–3     | Setup project & tampilan dasar          |
| 4–5     | Fitur Tugas & penyimpanan Hive          |
| 6–7     | Fitur Jadwal kelas & absensi manual     |
| 8       | Validasi, finishing UI, build ke .exe   |

---

_Dokumen ini akan diperbarui secara berkala hingga proyek selesai._
