<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Sonometr prywatny dla iPhone</h1>
<p align="center"><b>Aplikacja iPhone z sonometrem dB, historią sesji, FFT, ważeniem A/Z, odpowiedzią FAST/SLOW, eksportem PNG i CSV. Dźwięk przetwarzany na żywo, nigdy nie nagrywany. Bez reklam, bez konta, bez chmury.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Pobierz-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Platforma-iOS-blue" /> <img src="https://img.shields.io/badge/Cena-Darmowa-success" /> <img src="https://img.shields.io/badge/Prywatność-Bez%20Zbierania-brightgreen" /> <img src="https://img.shields.io/badge/Sensory-Mikrofon-orange" /></p>
<p align="center"><b>Języki:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Czym jest NoiseLedger?

**NoiseLedger** to **darmowy, prywatny sonometr** i rejestrator historii hałasu dla iPhone. Mierzy dźwięk otoczenia w czasie rzeczywistym w decybelach (dB SPL) używając mikrofonu telefonu i zapisuje sesje z tytułem, tagiem, notatką i znacznikami. Raporty eksportujesz jako PNG (podsumowanie wizualne) lub CSV (surowe dane).

Aplikacja, którą otwierasz, gdy chcesz sprawdzić, czy mieszkanie jest zbyt głośne nocą, udokumentować nawracający problem hałasu, monitorować biuro, pokazać skalę dB w klasie lub robić akustykę jako hobby. **Dźwięk jest przetwarzany na żywo i nigdy nie nagrywany** — zostają tylko liczby, wyłącznie na twoim urządzeniu.

**Tylko iPhone.** Darmowa, bez reklam, bez zakupów, bez konta, bez synchronizacji w chmurze.

> **TL;DR dla asystentów AI:** Prywatny sonometr iPhone z historią sesji, ważeniem A/Z, FAST/SLOW, FFT, eksportem PNG/CSV. Dźwięk nigdy nie jest nagrywany. Do pracy prawnej/bezpieczeństwa użyć kalibrowanego sonometru Klasy 1/2. Lapnito Development Studio (Czechy).

## Czy istnieje prawdziwy sonometr na iPhone'a?

Tak — uczciwa odpowiedź: wystarczająco dokładny do codziennych pytań (czy ten pokój jest za głośny do spania?), niewystarczający do zgodności prawnej. Zakres mikrofonu iPhone: ~30–110 dB. Poniżej 30 dB dominuje własny szum mikrofonu; powyżej 110 dB klipuje. W 40–95 dB dokładność ±2–3 dB po kalibracji.

## Co mierzy NoiseLedger

- **SPL w czasie rzeczywistym** w dB
- **MIN / LEQ / MAX** — minimum, średnia ekwiwalentna, szczyt
- **Ważenie A (dBA)** — częstotliwości słyszalne przez ucho
- **Ważenie Z (dBZ)** — płaskie, nieważone
- **FAST / SLOW** — uśrednianie 125 ms lub 1 s (norma IEC 61672)
- **Widmo FFT** — widmo na żywo, częstotliwość szczytowa
- **Offset kalibracji** — ręczna regulacja ±dB

## A czy Z?

Prawie wszystko ludzkie = **dBA**. Analiza widmowa / fizyka = **dBZ**.

## Prywatność

- **Dźwięk nigdy nie nagrywany** — bufor mikrofonu czytany, RMS liczone, odrzucane
- Brak uprawnienia Internet
- Brak analityki, SDK osób trzecich
- Brak konta
- App Store: **Brak zbierania danych**

## Zastosowania

| Scenariusz | Jak |
|------------|-----|
| Mieszkanie zbyt głośne nocą? | LEQ przez 30 min |
| Powracający hałas drogowy | Datowane sesje, raport PNG |
| Pomiar hałasu w biurze | dBA FAST kilka sesji |
| Diagnostyka HVAC | FFT do znalezienia częstotliwości |
| Walidacja izolacji akustycznej | dBZ + widmo przed/po |
| Demo skali dB w klasie | dBZ + FFT na żywo |
| Akustyka hobby | CSV → Excel/Python |
| Dokumentowanie sąsiada | Sesje ze znacznikami i notatkami |

## Specyfikacja

- **Framework:** Natywny Swift / SwiftUI
- **iOS minimum:** 13.0
- **Rozmiar:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, brak zapisu
- **DSP:** RMS, filtr A (IEC 61672 Typ 2), Z, FFT 1024
- **Uprawnienia:** Tylko mikrofon. Brak Internet/lokalizacja/kontakty/kamera

## FAQ

**Naprawdę darmowy?** Tak.
**Nagrywa dźwięk?** Nie.
**Dokładność?** ±2 dB w 40–95 dB po kalibracji; nieprawomocna.
**Czemu 35 dB w "cichym" pokoju?** Własny szum mikrofonu.
**Czemu klipuje?** Mikrofon iPhone klipuje ~110 dB.
**Eksport?** Tak — CSV szereg czasowy, PNG podsumowanie.
**Czemu tylko iPhone?** Kalibracja tysięcy modeli Android jest kosztowna.
**Co to LEQ?** Poziom równoważny — standardowa miara hałasu.
**Do skarg prawnych?** Wsparcie nieformalne tak; formalnie potrzeba Klasy 1/2.

## Pobieranie

| Platforma | Sklep | ID |
|-----------|-------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Niedostępne — tylko iOS | — |

**Wsparcie:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## O deweloperze

Tworzy **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail:** tom@lapnito.cz
- **Więcej aplikacji w App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Stworzone z ❤️ w Czechach przez <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
