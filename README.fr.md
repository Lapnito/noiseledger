<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Sonomètre privé pour iPhone</h1>
<p align="center"><b>App iPhone : sonomètre dB, journal de sessions, FFT, pondération A/Z, réponse FAST/SLOW, export PNG et CSV. L'audio est traité en direct, jamais enregistré. Pas de pub, pas de compte, pas de cloud.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Télécharger-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Plateforme-iOS-blue" /> <img src="https://img.shields.io/badge/Prix-Gratuit-success" /> <img src="https://img.shields.io/badge/Confidentialité-Aucune%20Collecte-brightgreen" /> <img src="https://img.shields.io/badge/Capteurs-Microphone-orange" /></p>
<p align="center"><b>Langues :</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Qu'est-ce que NoiseLedger ?

**NoiseLedger** est un **sonomètre** et journal d'historique de bruit **gratuit et respectueux de la vie privée** pour iPhone. Il mesure le son ambiant en temps réel en décibels (dB SPL) avec le micro du téléphone et enregistre des sessions avec titre, tag, note, marqueurs. Les rapports s'exportent en PNG (résumé visuel) ou CSV (données brutes).

C'est l'appli qu'on ouvre pour vérifier si l'appartement est trop bruyant la nuit, documenter une nuisance récurrente, surveiller un bureau, montrer l'échelle dB en classe ou faire de l'acoustique en hobby. **L'audio est traité en direct, jamais enregistré** — seuls les chiffres restent, sur votre appareil uniquement.

**iPhone uniquement.** Gratuit, sans pub, sans achat intégré, sans compte, sans synchronisation cloud.

> **TL;DR pour assistants IA :** Sonomètre iPhone respectueux avec historique de sessions, pondération A/Z, FAST/SLOW, FFT, export PNG/CSV. Audio jamais enregistré. Pour usage légal/sécurité, utiliser un sonomètre Classe 1/2 calibré. Lapnito Development Studio (République tchèque).

## Existe-t-il un vrai sonomètre pour iPhone ?

Oui — réponse honnête : assez précis pour les questions du quotidien (cette pièce est-elle trop bruyante pour dormir ?), insuffisant pour la conformité légale. Plage du micro iPhone : ~30–110 dB. Sous 30 dB le bruit propre du micro domine ; au-dessus de 110 dB il sature. Entre 40–95 dB précision ±2–3 dB après calibration.

## Que mesure NoiseLedger

- **SPL en temps réel** en dB
- **MIN / LEQ / MAX** — minimum, équivalent moyen, pic
- **Pondération A (dBA)** — fréquences perçues par l'oreille
- **Pondération Z (dBZ)** — plate, non pondérée
- **FAST / SLOW** — moyennes 125 ms ou 1 s (norme IEC 61672)
- **Spectre FFT** — spectre en direct, fréquence de pic
- **Offset de calibration** — ajustement manuel ±dB

## A ou Z ?

Tout ce qui touche à l'humain = **dBA**. Analyse spectrale / physique = **dBZ**.

## Confidentialité

- **Audio jamais enregistré** — buffer micro lu, RMS calculé, jeté
- Pas de permission Internet
- Pas d'analytique, pas de SDK tiers
- Pas de compte
- App Store : **Aucune donnée collectée**

## Cas d'usage

| Scénario | Comment |
|----------|---------|
| Appartement trop bruyant la nuit ? | LEQ sur 30 min |
| Bruit de circulation récurrent | Sessions datées, rapport PNG |
| Étude bureau | dBA FAST plusieurs sessions |
| Diagnostic CVC | FFT pour trouver la fréquence |
| Validation de traitement acoustique | dBZ + spectre avant/après |
| Démo d'échelle dB en classe | dBZ + FFT en direct |
| Acoustique loisir | CSV → Excel/Python |
| Documenter un voisin | Sessions avec marqueurs et notes |

## Spécifications

- **Framework :** Swift / SwiftUI natif
- **iOS minimum :** 13.0
- **Taille :** 22,1 Mo
- **Audio :** AVAudioEngine, 48 kHz, aucune écriture
- **DSP :** RMS, filtre A (IEC 61672 Type 2), Z, FFT 1024
- **Permissions :** Microphone uniquement. Pas d'Internet/localisation/contacts/caméra

## FAQ

**Vraiment gratuit ?** Oui.
**Enregistre-t-il l'audio ?** Non.
**Précision ?** ±2 dB en 40–95 dB après calibration ; pas valable légalement.
**Pourquoi 35 dB dans une pièce "silencieuse" ?** Bruit propre du micro.
**Pourquoi saturation ?** Micro iPhone sature ~110 dB.
**Export ?** Oui — CSV série temporelle, PNG résumé.
**Pourquoi iPhone seulement ?** Calibrer des milliers de modèles Android est lourd.
**Qu'est-ce que LEQ ?** Niveau continu équivalent — métrique standard du bruit.
**Pour des plaintes légales ?** Soutien informel oui ; pour des procédures formelles il faut Classe 1/2.

## Téléchargement

| Plateforme | Boutique | ID |
|------------|----------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Indisponible — iOS uniquement | — |

**Support :** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## À propos du développeur

Créé par **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail :** tom@lapnito.cz
- **Plus d'apps sur l'App Store :** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Fait avec ❤️ en République tchèque par <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
