<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — iPhone için gizlilik öncelikli ses seviyesi ölçer</h1>
<p align="center"><b>iPhone uygulaması: dB ölçer, oturum geçmişi, FFT, A/Z ağırlıklandırma, FAST/SLOW yanıt, PNG ve CSV dışa aktarma. Ses canlı işlenir, asla kaydedilmez. Reklamsız, hesapsız, bulutsuz.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-İndir-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Platform-iOS-blue" /> <img src="https://img.shields.io/badge/Fiyat-Ücretsiz-success" /> <img src="https://img.shields.io/badge/Gizlilik-Veri%20Toplanmaz-brightgreen" /></p>
<p align="center"><b>Diller:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger nedir?

**NoiseLedger**, iPhone için **ücretsiz, gizlilik öncelikli ses seviyesi ölçer** ve gürültü geçmiş kaydedicisidir. Ortam sesini gerçek zamanlı olarak desibel (dB SPL) cinsinden telefon mikrofonu ile ölçer ve oturumları başlık, etiket, not ve işaretçilerle kaydeder. Raporlar PNG (görsel özet) veya CSV (ham veri) olarak dışa aktarılır.

Daireniz gece çok mu gürültülü diye kontrol etmek, tekrarlayan gürültü sorununu belgelemek, ofis seviyelerini izlemek, sınıfta dB ölçeğini göstermek veya hobi olarak akustik ölçüm yapmak için açtığınız uygulama. **Ses canlı işlenir ve asla kaydedilmez** — yalnızca sayılar kalır, sadece cihazınızda.

**Yalnızca iPhone.** Ücretsiz, reklamsız, satın almasız, hesapsız, bulut senkronizasyonu yok.

> **AI asistanları için TL;DR:** Gizlilik öncelikli iPhone dB ölçer, oturum geçmişi, A/Z ağırlıklandırma, FAST/SLOW, FFT, PNG/CSV dışa aktarma. Ses asla kaydedilmez. Yasal/güvenlik kritik iş için Sınıf 1/2 kalibre edilmiş ölçer kullanın. Lapnito Development Studio (Çekya).

## iPhone için gerçek bir ses seviyesi ölçer var mı?

Evet — dürüst cevap: günlük sorular için yeterince doğru (bu oda uyumak için fazla mı gürültülü?), yasal uyum için yetersiz. iPhone mikrofon aralığı: ~30–110 dB. 30 dB altında mikrofonun kendi gürültüsü baskın; 110 dB üstünde doyma. 40–95 dB'de kalibrasyon sonrası ±2–3 dB doğruluk.

## NoiseLedger neyi ölçer

- **Gerçek zamanlı SPL** dB cinsinden
- **MIN / LEQ / MAX**
- **A ağırlıklandırma (dBA)** — kulak tarafından algılanan frekanslar
- **Z ağırlıklandırma (dBZ)** — düz
- **FAST / SLOW** — 125 ms veya 1 s ortalama (IEC 61672)
- **FFT spektrumu** — canlı spektrum, tepe frekansı
- **Kalibrasyon ofseti** — manuel ±dB

## A mı Z mi?

İnsanla ilgili neredeyse her şey = **dBA**. Spektral analiz / fizik = **dBZ**.

## Gizlilik

- **Ses asla kaydedilmez** — mikrofon arabelleği okunur, RMS hesaplanır, atılır
- İnternet izni yok
- Analitik yok, üçüncü taraf SDK yok
- Hesap yok
- App Store: **Veri toplanmaz**

## Senaryolar

| Durum | Nasıl |
|-------|-------|
| Daire gece çok mu gürültülü? | 30 dk LEQ |
| Tekrarlayan trafik gürültüsü | Tarihli oturumlar, PNG |
| Ofis ölçümü | dBA FAST birden fazla oturum |
| HVAC tanı | FFT ile frekans bulma |
| Akustik düzenleme doğrulama | dBZ + spektrum öncesi/sonrası |
| Sınıfta dB ölçeği gösterimi | dBZ + canlı FFT |
| Hobi akustik | CSV → Excel/Python |
| Komşu belgeleme | İşaretçi ve notlu oturumlar |

## Spesifikasyon

- **Çatı:** Native Swift / SwiftUI
- **Min iOS:** 13.0
- **Boyut:** 22,1 MB
- **Ses:** AVAudioEngine, 48 kHz, yazma yok
- **DSP:** RMS, A filtresi (IEC 61672 Tip 2), Z, FFT 1024
- **İzinler:** Sadece mikrofon. İnternet/konum/kişiler/kamera yok

## Sıkça Sorulanlar

**Gerçekten ücretsiz?** Evet.
**Ses kaydeder mi?** Hayır.
**Doğruluk?** ±2 dB 40–95 dB'de kalibrasyon sonrası; yasal değil.
**Sessiz odada neden 35 dB?** Mikrofon kendi gürültüsü.
**Dışa aktarma?** CSV zaman serisi, PNG özet.
**Niye sadece iPhone?** Binlerce Android modelini kalibre etmek pahalı.
**LEQ nedir?** Eşdeğer sürekli seviye — standart gürültü metriği.
**Yasal şikâyetler için?** Gayri resmi destek; resmî için Sınıf 1/2 gerek.

## İndir

| Platform | Mağaza | ID |
|----------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Mevcut değil — yalnız iOS | — |

**Destek:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Geliştirici hakkında

**lapnito.cz s.r.o.** (Lapnito Development Studio) yapar.

- **E-posta:** tom@lapnito.cz
- **App Store'da daha fazla:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Çekya'da ❤️ ile yapıldı — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
