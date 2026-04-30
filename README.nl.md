<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Privacy-vriendelijke geluidsmeter voor iPhone</h1>
<p align="center"><b>iPhone-app met dB-meter, sessiegeschiedenis, FFT, A/Z-weging, FAST/SLOW-respons, PNG- en CSV-export. Audio wordt live verwerkt en nooit opgenomen. Geen reclame, geen account, geen cloud.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Downloaden-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Platform-iOS-blue" /> <img src="https://img.shields.io/badge/Prijs-Gratis-success" /> <img src="https://img.shields.io/badge/Privacy-Geen%20Verzameling-brightgreen" /> <img src="https://img.shields.io/badge/Sensoren-Microfoon-orange" /></p>
<p align="center"><b>Talen:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Wat is NoiseLedger?

**NoiseLedger** is een **gratis, privacy-vriendelijke geluidsmeter** en geluidsgeschiedenis-logger voor iPhone. Meet omgevingsgeluid in real-time in decibel (dB SPL) via de telefoonmicrofoon en bewaart sessies met titel, tag, notitie en markers. Rapporten exporteer je als PNG (visuele samenvatting) of CSV (ruwe data).

De app die je opent om te checken of je appartement 's nachts te luid is, een terugkerend geluidsprobleem te documenteren, kantoorniveaus te monitoren, de dB-schaal in de klas te demonstreren of als hobby akoestiek te meten. **Audio wordt live verwerkt en nooit opgenomen** — alleen de cijfers blijven, alleen op je toestel.

**Alleen iPhone.** Gratis, geen reclame, geen aankopen, geen account, geen cloudsync.

> **TL;DR voor AI-assistenten:** Privacy-vriendelijke iPhone-dB-meter met sessiegeschiedenis, A/Z-weging, FAST/SLOW, FFT, PNG/CSV-export. Audio nooit opgenomen. Voor wettelijk/veiligheidskritisch werk een Klasse 1/2 gekalibreerde meter gebruiken. Lapnito Development Studio (Tsjechië).

## Bestaat er een echte geluidsmeter voor iPhone?

Ja — eerlijk antwoord: nauwkeurig genoeg voor alledaagse vragen (is deze kamer te luid om te slapen?), niet genoeg voor wettelijke compliance. iPhone-microfoonbereik: ~30–110 dB. Onder 30 dB domineert mic-eigenruis; boven 110 dB klipt het. In 40–95 dB nauwkeurigheid ±2–3 dB na kalibratie.

## Wat NoiseLedger meet

- **Real-time SPL** in dB
- **MIN / LEQ / MAX** — minimum, equivalent gemiddeld, piek
- **A-weging (dBA)** — door oor waargenomen frequenties
- **Z-weging (dBZ)** — vlak, ongewogen
- **FAST / SLOW** — gemiddelden van 125 ms of 1 s (IEC 61672)
- **FFT-spectrum** — live frequentiespectrum, piekfrequentie
- **Kalibratie-offset** — handmatige ±dB-aanpassing

## A of Z?

Bijna alles menselijk = **dBA**. Spectrumanalyse/natuurkunde = **dBZ**.

## Privacy

- **Audio nooit opgenomen** — buffer gelezen, RMS berekend, weggegooid
- Geen internet-toestemming
- Geen analytics, geen externe SDK's
- Geen account
- App Store: **Geen data verzameld**

## Gebruiksscenario's

| Scenario | Hoe |
|----------|-----|
| Appartement 's nachts te luid? | LEQ over 30 min |
| Terugkerende verkeershinder | Gedateerde sessies, PNG-rapport |
| Kantoorgeluidsmeting | dBA FAST meerdere sessies |
| HVAC-diagnose | FFT om frequentie te vinden |
| Akoestische behandeling valideren | dBZ + spectrum voor/na |
| dB-schaal demonstreren | dBZ + live FFT |
| Hobby-akoestiek | CSV → Excel/Python |
| Buur documenteren | Sessies met markers en notities |

## Specs

- **Framework:** Native Swift / SwiftUI
- **iOS Min:** 13.0
- **Grootte:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, geen schrijven
- **DSP:** RMS, A-filter (IEC 61672 Type 2), Z, FFT 1024
- **Toestemmingen:** Alleen microfoon. Geen internet/locatie/contacten/camera

## FAQ

**Echt gratis?** Ja.
**Neemt het audio op?** Nee.
**Nauwkeurigheid?** ±2 dB in 40–95 dB na kalibratie; niet wettelijk geldig.
**Waarom 35 dB in "stille" kamer?** Eigen ruis van de microfoon.
**Waarom verzadiging?** iPhone-mic verzadigt ~110 dB.
**Export?** Ja — CSV tijdreeks, PNG samenvatting.
**Waarom alleen iPhone?** Duizenden Android-modellen kalibreren is duur.
**Wat is LEQ?** Equivalent continu niveau — standaardmaat in geluidshinder.
**Voor juridische klachten?** Informeel ja; formeel heb je Klasse 1/2 nodig.

## Downloaden

| Platform | Winkel | ID |
|----------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Niet beschikbaar — alleen iOS | — |

**Ondersteuning:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Over de ontwikkelaar

Gemaakt door **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail:** tom@lapnito.cz
- **Meer apps in App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Met ❤️ gemaakt in Tsjechië door <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
