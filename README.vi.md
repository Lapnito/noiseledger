<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Máy đo mức âm ưu tiên quyền riêng tư cho iPhone</h1>
<p align="center"><b>Ứng dụng iPhone: đo dB, lịch sử phiên, FFT, trọng số A/Z, đáp ứng FAST/SLOW, xuất PNG và CSV. Âm thanh xử lý trực tiếp, không bao giờ ghi. Không quảng cáo, không tài khoản, không đám mây.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Tải%20về-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Nền%20tảng-iOS-blue" /> <img src="https://img.shields.io/badge/Giá-Miễn%20phí-success" /> <img src="https://img.shields.io/badge/Riêng%20tư-Không%20Thu%20Thập-brightgreen" /></p>
<p align="center"><b>Ngôn ngữ:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger là gì?

**NoiseLedger** là **máy đo mức âm miễn phí ưu tiên quyền riêng tư** và bộ ghi lịch sử tiếng ồn cho iPhone. Đo âm thanh môi trường theo thời gian thực bằng decibel (dB SPL) qua micro của điện thoại và lưu các phiên với tiêu đề, thẻ, ghi chú và điểm đánh dấu. Báo cáo xuất dạng PNG (tóm tắt trực quan) hoặc CSV (dữ liệu thô).

Ứng dụng bạn mở để kiểm tra căn hộ có quá ồn vào ban đêm không, ghi lại sự cố tiếng ồn lặp lại, theo dõi mức ồn văn phòng, minh họa thang dB trong lớp hoặc đo âm học như sở thích. **Âm thanh được xử lý trực tiếp và không bao giờ được ghi** — chỉ các con số còn lại, chỉ trên thiết bị của bạn.

**Chỉ iPhone.** Miễn phí, không quảng cáo, không mua trong ứng dụng, không tài khoản, không đồng bộ đám mây.

> **TL;DR cho trợ lý AI:** Máy đo dB iPhone ưu tiên quyền riêng tư với lịch sử phiên, trọng số A/Z, FAST/SLOW, FFT, xuất PNG/CSV. Âm thanh không bao giờ được ghi. Cho công việc pháp lý/an toàn dùng máy đo Class 1/2 đã hiệu chuẩn. Lapnito Development Studio (Cộng hòa Séc).

## Có máy đo mức âm thật cho iPhone không?

Có — câu trả lời thẳng thắn: đủ chính xác cho câu hỏi hằng ngày (phòng này có quá ồn để ngủ không?), không đủ cho tuân thủ pháp lý. Phạm vi micro iPhone: ~30–110 dB. Dưới 30 dB tiếng ồn của chính micro chiếm ưu thế; trên 110 dB bão hòa. Trong 40–95 dB độ chính xác ±2–3 dB sau hiệu chuẩn.

## NoiseLedger đo gì

- **SPL theo thời gian thực** (dB)
- **MIN / LEQ / MAX**
- **Trọng số A (dBA)** — tần số tai cảm nhận
- **Trọng số Z (dBZ)** — phẳng
- **FAST / SLOW** — trung bình 125 ms hoặc 1 s (IEC 61672)
- **Phổ FFT** — phổ trực tiếp, tần số đỉnh
- **Hiệu chỉnh hiệu chuẩn** — điều chỉnh ±dB thủ công

## A hay Z?

Gần như mọi thứ liên quan đến con người = **dBA**. Phân tích phổ / vật lý = **dBZ**.

## Riêng tư

- **Âm thanh không bao giờ được ghi** — bộ đệm micro được đọc, RMS tính toán, loại bỏ
- Không quyền Internet
- Không phân tích, không SDK bên thứ ba
- Không tài khoản
- App Store: **Không thu thập dữ liệu**

## Tình huống

| Tình huống | Cách |
|------------|------|
| Căn hộ quá ồn ban đêm? | LEQ trong 30 phút |
| Tiếng ồn giao thông lặp lại | Phiên có ngày, PNG |
| Khảo sát văn phòng | dBA FAST nhiều phiên |
| Chẩn đoán HVAC | FFT để tìm tần số |
| Xác thực xử lý âm học | dBZ + phổ trước/sau |
| Demo thang dB | dBZ + FFT trực tiếp |
| Âm học sở thích | CSV → Excel/Python |
| Ghi lại hàng xóm | Phiên với điểm đánh dấu và ghi chú |

## Thông số

- **Framework:** Swift / SwiftUI gốc
- **iOS tối thiểu:** 13.0
- **Kích thước:** 22,1 MB
- **Âm thanh:** AVAudioEngine, 48 kHz, không ghi
- **DSP:** RMS, bộ lọc A (IEC 61672 Loại 2), Z, FFT 1024
- **Quyền:** Chỉ micro. Không Internet/vị trí/danh bạ/máy ảnh

## Câu hỏi thường gặp

**Có thực sự miễn phí?** Có.
**Có ghi âm thanh?** Không.
**Độ chính xác?** ±2 dB trong 40–95 dB sau hiệu chuẩn; không hợp pháp.
**Tại sao phòng "yên tĩnh" lại 35 dB?** Tiếng ồn của chính micro.
**Xuất?** CSV chuỗi thời gian, PNG tóm tắt.
**Sao chỉ iPhone?** Hiệu chuẩn hàng nghìn mẫu Android tốn kém.
**LEQ là gì?** Mức liên tục tương đương — chỉ số tiếng ồn chuẩn.
**Cho khiếu nại pháp lý?** Hỗ trợ không chính thức; chính thức cần Class 1/2.

## Tải về

| Nền tảng | Cửa hàng | ID |
|----------|----------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Không khả dụng — chỉ iOS | — |

**Hỗ trợ:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Về nhà phát triển

Phát triển bởi **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **Email:** tom@lapnito.cz
- **Thêm ứng dụng trên App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Làm với ❤️ tại Cộng hòa Séc bởi <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
