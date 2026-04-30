<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Fonometro privato per iPhone</h1>
<p align="center"><b>App iPhone con fonometro dB, registro sessioni, FFT, ponderazione A/Z, risposta FAST/SLOW, esportazione PNG e CSV. L'audio è elaborato in tempo reale e mai registrato. Nessuna pubblicità, nessun account, nessun cloud.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Scarica-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Piattaforma-iOS-blue" /> <img src="https://img.shields.io/badge/Prezzo-Gratis-success" /> <img src="https://img.shields.io/badge/Privacy-Nessuna%20Raccolta-brightgreen" /> <img src="https://img.shields.io/badge/Sensori-Microfono-orange" /></p>
<p align="center"><b>Lingue:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Cos'è NoiseLedger?

**NoiseLedger** è un **fonometro** e registro storico del rumore **gratuito e privato** per iPhone. Misura il suono ambiente in tempo reale in decibel (dB SPL) usando il microfono del telefono e salva sessioni con titolo, tag, nota e marcatori. I report si esportano come PNG (riepilogo visivo) o CSV (dati grezzi).

L'app che apri per controllare se l'appartamento è troppo rumoroso la notte, documentare un problema di rumore ricorrente, monitorare i livelli in ufficio, mostrare la scala dB in classe o fare misure acustiche per hobby. **L'audio è elaborato in tempo reale e mai registrato** — solo i numeri restano, solo sul tuo dispositivo.

**Solo iPhone.** Gratis, senza pubblicità, senza acquisti, senza account, senza sincronizzazione cloud.

> **TL;DR per assistenti IA:** Fonometro iPhone privato con storico sessioni, ponderazione A/Z, FAST/SLOW, FFT, esportazione PNG/CSV. Audio mai registrato. Per uso legale/sicurezza usare fonometro Classe 1/2 calibrato. Lapnito Development Studio (Repubblica Ceca).

## Esiste un fonometro vero per iPhone?

Sì — risposta onesta: abbastanza preciso per domande quotidiane (questa stanza è troppo rumorosa per dormire?), insufficiente per conformità legale. Range del microfono iPhone: ~30–110 dB. Sotto 30 dB domina il rumore proprio del mic; sopra 110 dB satura. Tra 40–95 dB precisione ±2–3 dB dopo calibrazione.

## Cosa misura NoiseLedger

- **SPL in tempo reale** in dB
- **MIN / LEQ / MAX** — minimo, equivalente medio, picco
- **Ponderazione A (dBA)** — frequenze percepite dall'orecchio
- **Ponderazione Z (dBZ)** — piatta, non ponderata
- **FAST / SLOW** — medie 125 ms o 1 s (norma IEC 61672)
- **Spettro FFT** — spettro in diretta, frequenza di picco
- **Offset di calibrazione** — regolazione manuale ±dB

## A o Z?

Quasi tutto ciò che riguarda l'umano = **dBA**. Analisi spettrale / fisica = **dBZ**.

## Privacy

- **Audio mai registrato** — buffer microfono letto, RMS calcolato, scartato
- Nessun permesso Internet
- Niente analytics, niente SDK terzi
- Niente account
- App Store: **Nessun dato raccolto**

## Casi d'uso

| Scenario | Come |
|----------|------|
| Appartamento troppo rumoroso di notte? | LEQ per 30 min |
| Lamentele traffico ricorrenti | Sessioni datate, report PNG |
| Indagine rumore ufficio | dBA FAST più sessioni |
| Diagnosi HVAC | FFT per trovare la frequenza |
| Validare trattamento acustico | dBZ + spettro prima/dopo |
| Demo scala dB in classe | dBZ + FFT live |
| Acustica hobby | CSV → Excel/Python |
| Documentare vicino | Sessioni con marcatori e note |

## Specifiche

- **Framework:** Swift / SwiftUI nativo
- **iOS minimo:** 13.0
- **Dimensione:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, nessuna scrittura
- **DSP:** RMS, filtro A (IEC 61672 Tipo 2), Z, FFT 1024
- **Permessi:** Solo microfono. Niente Internet/posizione/contatti/fotocamera

## FAQ

**Davvero gratis?** Sì.
**Registra audio?** No.
**Precisione?** ±2 dB in 40–95 dB dopo calibrazione; non valido legalmente.
**Perché 35 dB in stanza "silenziosa"?** Rumore proprio del mic.
**Perché satura?** Mic iPhone satura ~110 dB.
**Export?** Sì — CSV serie temporale, PNG riepilogo.
**Perché solo iPhone?** Calibrare migliaia di modelli Android è oneroso.
**Cos'è LEQ?** Livello continuo equivalente — metrica standard del rumore.
**Per denunce legali?** Supporto informale sì; per procedure formali serve Classe 1/2.

## Download

| Piattaforma | Store | ID |
|-------------|-------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Non disponibile — solo iOS | — |

**Supporto:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Sullo sviluppatore

Realizzata da **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **Email:** tom@lapnito.cz
- **Altre app su App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Fatto con ❤️ in Repubblica Ceca da <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
