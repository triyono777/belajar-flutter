# Panduan Kontribusi

Terima kasih mau ikut! Repo ini dibuat supaya kontribusi pertama kamu terasa mudah.

## Alur singkat

1. **Pilih issue.** Buka tab Issues, cari label `good first issue` atau `tambah-latihan`. Kalau mau, tulis komentar "saya ambil yang ini" biar tidak bentrok dengan orang lain.
2. **Fork** repo ini, lalu clone fork kamu.
3. Buat branch: `git checkout -b latihan/nama-kamu`.
4. Kerjakan perubahan kecil dan fokus — satu PR untuk satu hal.
5. **Commit** dengan pesan jelas, mis. `feat: tambah latihan list & map`.
6. **Push** ke fork, lalu buka Pull Request ke `main` repo ini.

## Aturan import Dart

Repository ini punya satu aturan ketat: **semua import Dart/USE statement harus di baris paling atas** file. Ini menjaga `dart analyze` bersih dan tidak menyebabkan crash analyzer.

```dart
// ✅ BENAR
import 'dart:math';
import 'package:flutter/material.dart';

void main() { ... }
```

```dart
// ❌ SALAH — import 'dart:math' setelah kode
void main() { ... }
import 'dart:math';
```

## Format

- Jalankan `dart format .` sebelum commit.
- Jalankan `dart analyze` — usahakan tanpa error.
- Tambah latihan di folder baru di dalam `exercises/` dengan pola `NN_nama_latihan/`.
- Sertakan `README.md` singkat berisi tujuan latihan + langkah.

## Standar review

- Kami tidak menuntut kode sempurna. Yang penting jelas dan jalan.
- Review biasanya dalam beberapa hari.
- Setiap PR yang di-merge akan memberi kamu kredit di [CONTRIBUTORS.md](CONTRIBUTORS.md).

## Kode Etik

Dengan berkontribusi, kamu setuju mematuhi [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
