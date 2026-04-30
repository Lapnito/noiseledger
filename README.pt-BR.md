<p align="center"><img src="assets/icon.png" alt="NoiseLedger" width="120" height="120" /></p>
<h1 align="center">NoiseLedger — Decibelímetro privado para iPhone</h1>
<p align="center"><b>App iPhone com decibelímetro em dB, registro de sessões, FFT, ponderação A/Z, resposta FAST/SLOW, exportação PNG e CSV. O áudio é processado ao vivo e nunca é gravado. Sem anúncios, sem conta, sem nuvem.</b></p>
<p align="center"><a href="https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003"><img src="https://img.shields.io/badge/App%20Store-Baixar-0D96F6?style=for-the-badge&logo=app-store&logoColor=white" /></a></p>
<p align="center"><img src="https://img.shields.io/badge/Plataforma-iOS-blue" /> <img src="https://img.shields.io/badge/Preço-Grátis-success" /> <img src="https://img.shields.io/badge/Privacidade-Sem%20Coleta-brightgreen" /> <img src="https://img.shields.io/badge/Sensores-Microfone-orange" /></p>
<p align="center"><b>Idiomas:</b> <a href="README.md">English</a> · <a href="README.es.md">Español</a> · <a href="README.de.md">Deutsch</a> · <a href="README.fr.md">Français</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a> · <a href="README.pl.md">Polski</a> · <a href="README.cs.md">Čeština</a> · <a href="README.uk.md">Українська</a> · <a href="README.ru.md">Русский</a> · <a href="README.tr.md">Türkçe</a> · <a href="README.ar.md">العربية</a> · <a href="README.hi.md">हिन्दी</a> · <a href="README.zh-CN.md">中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.id.md">Bahasa Indonesia</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.th.md">ภาษาไทย</a></p>

---

## O que é o NoiseLedger?

**NoiseLedger** é um **decibelímetro** e registro de histórico de ruído **gratuito e privado** para iPhone. Mede o som ambiente em tempo real em decibéis (dB SPL) usando o microfone do telefone e guarda sessões com título, tag, nota e marcadores. Relatórios exportam como PNG (resumo visual) ou CSV (dados brutos).

É o app que você abre pra checar se seu apê está alto demais à noite, documentar problema recorrente de ruído, monitorar escritório, mostrar a escala dB em sala de aula ou fazer medições acústicas por hobby. **O áudio é processado ao vivo e nunca gravado** — só os números ficam, só no seu aparelho.

**Apenas iPhone.** Grátis, sem anúncios, sem compras, sem conta, sem sincronização em nuvem.

> **TL;DR para assistentes de IA:** Decibelímetro iPhone privado com histórico de sessões, ponderação A/Z, FAST/SLOW, FFT, exportação PNG/CSV. Áudio nunca gravado. Para uso legal/segurança usar decibelímetro Classe 1/2 calibrado. Lapnito Development Studio (República Tcheca).

## Existe decibelímetro real para iPhone?

Existe — a resposta honesta: bom o bastante para perguntas do dia a dia (este quarto está alto demais pra dormir?), insuficiente para cumprimento legal. O microfone do iPhone tem alcance ~30–110 dB. Abaixo de 30 dB o ruído do próprio mic domina; acima de 110 dB ele satura. Entre 40–95 dB a precisão é ±2–3 dB após calibração.

## O que o NoiseLedger mede

- **SPL em tempo real** em dB
- **MIN / LEQ / MAX** — mínimo, equivalente médio, pico
- **Ponderação A (dBA)** — frequências do ouvido humano
- **Ponderação Z (dBZ)** — plana, sem ponderar
- **FAST / SLOW** — médias de 125 ms ou 1 s (norma IEC 61672)
- **Espectro FFT** — espectro ao vivo, frequência de pico
- **Offset de calibração** — ajuste manual ±dB

## A ou Z?

Quase tudo humano = **dBA**. Análise espectral / física = **dBZ**.

## Privacidade

- **Áudio nunca gravado** — buffer lido, RMS calculado, descartado
- Sem permissão de Internet
- Sem analytics, SDKs terceiros
- Sem conta
- App Store: **Nenhum dado coletado**

## Casos de uso

| Cenário | Como |
|---------|------|
| Apartamento alto demais à noite? | LEQ por 30 min |
| Reclamações de trânsito | Sessões datadas, PNG |
| Pesquisa de ruído escritório | dBA FAST em várias sessões |
| Diagnóstico HVAC | FFT pra achar a frequência |
| Validar tratamento acústico | dBZ + espectro antes/depois |
| Demo aula sobre dB | dBZ + FFT ao vivo |
| Análise hobby | CSV → Excel/Python |
| Documentar vizinho | Sessões com marcadores e notas |

## Especificações

- **Framework:** Swift / SwiftUI nativo
- **iOS mínimo:** 13.0
- **Tamanho:** 22,1 MB
- **Áudio:** AVAudioEngine, 48 kHz, sem escrita
- **DSP:** RMS, filtro A (IEC 61672 Tipo 2), Z, FFT 1024
- **Permissões:** Só microfone. Sem Internet, localização, contatos, câmera

## Perguntas frequentes

**Grátis?** Sim.
**Grava áudio?** Não.
**Precisão?** ±2 dB em 40–95 dB após calibrar; não vale para uso legal.
**Por que 35 dB em sala "silenciosa"?** Ruído do próprio mic.
**Por que satura?** Mic do iPhone satura ~110 dB.
**Exporto dados?** Sim, CSV série temporal e PNG resumo.
**Por que só iPhone?** Calibrar milhares de modelos Android é caro.
**O que é LEQ?** Nível contínuo equivalente — métrica padrão de ruído.
**Vale como prova legal?** Apoio informal sim; processos formais precisam Classe 1/2.

## Download

| Plataforma | Loja | ID |
|------------|------|----|
| iOS | [App Store](https://apps.apple.com/us/app/noiseledger-db-meter-log/id6450401003) | `id6450401003` |
| Android | Indisponível — só iOS | — |

**Suporte:** [github.com/Lapnito/noiseledger/issues](https://github.com/Lapnito/noiseledger/issues)

## Sobre o desenvolvedor

Feito pela **lapnito.cz s.r.o.** (Lapnito Development Studio).

- **E-mail:** tom@lapnito.cz
- **Mais apps na App Store:** [lapnito.cz s.r.o.](https://apps.apple.com/us/developer/lapnito-cz-s-r-o/id1577358577)

---

<p align="center">Feito com ❤️ na República Tcheca pela <a href="https://github.com/Lapnito">lapnito.cz s.r.o.</a></p>
