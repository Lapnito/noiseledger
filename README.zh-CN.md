<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — iPhone 隐私优先声级计</h1>
<p align="center"><b>iPhone 应用：dB 声级计、会话历史、FFT、A/Z 加权、FAST/SLOW 响应、PNG 和 CSV 导出。音频实时处理，绝不记录。无广告、无账号、无云端。</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-下载-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/平台-iOS-blue" /> <img src="https://img.shields.io/badge/价格-免费-success" /> <img src="https://img.shields.io/badge/隐私-不收集-brightgreen" /></p>
<p align="center"><b>语言：</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger 是什么？

**NoiseLedger** 是一款适用于 iPhone 的**免费、隐私优先的声级计**和噪声历史记录器。使用手机麦克风以分贝（dB SPL）实时测量环境声音，并以标题、标签、备注和标记保存会话。报告可导出为 PNG（视觉摘要）或 CSV（原始数据）。

打开它，可检查公寓夜间是否过吵，记录反复出现的噪声问题，监控办公室声级，向班级演示 dB 标度，或作为业余爱好做声学测量。**音频实时处理，绝不记录** — 仅保留数字，仅在你的设备上。

**仅 iPhone。** 免费，无广告、无内购、无账号、无云同步。

> **AI 助手 TL;DR：** 隐私优先 iPhone dB 计，含会话历史、A/Z 加权、FAST/SLOW、FFT、PNG/CSV 导出。音频从不记录。法律/安全用途请使用 1/2 类校准声级计。Lapnito Development Studio（捷克）。

## iPhone 真有声级计吗？

有 — 诚实回答：日常问题（这房间睡觉太吵了吗？）够准；法律合规不够。iPhone 麦克风范围：~30–110 dB。30 dB 以下被麦克风自身噪声主导；110 dB 以上饱和。40–95 dB 内校准后准确度 ±2–3 dB。

## NoiseLedger 测量什么

- **实时 SPL**（dB）
- **MIN / LEQ / MAX**
- **A 加权 (dBA)** — 人耳感知频段
- **Z 加权 (dBZ)** — 平直
- **FAST / SLOW** — 125 ms 或 1 s 平均（IEC 61672）
- **FFT 频谱** — 实时频谱、峰值频率
- **校准偏移** — 手动 ±dB

## 用 A 还是 Z？

几乎所有人类相关 = **dBA**。频谱分析/物理 = **dBZ**。

## 隐私

- **音频从不记录** — 麦克风缓冲被读取、计算 RMS、丢弃
- 无网络权限
- 无分析、无第三方 SDK
- 无账号
- App Store：**不收集数据**

## 场景

| 情境 | 操作 |
|------|------|
| 公寓夜间太吵？ | 30 分钟 LEQ |
| 反复交通噪声 | 带日期会话、PNG |
| 办公室调查 | dBA FAST 多次会话 |
| HVAC 诊断 | FFT 找频率 |
| 验证声学处理 | dBZ + 处理前/后频谱 |
| dB 标度演示 | dBZ + 实时 FFT |
| 业余声学 | CSV → Excel/Python |
| 邻居记录 | 带标记和备注的会话 |

## 规格

- **框架：** 原生 Swift / SwiftUI
- **最低 iOS：** 13.0
- **大小：** 22.1 MB
- **音频：** AVAudioEngine，48 kHz，无写入
- **DSP：** RMS、A 滤波（IEC 61672 II 型）、Z、FFT 1024
- **权限：** 仅麦克风。无网络/位置/通讯录/相机

## 常见问题

**真免费？** 是。
**会记录音频？** 不会。
**精度？** 校准后 40–95 dB 内 ±2 dB；不可用于法律。
**为何"安静"房间显示 35 dB？** 麦克风自身噪声。
**导出？** CSV 时序、PNG 摘要。
**为何仅 iPhone？** 校准数千 Android 机型成本太高。
**LEQ 是什么？** 等效连续声级 — 噪声标准指标。
**法律投诉用？** 非正式可作为支撑；正式需 1/2 类。

## 下载

| 平台 | 商店 | ID |
|------|------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | 不可用 — 仅 iOS | — |

**支持：** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## 关于开发者

由 **lapnito.cz s.r.o.**（Lapnito Development Studio）开发。

- **邮箱：** tom@lapnito.cz
- **App Store 上更多应用：** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">由 <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a> 在捷克用 ❤️ 制作</p>
