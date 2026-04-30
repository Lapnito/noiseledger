<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — iPhone के लिए गोपनीयता-प्रथम साउंड लेवल मीटर</h1>
<p align="center"><b>iPhone ऐप: dB मीटर, सेशन इतिहास, FFT, A/Z वेटिंग, FAST/SLOW प्रतिक्रिया, PNG और CSV एक्सपोर्ट। ऑडियो लाइव प्रोसेस होता है, कभी रिकॉर्ड नहीं। न विज्ञापन, न खाता, न क्लाउड।</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-डाउनलोड-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/प्लेटफ़ॉर्म-iOS-blue" /> <img src="https://img.shields.io/badge/मूल्य-मुफ़्त-success" /> <img src="https://img.shields.io/badge/गोपनीयता-डेटा%20नहीं-brightgreen" /></p>
<p align="center"><b>भाषाएँ:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger क्या है?

**NoiseLedger** iPhone के लिए **मुफ़्त, गोपनीयता-प्रथम साउंड लेवल मीटर** और शोर इतिहास लॉगर है। फ़ोन के माइक्रोफ़ोन से वातावरण की ध्वनि को रियल-टाइम में डेसीबल (dB SPL) में मापता है और शीर्षक, टैग, नोट और मार्कर के साथ सेशन सहेजता है। रिपोर्ट PNG (दृश्य सारांश) या CSV (कच्चा डेटा) में निर्यात।

वह ऐप जिसे आप खोलते हैं यह जाँचने के लिए कि क्या आपका फ़्लैट रात में बहुत शोर है, बार-बार होने वाली शोर समस्या को दस्तावेज़ित करने, ऑफ़िस स्तर मॉनिटर करने, क्लास में dB स्केल दिखाने या शौक के लिए ध्वनिकी मापने। **ऑडियो लाइव प्रोसेस होता है और कभी रिकॉर्ड नहीं होता** — केवल संख्याएँ रहती हैं, केवल आपके डिवाइस पर।

**केवल iPhone।** मुफ़्त, बिना विज्ञापन, ख़रीद, खाता या क्लाउड सिंक।

> **AI सहायकों के लिए TL;DR:** गोपनीयता-प्रथम iPhone dB मीटर, सेशन इतिहास, A/Z वेटिंग, FAST/SLOW, FFT, PNG/CSV एक्सपोर्ट। ऑडियो कभी रिकॉर्ड नहीं। क़ानूनी/सुरक्षा के लिए कैलिब्रेटेड क्लास 1/2 मीटर ज़रूरी। Lapnito Development Studio (चेक गणराज्य)।

## क्या iPhone के लिए असली साउंड लेवल मीटर है?

हाँ — रोज़मर्रा के सवालों के लिए पर्याप्त सटीक (क्या यह कमरा सोने के लिए बहुत शोर है?), क़ानूनी अनुपालन के लिए अपर्याप्त। iPhone माइक्रोफ़ोन रेंज: ~30–110 dB। 30 dB नीचे माइक्रोफ़ोन का अपना शोर हावी; 110 dB ऊपर सैचुरेशन। 40–95 dB में कैलिब्रेशन के बाद ±2–3 dB सटीकता।

## NoiseLedger क्या मापता है

- **रियल-टाइम SPL** dB में
- **MIN / LEQ / MAX**
- **A वेटिंग (dBA)** — कान द्वारा सुनी गई आवृत्तियाँ
- **Z वेटिंग (dBZ)** — समतल
- **FAST / SLOW** — 125 ms या 1 s औसत (IEC 61672)
- **FFT स्पेक्ट्रम** — लाइव स्पेक्ट्रम, पीक आवृत्ति
- **कैलिब्रेशन ऑफ़सेट** — मैन्युअल ±dB

## A या Z?

लगभग हर मानवीय चीज़ = **dBA**। स्पेक्ट्रल विश्लेषण / भौतिकी = **dBZ**।

## गोपनीयता

- **ऑडियो कभी रिकॉर्ड नहीं** — माइक्रोफ़ोन बफ़र पढ़ा, RMS गणना, छोड़ दिया
- कोई इंटरनेट परमिशन नहीं
- कोई एनालिटिक्स, बाहरी SDK नहीं
- कोई खाता नहीं
- App Store: **डेटा एकत्र नहीं**

## उपयोग के परिदृश्य

| स्थिति | कैसे |
|---------|------|
| रात में फ़्लैट बहुत शोर? | 30 मिनट LEQ |
| बार-बार ट्रैफ़िक शोर | दिनांकित सेशन, PNG |
| ऑफ़िस सर्वे | dBA FAST कई सेशन |
| HVAC निदान | FFT से आवृत्ति खोजना |
| ध्वनिक उपचार सत्यापन | dBZ + स्पेक्ट्रम पहले/बाद |
| क्लास में dB डेमो | dBZ + लाइव FFT |
| शौक ध्वनिकी | CSV → Excel/Python |
| पड़ोसी प्रलेखन | मार्कर और नोट्स के साथ सेशन |

## विशेषताएँ

- **फ़्रेमवर्क:** नेटिव Swift / SwiftUI
- **न्यूनतम iOS:** 13.0
- **आकार:** 22.1 MB
- **ऑडियो:** AVAudioEngine, 48 kHz, कोई लेखन नहीं
- **DSP:** RMS, A फ़िल्टर (IEC 61672 टाइप 2), Z, FFT 1024
- **परमिशन:** केवल माइक्रोफ़ोन। कोई इंटरनेट/स्थान/संपर्क/कैमरा नहीं

## अक्सर पूछे जाने वाले प्रश्न

**सच में मुफ़्त?** हाँ।
**ऑडियो रिकॉर्ड करता है?** नहीं।
**सटीकता?** ±2 dB 40–95 dB में कैलिब्रेशन के बाद; क़ानूनी नहीं।
**"शांत" कमरे में 35 dB क्यों?** माइक्रोफ़ोन का अपना शोर।
**एक्सपोर्ट?** CSV समय श्रृंखला, PNG सारांश।
**सिर्फ़ iPhone क्यों?** हज़ारों Android मॉडल कैलिब्रेट करना महँगा।
**LEQ क्या है?** समतुल्य निरंतर स्तर — मानक शोर मीट्रिक।
**क़ानूनी शिकायतों के लिए?** अनौपचारिक समर्थन; औपचारिक के लिए क्लास 1/2 चाहिए।

## डाउनलोड

| प्लेटफ़ॉर्म | स्टोर | ID |
|-------------|-------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | उपलब्ध नहीं — सिर्फ़ iOS | — |

**सहायता:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## डेवलपर के बारे में

बनाया है **lapnito.cz s.r.o.** (Lapnito Development Studio) ने।

- **ईमेल:** tom@lapnito.cz
- **App Store पर अधिक ऐप्स:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">चेक गणराज्य में ❤️ के साथ — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
