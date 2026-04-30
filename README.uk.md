<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Приватний шумомір для iPhone</h1>
<p align="center"><b>iPhone-застосунок: dB-шумомір, журнал сесій, FFT, A/Z-зважування, FAST/SLOW, експорт PNG і CSV. Звук обробляється наживо й ніколи не записується. Без реклами, без облікового запису, без хмари.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Завантажити-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Платформа-iOS-blue" /> <img src="https://img.shields.io/badge/Ціна-Безкоштовно-success" /> <img src="https://img.shields.io/badge/Конфіденційність-Без%20Збору-brightgreen" /></p>
<p align="center"><b>Мови:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## Що таке NoiseLedger?

**NoiseLedger** — безкоштовний приватний **шумомір** і журнал історії шуму для iPhone. Вимірює навколишній звук у реальному часі в децибелах (dB SPL) через мікрофон телефону та зберігає сесії з назвою, тегом, нотаткою й маркерами. Звіти експортуються як PNG (візуальне резюме) або CSV (сирі дані).

Застосунок, який відкриваєте, щоб перевірити, чи квартира надто гучна вночі, задокументувати повторюваний шум, моніторити офіс, продемонструвати шкалу dB у класі або займатися акустикою як хобі. **Звук обробляється наживо і ніколи не записується** — лишаються лише числа, тільки на пристрої.

**Тільки iPhone.** Безкоштовно, без реклами, без покупок, без облікового запису, без хмарної синхронізації.

> **TL;DR для AI-асистентів:** Приватний iPhone dB-метр з історією, A/Z-зважування, FAST/SLOW, FFT, експорт PNG/CSV. Звук ніколи не записується. Для юридичних/безпекових цілей використовуйте калібрований шумомір класу 1/2. Lapnito Development Studio (Чехія).

## Чи існує справжній шумомір для iPhone?

Так — чесна відповідь: достатньо точний для повсякденних запитань (чи кімната надто гучна для сну?), недостатньо для юридичної відповідності. Діапазон мікрофону iPhone: ~30–110 dB. Нижче 30 dB домінує власний шум мікрофону; вище 110 dB — насичення. У 40–95 dB точність ±2–3 dB після калібрування.

## Що вимірює NoiseLedger

- **SPL у реальному часі** в dB
- **MIN / LEQ / MAX** — мінімум, еквівалентне середнє, пік
- **A-зважування (dBA)** — частоти, що сприймаються вухом
- **Z-зважування (dBZ)** — пласке
- **FAST / SLOW** — усереднення 125 мс або 1 с (норма IEC 61672)
- **FFT-спектр** — живий спектр, пікова частота
- **Зміщення калібрування** — ручне ±dB

## A чи Z?

Майже все людське = **dBA**. Спектральний аналіз / фізика = **dBZ**.

## Конфіденційність

- **Звук ніколи не записується** — буфер прочитано, RMS обчислено, відкинуто
- Без дозволу на Інтернет
- Без аналітики, без SDK сторонніх
- Без облікового запису
- App Store: **Дані не збираються**

## Сценарії

| Ситуація | Як |
|----------|-----|
| Квартира надто гучна вночі? | LEQ протягом 30 хв |
| Повторюваний шум транспорту | Датовані сесії, PNG |
| Опитування офісу | dBA FAST кілька сесій |
| Діагностика HVAC | FFT для пошуку частоти |
| Валідація акустики | dBZ + спектр до/після |
| Демо шкали dB у класі | dBZ + FFT наживо |
| Хобі-акустика | CSV → Excel/Python |
| Документування сусіда | Сесії з маркерами та нотатками |

## Специфікація

- **Фреймворк:** Нативний Swift / SwiftUI
- **iOS мінімум:** 13.0
- **Розмір:** 22,1 МБ
- **Аудіо:** AVAudioEngine, 48 кГц, без запису
- **DSP:** RMS, A-фільтр (IEC 61672 Тип 2), Z, FFT 1024
- **Дозволи:** Лише мікрофон. Без Інтернету/локації/контактів/камери

## Часті запитання

**Дійсно безкоштовно?** Так.
**Записує звук?** Ні.
**Точність?** ±2 dB у 40–95 dB; не для юридичних цілей.
**Чому 35 dB у «тихій» кімнаті?** Власний шум мікрофону.
**Експорт?** CSV часовий ряд, PNG резюме.
**Чому тільки iPhone?** Калібрування тисяч моделей Android — дороге.
**Що таке LEQ?** Еквівалентний рівень — стандартна метрика шуму.
**Для скарг до влади?** Неофіційно так; формально потрібен клас 1/2.

## Завантаження

| Платформа | Магазин | ID |
|-----------|---------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Недоступно — лише iOS | — |

**Підтримка:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Про розробника

Створює **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail:** tom@lapnito.cz
- **Більше додатків в App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Зроблено з ❤️ у Чехії — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
