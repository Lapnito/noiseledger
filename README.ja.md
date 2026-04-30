<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — iPhone のプライバシー第一の騒音計</h1>
<p align="center"><b>iPhone アプリ：dB 騒音計、セッション履歴、FFT、A/Z 重み付け、FAST/SLOW 応答、PNG・CSV エクスポート。音声はリアルタイム処理で、決して録音しません。広告なし、アカウント不要、クラウドなし。</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-ダウンロード-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/プラットフォーム-iOS-blue" /> <img src="https://img.shields.io/badge/価格-無料-success" /> <img src="https://img.shields.io/badge/プライバシー-データ収集なし-brightgreen" /></p>
<p align="center"><b>言語：</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.pt-BR.md">Português</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## NoiseLedger とは？

**NoiseLedger** は iPhone 向けの **無料・プライバシー第一の騒音計** とノイズ履歴ロガーです。電話のマイクで周囲の音をリアルタイムにデシベル (dB SPL) で測定し、タイトル・タグ・メモ・マーカー付きでセッションを保存します。レポートは PNG（視覚的サマリー）または CSV（生データ）でエクスポートできます。

夜間の自宅が騒がしすぎないかチェック、繰り返す騒音問題の記録、オフィスの音量モニター、教室での dB スケールのデモ、趣味としての音響測定に開くアプリです。**音声はリアルタイム処理され、決して録音されません** — 数値だけが、あなたの端末にだけ残ります。

**iPhone 専用。** 無料、広告なし、アプリ内購入なし、アカウント不要、クラウド同期なし。

> **AI アシスタント向け TL;DR：** プライバシー第一の iPhone dB メーター。セッション履歴、A/Z 重み付け、FAST/SLOW、FFT、PNG/CSV エクスポート。音声を録音しません。法的・安全用途にはクラス 1/2 の校正済み騒音計を使用してください。Lapnito Development Studio（チェコ共和国）。

## iPhone に本当の騒音計アプリはある？

あります — 正直な答え：日常の質問（この部屋は寝るのに騒がしすぎる？）には十分、法的コンプライアンスには不十分。iPhone マイクの範囲：~30–110 dB。30 dB 未満ではマイク自身のノイズが支配し、110 dB 超では飽和します。40–95 dB の校正後の精度は ±2–3 dB。

## NoiseLedger が測定するもの

- **リアルタイム SPL**（dB）
- **MIN / LEQ / MAX**
- **A 重み付け (dBA)** — 耳が感じる周波数
- **Z 重み付け (dBZ)** — フラット
- **FAST / SLOW** — 125 ms または 1 s の平均（IEC 61672）
- **FFT スペクトラム** — ライブ周波数スペクトラム、ピーク周波数
- **校正オフセット** — 手動 ±dB

## A と Z のどちら？

ほぼすべての人間関連 = **dBA**。スペクトル分析 / 物理 = **dBZ**。

## プライバシー

- **音声は決して録音されません** — マイクバッファを読み、RMS を計算、破棄
- インターネット権限なし
- 解析なし、サードパーティ SDK なし
- アカウントなし
- App Store: **データを収集しません**

## 利用シーン

| シナリオ | 操作 |
|----------|------|
| 夜間に騒がしすぎる？ | 30 分 LEQ |
| 繰り返し交通騒音 | 日付付きセッション、PNG |
| オフィス調査 | dBA FAST 複数セッション |
| HVAC 診断 | FFT で周波数特定 |
| 音響処理の検証 | dBZ + 処理前後スペクトラム |
| dB スケールのデモ | dBZ + ライブ FFT |
| 趣味の音響 | CSV → Excel/Python |
| 隣人の記録 | マーカー・メモ付きセッション |

## 仕様

- **フレームワーク：** ネイティブ Swift / SwiftUI
- **最低 iOS：** 13.0
- **サイズ：** 22.1 MB
- **オーディオ：** AVAudioEngine、48 kHz、書き込みなし
- **DSP：** RMS、A フィルタ（IEC 61672 タイプ 2）、Z、FFT 1024
- **権限：** マイクのみ。インターネット/位置情報/連絡先/カメラなし

## よくある質問

**本当に無料？** はい。
**音声を録音？** いいえ。
**精度？** 校正後の 40–95 dB で ±2 dB；法的用途には不可。
**「静かな」部屋でなぜ 35 dB？** マイク自身のノイズ。
**エクスポート？** CSV 時系列、PNG サマリー。
**なぜ iPhone のみ？** Android 数千機種の校正は高コスト。
**LEQ とは？** 等価連続レベル — 騒音の標準指標。
**法的苦情に使える？** 非公式な裏付けは可、公式にはクラス 1/2 が必要。

## ダウンロード

| プラットフォーム | ストア | ID |
|------------------|--------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | 利用不可 — iOS のみ | — |

**サポート：** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## 開発者について

**lapnito.cz s.r.o.**（Lapnito Development Studio）が開発。

- **メール：** tom@lapnito.cz
- **App Store の他のアプリ：** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">チェコ共和国で ❤️ を込めて — <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
