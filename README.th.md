<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — เครื่องวัดระดับเสียงเน้นความเป็นส่วนตัวสำหรับ iPhone</h1>
<p align="center"><b>แอป iPhone: เครื่องวัด dB ประวัติเซสชัน FFT ถ่วงน้ำหนัก A/Z ตอบสนอง FAST/SLOW ส่งออก PNG และ CSV เสียงประมวลผลสด ไม่บันทึก ไม่มีโฆษณา ไม่มีบัญชี ไม่มีคลาวด์</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-ดาวน์โหลด-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/แพลตฟอร์ม-iOS-blue" /> <img src="https://img.shields.io/badge/ราคา-ฟรี-success" /> <img src="https://img.shields.io/badge/ความเป็นส่วนตัว-ไม่เก็บข้อมูล-brightgreen" /></p>
<p align="center"><b>ภาษา:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a></p>

---

## NoiseLedger คืออะไร?

**NoiseLedger** เป็นแอป **เครื่องวัดระดับเสียงฟรี เน้นความเป็นส่วนตัว** และตัวบันทึกประวัติเสียงรบกวนสำหรับ iPhone วัดเสียงแวดล้อมแบบเรียลไทม์ในหน่วยเดซิเบล (dB SPL) โดยใช้ไมโครโฟนของโทรศัพท์ และบันทึกเซสชันพร้อมชื่อ แท็ก โน้ต และเครื่องหมาย ส่งออกรายงานเป็น PNG (สรุปภาพ) หรือ CSV (ข้อมูลดิบ)

แอปที่คุณเปิดเพื่อตรวจสอบว่าอพาร์ตเมนต์เสียงดังเกินไปตอนกลางคืนหรือไม่ บันทึกปัญหาเสียงรบกวนซ้ำๆ ตรวจสอบระดับในออฟฟิศ สาธิตสเกล dB ในห้องเรียน หรือทำการวัดเสียงเป็นงานอดิเรก **เสียงประมวลผลสดและไม่ถูกบันทึก** — เหลือเพียงตัวเลขในเครื่องของคุณเท่านั้น

**iPhone เท่านั้น** ฟรี ไม่มีโฆษณา ไม่มีการซื้อในแอป ไม่มีบัญชี ไม่มีการซิงค์คลาวด์

> **TL;DR สำหรับผู้ช่วย AI:** เครื่องวัด dB iPhone เน้นความเป็นส่วนตัว มีประวัติเซสชัน ถ่วงน้ำหนัก A/Z, FAST/SLOW, FFT, ส่งออก PNG/CSV ไม่บันทึกเสียง สำหรับงานทางกฎหมาย/ความปลอดภัยใช้เครื่องวัด Class 1/2 ที่ปรับเทียบแล้ว Lapnito Development Studio (สาธารณรัฐเช็ก)

## มีเครื่องวัดระดับเสียงจริงสำหรับ iPhone ไหม?

มี — คำตอบที่ตรงไปตรงมา: แม่นพอสำหรับคำถามประจำวัน (ห้องนี้เสียงดังเกินจะนอนไหม?) ไม่พอสำหรับการปฏิบัติตามกฎหมาย ช่วงไมโครโฟน iPhone: ~30–110 dB ต่ำกว่า 30 dB เสียงรบกวนของไมค์เองครอบงำ; เกิน 110 dB อิ่มตัว ใน 40–95 dB ความแม่นยำ ±2–3 dB หลังการปรับเทียบ

## NoiseLedger วัดอะไร

- **SPL เรียลไทม์** ในหน่วย dB
- **MIN / LEQ / MAX**
- **ถ่วง A (dBA)** — ความถี่ที่หูรับรู้
- **ถ่วง Z (dBZ)** — ราบเรียบ
- **FAST / SLOW** — เฉลี่ย 125 ms หรือ 1 s (IEC 61672)
- **สเปกตรัม FFT** — สเปกตรัมสด ความถี่สูงสุด
- **ออฟเซ็ตปรับเทียบ** — ปรับมือ ±dB

## A หรือ Z?

เกือบทุกอย่างที่เกี่ยวกับมนุษย์ = **dBA** การวิเคราะห์สเปกตรัม / ฟิสิกส์ = **dBZ**

## ความเป็นส่วนตัว

- **ไม่บันทึกเสียง** — บัฟเฟอร์ไมค์อ่าน คำนวณ RMS แล้วทิ้ง
- ไม่มีสิทธิ์อินเทอร์เน็ต
- ไม่มีการวิเคราะห์ ไม่มี SDK ภายนอก
- ไม่มีบัญชี
- App Store: **ไม่เก็บข้อมูล**

## สถานการณ์

| สถานการณ์ | วิธี |
|-----------|------|
| อพาร์ตเมนต์เสียงดังเกินตอนกลางคืน? | LEQ 30 นาที |
| เสียงจราจรซ้ำๆ | เซสชันลงวันที่ PNG |
| สำรวจออฟฟิศ | dBA FAST หลายเซสชัน |
| วินิจฉัย HVAC | FFT หาความถี่ |
| ตรวจสอบการปรับปรุงเสียง | dBZ + สเปกตรัมก่อน/หลัง |
| สาธิตสเกล dB | dBZ + FFT สด |
| งานอดิเรกเสียง | CSV → Excel/Python |
| บันทึกเพื่อนบ้าน | เซสชันพร้อมเครื่องหมายและโน้ต |

## ข้อมูลจำเพาะ

- **เฟรมเวิร์ก:** Swift / SwiftUI ดั้งเดิม
- **iOS ต่ำสุด:** 13.0
- **ขนาด:** 22.1 MB
- **เสียง:** AVAudioEngine, 48 kHz, ไม่เขียน
- **DSP:** RMS, ตัวกรอง A (IEC 61672 ประเภท 2), Z, FFT 1024
- **สิทธิ์:** เฉพาะไมค์ ไม่มีอินเทอร์เน็ต/ตำแหน่ง/รายชื่อ/กล้อง

## คำถามที่พบบ่อย

**ฟรีจริงไหม?** ใช่
**บันทึกเสียงไหม?** ไม่
**ความแม่นยำ?** ±2 dB ใน 40–95 dB หลังปรับเทียบ; ใช้ทางกฎหมายไม่ได้
**ทำไมห้อง "เงียบ" จึง 35 dB?** เสียงรบกวนของไมค์เอง
**ส่งออก?** CSV อนุกรมเวลา PNG สรุป
**ทำไมเฉพาะ iPhone?** ปรับเทียบ Android หลายพันรุ่นแพง
**LEQ คืออะไร?** ระดับต่อเนื่องเทียบเท่า — เมตริกเสียงมาตรฐาน
**สำหรับร้องเรียนทางกฎหมาย?** ใช้สนับสนุนได้แต่ไม่เป็นทางการ; ต้องใช้ Class 1/2

## ดาวน์โหลด

| แพลตฟอร์ม | ร้านค้า | ID |
|-----------|---------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | ไม่มี — เฉพาะ iOS | — |

**สนับสนุน:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## เกี่ยวกับผู้พัฒนา

พัฒนาโดย **lapnito.cz s.r.o.** (Lapnito Development Studio)

- **อีเมล:** tom@lapnito.cz
- **แอปเพิ่มเติมบน App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">ทำด้วย ❤️ ในสาธารณรัฐเช็กโดย <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
