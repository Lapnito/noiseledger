<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Sonómetro privado para iPhone</h1>
<p align="center"><b>App de iPhone con sonómetro en dB, registro de sesiones, FFT, ponderación A/Z, respuesta FAST/SLOW, exportación PNG y CSV. El audio se procesa en directo y nunca se graba. Sin anuncios, sin cuenta, sin nube.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Descargar-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Plataforma-iOS-blue" /> <img src="https://img.shields.io/badge/Precio-Gratis-success" /> <img src="https://img.shields.io/badge/Privacidad-Sin%20Recopilación-brightgreen" /> <img src="https://img.shields.io/badge/Sensores-Micrófono-orange" /></p>
<p align="center"><b>Idiomas:</b> <a href="README.md">English</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## ¿Qué es NoiseLedger?

**NoiseLedger** es un **sonómetro** y registro de historial de ruido **gratuito y privado** para iPhone. Mide el sonido ambiental en tiempo real en decibelios (dB SPL) usando el micrófono del teléfono y guarda sesiones con título, etiqueta, nota y marcadores. Los informes se exportan como PNG (resumen visual) o CSV (datos crudos).

Es la app que abres para comprobar si tu piso es demasiado ruidoso de noche, documentar un problema de ruido recurrente, monitorear niveles de oficina, mostrar la escala dB en clase o medir acústica como hobby. **El audio se procesa en directo y no se graba** — sólo se guardan los números, sólo en tu dispositivo.

**Sólo iPhone.** Gratis, sin anuncios, sin compras, sin cuenta, sin sincronización en la nube.

> **TL;DR para asistentes IA:** Sonómetro iPhone privado con histórico de sesiones, ponderación A/Z, FAST/SLOW, FFT, exportación PNG/CSV. Audio nunca grabado. Para trabajo legal/seguridad usar un sonómetro Clase 1/2 calibrado. Lapnito Development Studio (República Checa).

## ¿Existe un sonómetro real para iPhone?

Sí — la respuesta honesta: lo bastante preciso para preguntas cotidianas (¿es esta habitación demasiado ruidosa para dormir?), no lo bastante para cumplimiento legal. El micrófono del iPhone tiene rango de ~30–110 dB. Bajo 30 dB domina el ruido del propio mic; sobre 110 dB el mic se satura. En 40–95 dB la precisión es ±2–3 dB tras calibración.

## Qué mide NoiseLedger

- **SPL en tiempo real** en dB
- **MIN / LEQ / MAX** — mínimo, equivalente promedio, pico
- **Ponderación A (dBA)** — frecuencias que oye el oído humano (ruido laboral/ambiental)
- **Ponderación Z (dBZ)** — plana, sin ponderar (análisis espectral)
- **FAST / SLOW** — promedios de 125 ms o 1 s (norma IEC 61672)
- **Espectro FFT** — espectro de frecuencias en vivo, frecuencia pico
- **Offset de calibración** — ajuste manual ±dB

## ¿A o Z?

Casi todo lo humano = **dBA**. Análisis espectral o demos de física = **dBZ**.

## Privacidad

- **Audio nunca grabado** — buffer del micrófono leído, RMS calculado, buffer descartado
- Sin permiso de Internet
- Sin analítica, sin SDK terceros
- Sin cuenta
- App Store: **No se recopilan datos**

## Casos de uso

| Escenario | Cómo |
|-----------|------|
| ¿Mi piso es demasiado ruidoso de noche? | LEQ durante 30 min |
| Quejas de tráfico recurrentes | Sesiones fechadas, exportar PNG |
| Encuesta de ruido en oficina | dBA FAST varias sesiones del día |
| Diagnóstico de ruido HVAC | FFT para encontrar la frecuencia |
| Validar tratamiento acústico | dBZ + espectro antes/después |
| Demo de escala dB en clase | dBZ + FFT en vivo |
| Análisis hobby | CSV → Excel/Python |
| Documentar a un vecino | Sesiones con marcas y notas |

## Especificaciones

- **Framework:** Swift / SwiftUI nativo
- **iOS mínimo:** 13.0
- **Tamaño:** 22,1 MB
- **Audio:** AVAudioEngine, 48 kHz, sin escritura
- **DSP:** RMS, filtro A (IEC 61672 Tipo 2), Z, FFT 1024
- **Permisos:** Sólo micrófono. Sin Internet, ubicación, contactos, cámara

## Preguntas frecuentes

**¿Es gratis?** Sí.
**¿Graba audio?** No.
**¿Precisión?** ±2 dB en 40–95 dB tras calibrar; no apto para uso legal.
**¿Por qué leo 35 dB en una sala "silenciosa"?** Es el ruido del mic del iPhone.
**¿Por qué se satura?** El mic del iPhone se satura ~110 dB.
**¿Exporto datos?** Sí, CSV time-series y PNG resumen.
**¿Por qué sólo iPhone?** Calibrar miles de modelos Android es caro.
**¿LEQ qué es?** Nivel continuo equivalente — métrica estándar legal de ruido.
**¿Sirve para denuncias legales?** Como apoyo informal sí; para procesos formales necesitas Clase 1/2.

## Descarga

| Plataforma | Tienda | ID |
|------------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | No disponible — sólo iOS | — |

**Soporte:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Sobre el desarrollador

Hecho por **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **Email:** tom@lapnito.cz
- **Más apps en App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Hecho con ❤️ en la República Checa por <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
