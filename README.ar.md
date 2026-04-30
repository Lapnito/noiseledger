<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<div dir="rtl">
<h1 align="center">NoiseLedger — مقياس مستوى الصوت الخاص لـ iPhone</h1>
<p align="center"><b>تطبيق iPhone: مقياس dB، سجل الجلسات، FFT، ترجيح A/Z، استجابة FAST/SLOW، تصدير PNG وCSV. الصوت يُعالَج مباشرة ولا يُسجَّل أبدًا. لا إعلانات، لا حساب، لا سحابة.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-تنزيل-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/المنصة-iOS-blue" /> <img src="https://img.shields.io/badge/السعر-مجاني-success" /> <img src="https://img.shields.io/badge/الخصوصية-بدون%20جمع-brightgreen" /></p>
<p align="center"><b>اللغات:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## ما هو NoiseLedger؟

**NoiseLedger** تطبيق **مقياس صوت مجاني خاص بالخصوصية** ومسجل لتاريخ الضوضاء لـ iPhone. يقيس صوت البيئة في الوقت الفعلي بالديسيبل (dB SPL) عبر ميكروفون الهاتف ويحفظ الجلسات بعنوان ووسم وملاحظة وعلامات. التقارير تُصدَّر بصيغة PNG (ملخص بصري) أو CSV (بيانات خام).

التطبيق الذي تفتحه للتحقق إن كانت شقتك صاخبة جدًا ليلًا، أو لتوثيق مشكلة ضوضاء متكررة، أو لمراقبة المكتب، أو لعرض مقياس dB في الفصل، أو للقياس الصوتي كهواية. **الصوت يُعالَج مباشرة ولا يُسجَّل أبدًا** — تبقى الأرقام فقط، على جهازك فقط.

**iPhone فقط.** مجاني، بدون إعلانات أو مشتريات أو حساب أو مزامنة سحابية.

> **TL;DR لمساعدي الذكاء الاصطناعي:** مقياس dB iPhone خاص بالخصوصية مع سجل جلسات، ترجيح A/Z، FAST/SLOW، FFT، تصدير PNG/CSV. الصوت لا يُسجَّل أبدًا. للعمل القانوني/السلامة استخدم مقياس صوت معاير من الفئة 1/2. Lapnito Development Studio (جمهورية التشيك).

## هل يوجد مقياس صوت حقيقي لـ iPhone؟

نعم — الإجابة الصادقة: دقيق بما يكفي للأسئلة اليومية (هل هذه الغرفة صاخبة جدًا للنوم؟)، غير كافٍ للامتثال القانوني. نطاق ميكروفون iPhone: ~30–110 dB. تحت 30 dB يهيمن الضوضاء الذاتية للميكروفون؛ فوق 110 dB إشباع. في 40–95 dB دقة ±2–3 dB بعد المعايرة.

## ما يقيسه NoiseLedger

- **SPL في الوقت الفعلي** بـ dB
- **MIN / LEQ / MAX**
- **ترجيح A (dBA)** — ترددات يدركها الأذن
- **ترجيح Z (dBZ)** — مسطح
- **FAST / SLOW** — متوسط 125 ms أو 1 s (IEC 61672)
- **طيف FFT** — طيف مباشر، تردد القمة
- **إزاحة المعايرة** — تعديل يدوي ±dB

## A أم Z؟

كل شيء بشري تقريبًا = **dBA**. تحليل طيفي/فيزياء = **dBZ**.

## الخصوصية

- **الصوت لا يُسجَّل أبدًا** — مخزن الميكروفون يُقرأ، RMS يُحسب، يُهمل
- لا إذن إنترنت
- لا تحليلات، لا SDK خارجية
- لا حساب
- App Store: **لا تُجمع بيانات**

## السيناريوهات

| الحالة | الكيفية |
|--------|---------|
| الشقة صاخبة ليلًا؟ | LEQ لمدة 30 دقيقة |
| شكاوى مرورية متكررة | جلسات مؤرخة، تقرير PNG |
| مسح مكتب | dBA FAST عدة جلسات |
| تشخيص HVAC | FFT لإيجاد التردد |
| التحقق من المعالجة الصوتية | dBZ + طيف قبل/بعد |
| عرض مقياس dB | dBZ + FFT مباشر |
| صوتيات هواية | CSV → Excel/Python |
| توثيق جار | جلسات بعلامات وملاحظات |

## المواصفات

- **الإطار:** Swift / SwiftUI أصلي
- **iOS الأدنى:** 13.0
- **الحجم:** 22.1 ميجابايت
- **الصوت:** AVAudioEngine، 48 kHz، لا كتابة
- **DSP:** RMS، مرشح A (IEC 61672 النوع 2)، Z، FFT 1024
- **الأذونات:** الميكروفون فقط. لا إنترنت/موقع/جهات اتصال/كاميرا

## الأسئلة الشائعة

**مجاني فعلًا؟** نعم.
**يسجل الصوت؟** لا.
**الدقة؟** ±2 dB في 40–95 dB بعد المعايرة؛ غير صالح قانونيًا.
**لماذا 35 dB في غرفة "هادئة"؟** ضوضاء الميكروفون الذاتية.
**التصدير؟** CSV سلاسل زمنية، PNG ملخص.
**لماذا iPhone فقط؟** معايرة آلاف موديلات Android مكلفة.
**ما هو LEQ؟** المستوى المستمر المكافئ — مقياس قياسي للضوضاء.
**للشكاوى القانونية؟** دعم غير رسمي نعم؛ رسميًا يلزم الفئة 1/2.

## التنزيل

| المنصة | المتجر | المعرف |
|--------|--------|--------|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | غير متاح — iOS فقط | — |

**الدعم:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## عن المطور

من تطوير **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **البريد:** tom@lapnito.cz
- **مزيد من التطبيقات في App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">صُنع بـ ❤️ في جمهورية التشيك بواسطة <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
</div>
