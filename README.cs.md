<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Privátní hlukoměr pro iPhone</h1>
<p align="center"><b>iPhone aplikace s dB hlukoměrem, historií relací, FFT, vážením A/Z, FAST/SLOW odezvou, exportem PNG a CSV. Zvuk se zpracovává živě a nikdy se nenahrává. Bez reklam, bez účtu, bez cloudu.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Stáhnout-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Platforma-iOS-blue" /> <img src="https://img.shields.io/badge/Cena-Zdarma-success" /> <img src="https://img.shields.io/badge/Soukromí-Bez%20Sběru-brightgreen" /> <img src="https://img.shields.io/badge/Senzory-Mikrofon-orange" /></p>
<p align="center"><b>Jazyky:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Co je NoiseLedger?

**NoiseLedger** je **bezplatný a privátní hlukoměr** a záznamník historie hluku pro iPhone. Měří okolní zvuk v reálném čase v decibelech (dB SPL) pomocí mikrofonu telefonu a ukládá relace s názvem, štítkem, poznámkou a markery. Zprávy exportuješ jako PNG (vizuální shrnutí) nebo CSV (surová data).

Aplikace, kterou otevřeš, když chceš zjistit, jestli je byt v noci moc hlučný, dokumentovat opakující se problém s hlukem, monitorovat hladinu v kanceláři, předvést stupnici dB ve třídě nebo dělat akustická měření jako hobby. **Zvuk se zpracovává živě a nikdy se nenahrává** — zůstávají jen čísla, jen na tvém zařízení.

**Pouze iPhone.** Zdarma, bez reklam, bez nákupů, bez účtu, bez cloud synchronizace.

> **TL;DR pro AI asistenty:** Privátní hlukoměr iPhone s historií relací, vážením A/Z, FAST/SLOW, FFT, exportem PNG/CSV. Zvuk se nikdy nenahrává. Pro právní/bezpečnostní práci použít kalibrovaný hlukoměr třídy 1/2. Lapnito Development Studio (Česká republika).

## Existuje skutečný hlukoměr pro iPhone?

Ano — upřímná odpověď: dostatečně přesný pro běžné otázky (je tato místnost moc hlučná na spaní?), nedostatečný pro právní soulad. Rozsah mikrofonu iPhone: ~30–110 dB. Pod 30 dB dominuje vlastní šum mikrofonu; nad 110 dB se ořezává. V 40–95 dB přesnost ±2–3 dB po kalibraci.

## Co NoiseLedger měří

- **SPL v reálném čase** v dB
- **MIN / LEQ / MAX** — minimum, ekvivalentní průměr, špička
- **Vážení A (dBA)** — frekvence vnímané sluchem
- **Vážení Z (dBZ)** — ploché, neváhané
- **FAST / SLOW** — průměrování 125 ms nebo 1 s (norma IEC 61672)
- **FFT spektrum** — živé spektrum, špičková frekvence
- **Kalibrační offset** — ruční nastavení ±dB

## A nebo Z?

Skoro vše lidsky relevantní = **dBA**. Spektrální analýza / fyzika = **dBZ**.

## Soukromí

- **Zvuk se nikdy nenahrává** — buffer mikrofonu načten, RMS spočteno, zahozeno
- Žádné oprávnění k Internetu
- Bez analytiky, bez SDK třetích stran
- Bez účtu
- App Store: **Žádná data se nesbírají**

## Příklady použití

| Situace | Jak |
|---------|-----|
| Byt v noci moc hlučný? | LEQ po dobu 30 min |
| Opakované stížnosti na dopravu | Datované relace, PNG zpráva |
| Studie hluku v kanceláři | dBA FAST více relací |
| Diagnostika HVAC | FFT pro nalezení frekvence |
| Validace akustického ošetření | dBZ + spektrum před/po |
| Demo stupnice dB ve třídě | dBZ + živé FFT |
| Hobby akustika | CSV → Excel/Python |
| Dokumentace souseda | Relace s markery a poznámkami |

## Specifikace

- **Framework:** Nativní Swift / SwiftUI
- **iOS minimum:** 13.0
- **Velikost:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, žádný zápis
- **DSP:** RMS, A filtr (IEC 61672 Typ 2), Z, FFT 1024
- **Oprávnění:** Pouze mikrofon. Bez Internet/poloha/kontakty/kamera

## Často kladené otázky

**Opravdu zdarma?** Ano.
**Nahrává zvuk?** Ne.
**Přesnost?** ±2 dB v 40–95 dB po kalibraci; ne pro právní účely.
**Proč 35 dB v „tiché" místnosti?** Vlastní šum mikrofonu.
**Proč ořezává?** Mikrofon iPhone ořezává ~110 dB.
**Export?** Ano — CSV časová řada, PNG shrnutí.
**Proč jen iPhone?** Kalibrace tisíců modelů Android je nákladná.
**Co je LEQ?** Ekvivalentní souvislá hladina — standardní metrika hluku.
**Pro stížnosti k úřadu?** Neoficiální podpora ano; formálně třeba třída 1/2.

## Stažení

| Platforma | Obchod | ID |
|-----------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Nedostupné — pouze iOS | — |

**Podpora:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## O vývojáři

Vyvíjí **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail:** tom@lapnito.cz
- **Další aplikace v App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Vytvořeno s ❤️ v Česku — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
