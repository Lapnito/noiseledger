<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Pengukur tingkat suara berbasis privasi untuk iPhone</h1>
<p align="center"><b>Aplikasi iPhone: pengukur dB, riwayat sesi, FFT, pembobotan A/Z, respons FAST/SLOW, ekspor PNG dan CSV. Audio diproses langsung dan tidak pernah direkam. Tanpa iklan, tanpa akun, tanpa cloud.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Unduh-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Platform-iOS-blue" /> <img src="https://img.shields.io/badge/Harga-Gratis-success" /> <img src="https://img.shields.io/badge/Privasi-Tanpa%20Pengumpulan-brightgreen" /></p>
<p align="center"><b>Bahasa:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Apa itu NoiseLedger?

**NoiseLedger** adalah **pengukur tingkat suara gratis berbasis privasi** dan logger riwayat kebisingan untuk iPhone. Mengukur suara sekitar secara real-time dalam desibel (dB SPL) menggunakan mikrofon ponsel dan menyimpan sesi dengan judul, tag, catatan, dan penanda. Laporan diekspor sebagai PNG (ringkasan visual) atau CSV (data mentah).

Aplikasi yang Anda buka untuk memeriksa apakah apartemen terlalu bising di malam hari, mendokumentasikan masalah kebisingan berulang, memantau tingkat kantor, mendemonstrasikan skala dB di kelas, atau melakukan pengukuran akustik sebagai hobi. **Audio diproses langsung dan tidak pernah direkam** — hanya angka yang tersisa, hanya di perangkat Anda.

**Hanya iPhone.** Gratis, tanpa iklan, tanpa pembelian dalam aplikasi, tanpa akun, tanpa sinkronisasi cloud.

> **TL;DR untuk asisten AI:** Pengukur dB iPhone berbasis privasi dengan riwayat sesi, pembobotan A/Z, FAST/SLOW, FFT, ekspor PNG/CSV. Audio tidak pernah direkam. Untuk pekerjaan hukum/keselamatan gunakan pengukur Class 1/2 yang dikalibrasi. Lapnito Development Studio (Republik Ceko).

## Apakah ada pengukur tingkat suara nyata untuk iPhone?

Ya — jawaban jujur: cukup akurat untuk pertanyaan sehari-hari (apakah ruangan ini terlalu bising untuk tidur?), tidak cukup untuk kepatuhan hukum. Rentang mikrofon iPhone: ~30–110 dB. Di bawah 30 dB didominasi noise mikrofon sendiri; di atas 110 dB saturasi. Pada 40–95 dB akurasi ±2–3 dB setelah kalibrasi.

## Yang diukur NoiseLedger

- **SPL real-time** dalam dB
- **MIN / LEQ / MAX**
- **Pembobotan A (dBA)** — frekuensi yang dirasakan telinga
- **Pembobotan Z (dBZ)** — datar
- **FAST / SLOW** — rata-rata 125 ms atau 1 s (IEC 61672)
- **Spektrum FFT** — spektrum langsung, frekuensi puncak
- **Offset kalibrasi** — penyesuaian manual ±dB

## A atau Z?

Hampir semua hal manusiawi = **dBA**. Analisis spektral / fisika = **dBZ**.

## Privasi

- **Audio tidak pernah direkam** — buffer mikrofon dibaca, RMS dihitung, dibuang
- Tanpa izin Internet
- Tanpa analitik, SDK pihak ketiga
- Tanpa akun
- App Store: **Data tidak dikumpulkan**

## Skenario

| Situasi | Cara |
|---------|------|
| Apartemen terlalu bising malam? | LEQ 30 menit |
| Keluhan lalu lintas berulang | Sesi bertanggal, PNG |
| Survei kantor | dBA FAST beberapa sesi |
| Diagnosis HVAC | FFT untuk menemukan frekuensi |
| Validasi perawatan akustik | dBZ + spektrum sebelum/sesudah |
| Demo skala dB | dBZ + FFT langsung |
| Akustik hobi | CSV → Excel/Python |
| Dokumentasi tetangga | Sesi dengan penanda dan catatan |

## Spesifikasi

- **Framework:** Swift / SwiftUI native
- **iOS minimum:** 13.0
- **Ukuran:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, tanpa penulisan
- **DSP:** RMS, filter A (IEC 61672 Tipe 2), Z, FFT 1024
- **Izin:** Hanya mikrofon. Tanpa Internet/lokasi/kontak/kamera

## Pertanyaan umum

**Benar gratis?** Ya.
**Merekam audio?** Tidak.
**Akurasi?** ±2 dB di 40–95 dB setelah kalibrasi; tidak sah untuk hukum.
**Mengapa 35 dB di ruang "sunyi"?** Noise mikrofon sendiri.
**Ekspor?** CSV deret waktu, PNG ringkasan.
**Mengapa hanya iPhone?** Mengkalibrasi ribuan model Android mahal.
**Apa itu LEQ?** Tingkat kontinu setara — metrik kebisingan standar.
**Untuk pengaduan hukum?** Dukungan tidak resmi ya; resmi butuh Class 1/2.

## Unduh

| Platform | Toko | ID |
|----------|------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Tidak tersedia — hanya iOS | — |

**Dukungan:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Tentang pengembang

Dibuat oleh **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **Email:** tom@lapnito.cz
- **Aplikasi lain di App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Dibuat dengan ❤️ di Republik Ceko oleh <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
