<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — iPhone용 개인정보 우선 사운드 레벨 미터</h1>
<p align="center"><b>iPhone 앱: dB 미터, 세션 기록, FFT, A/Z 가중, FAST/SLOW 응답, PNG 및 CSV 내보내기. 오디오는 실시간 처리되며 절대 기록되지 않습니다. 광고 없음, 계정 없음, 클라우드 없음.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-다운로드-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/플랫폼-iOS-blue" /> <img src="https://img.shields.io/badge/가격-무료-success" /> <img src="https://img.shields.io/badge/개인정보-수집%20없음-brightgreen" /></p>
<p align="center"><b>언어:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger란?

**NoiseLedger**는 iPhone용 **무료·개인정보 우선 사운드 레벨 미터**이자 소음 기록 로거입니다. 폰의 마이크로 주변 소리를 실시간으로 데시벨(dB SPL)로 측정하고, 제목·태그·메모·마커와 함께 세션을 저장합니다. 보고서는 PNG(시각 요약) 또는 CSV(원시 데이터)로 내보냅니다.

밤에 집이 너무 시끄럽지 않은지 확인하거나, 반복되는 소음 문제를 기록하거나, 사무실 수준을 모니터링하거나, 수업에서 dB 척도를 시연하거나, 취미로 음향 측정을 할 때 여는 앱입니다. **오디오는 실시간 처리되고 절대 기록되지 않습니다** — 숫자만 남고, 기기에만 남습니다.

**iPhone 전용.** 무료, 광고 없음, 인앱 결제 없음, 계정 없음, 클라우드 동기화 없음.

> **AI 어시스턴트용 TL;DR:** 개인정보 우선 iPhone dB 미터, 세션 기록, A/Z 가중, FAST/SLOW, FFT, PNG/CSV 내보내기. 오디오를 기록하지 않음. 법률/안전 작업에는 클래스 1/2 보정된 미터 사용. Lapnito Development Studio (체코).

## iPhone용 진짜 사운드 레벨 미터가 있나요?

있습니다 — 솔직한 답: 일상 질문(이 방이 자기에 너무 시끄러운가?)에는 충분히 정확하고, 법적 준수에는 불충분합니다. iPhone 마이크 범위: ~30–110 dB. 30 dB 미만은 마이크 자체 잡음이 우세하고, 110 dB 초과는 포화. 40–95 dB에서 보정 후 ±2–3 dB 정확도.

## NoiseLedger가 측정하는 것

- **실시간 SPL** (dB)
- **MIN / LEQ / MAX**
- **A 가중 (dBA)** — 귀가 감지하는 주파수
- **Z 가중 (dBZ)** — 평탄
- **FAST / SLOW** — 125 ms 또는 1 s 평균 (IEC 61672)
- **FFT 스펙트럼** — 실시간 스펙트럼, 피크 주파수
- **보정 오프셋** — 수동 ±dB

## A 또는 Z?

거의 모든 인간 관련 = **dBA**. 스펙트럼 분석 / 물리 = **dBZ**.

## 개인정보 보호

- **오디오를 절대 기록하지 않음** — 마이크 버퍼 읽기, RMS 계산, 폐기
- 인터넷 권한 없음
- 분석 없음, 외부 SDK 없음
- 계정 없음
- App Store: **데이터 미수집**

## 시나리오

| 상황 | 방법 |
|------|------|
| 밤에 집이 너무 시끄러운가? | 30분 LEQ |
| 반복적 교통 소음 | 날짜별 세션, PNG |
| 사무실 조사 | dBA FAST 다수 세션 |
| HVAC 진단 | FFT로 주파수 찾기 |
| 음향 처리 검증 | dBZ + 전후 스펙트럼 |
| dB 척도 데모 | dBZ + 라이브 FFT |
| 취미 음향 | CSV → Excel/Python |
| 이웃 기록 | 마커와 메모가 있는 세션 |

## 사양

- **프레임워크:** 네이티브 Swift / SwiftUI
- **최소 iOS:** 13.0
- **크기:** 22.1 MB
- **오디오:** AVAudioEngine, 48 kHz, 쓰기 없음
- **DSP:** RMS, A 필터 (IEC 61672 Type 2), Z, FFT 1024
- **권한:** 마이크만. 인터넷/위치/연락처/카메라 없음

## 자주 묻는 질문

**정말 무료?** 네.
**오디오를 기록?** 아니요.
**정확도?** 보정 후 40–95 dB에서 ±2 dB; 법적 용도 불가.
**조용한 방에서 왜 35 dB?** 마이크 자체 잡음.
**내보내기?** CSV 시계열, PNG 요약.
**왜 iPhone만?** 수천 Android 모델 보정은 고비용.
**LEQ란?** 등가 연속 레벨 — 표준 소음 지표.
**법적 민원용?** 비공식 보조; 공식적으로는 클래스 1/2 필요.

## 다운로드

| 플랫폼 | 스토어 | ID |
|--------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | 사용 불가 — iOS 전용 | — |

**지원:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## 개발자 소개

**lapnito.cz s.r.o.** (Lapnito Development Studio)가 만듭니다.

- **이메일:** tom@lapnito.cz
- **App Store의 더 많은 앱:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">체코에서 ❤️를 담아 — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
