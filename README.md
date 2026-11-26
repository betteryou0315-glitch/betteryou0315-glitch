# 원대한 · Quant Research (Crypto)

**가설을 결과 보기 전에 등록하고, 처음 보는 데이터로 판정합니다. 대부분은 제 손으로 기각했습니다.**

> I pre-register hypotheses and judge them on unseen data. Six studies on Binance perpetual futures (2022–2026, up to 32 coins). Two survived. Direction prediction failed ten times — and I kept the record.

설계·판정 기준·해석은 제가, 코드 구현은 AI(Claude)가 합니다. 핵심 로직(신호, 미래 참조 방지, 판정)은 설계와 맞는지 직접 검토합니다.

---

## 연구 6개 — 판정 결과

| 연구 | 질문 | 판정 | 핵심 숫자 |
|---|---|---|---|
| [**crypto-storm-model**](https://github.com/betteryou0315-glitch/crypto-storm-model) | 레버리지 과열이 "곧 크게 터진다"를 변동성 이상으로 알려주나? | ✅ **모의고사·수능 통과**, 11/15부터 실시간 기록 중 | 특보 순간 실제 폭발 64.8%, 예보 63.7% (변동성만 보면 54.9%) |
| [**crypto-candle-model**](https://github.com/betteryou0315-glitch/crypto-candle-model) | 다음 1시간봉이 장대봉일까? 양봉일까? | ✅ 크기 합격 (공부 때 못 본 코인 12개 포함) / ❌ 방향 불합격 | 크기 AUC 0.729 vs 기준 0.720 / 방향 AUC 0.521 |
| [**crypto-overheat-psychology**](https://github.com/betteryou0315-glitch/crypto-overheat-psychology) | 롱 과열(펀딩비+RSI+OI)은 무엇을 예측하나? | 폭발은 재현, 방향 가설 6개 중 0개 통과 | 처음 보는 코인 4세트·2022 하락장 모두 평소의 1.5배 |
| [**crypto-daily-level-breakout**](https://github.com/betteryou0315-glitch/crypto-daily-level-breakout) | 전일 고저점에서 CVD가 돌파를 가르나? | CVD 기각 / "선의 힘" 재현됐으나 크기 기준 0.4%p 미달 | 비용 후 거래당 −0.10 ~ −0.16% → 수수료를 못 이김 |
| [**crypto-fear-capitulation**](https://github.com/betteryou0315-glitch/crypto-fear-capitulation) | 레버리지까지 털린 급락 = 공포의 끝인가? | ❌ 기각 | 단서 찾기 +10.1%p → 처음 보는 29종목에서 **0.0%p** |
| 펀딩비 캐리 (overheat 연구 02) | 현물 롱 + 선물 숏은 돈이 되나? | 진짜 엣지, 하지만 작음 | 비용 후 자본 대비 연 약 3% |

---

## 검증 방식 — 매 연구에 같은 장치를 씁니다

| 장치 | 막는 것 |
|---|---|
| **사전 등록** — 가설·규칙·합격 기준을 결과 보기 전에 기록, 이후 변경 금지 | 결과 보고 기준 바꾸기 |
| **홀드아웃 / 워크포워드** — 단서 찾기 데이터와 판정 데이터 분리, 판정은 1회 | 과최적화 |
| **엠바고** — 공부·시험 경계에 정답 창만큼 비움, 모든 힌트는 봉 마감 시각까지의 값만 | 미래 데이터 누수 |
| **날 단위 부트스트랩 · 월 단위 군집 t** — 겹치는 사건을 묶어서 신뢰구간 계산 | 부풀려진 t값 |
| **가짜 데이터 코드 점검** — 효과를 심은 데이터에서 통과, 없는 데이터에서 불합격하는지 먼저 확인 | 코드가 효과를 만들어내는 버그 |
| **진짜 상대와 비교** — 찍기가 아니라 "최근 변동성" 같은 뻔한 예상을 이겨야 합격 | 누구나 아는 정보를 새 정보로 착각 |

## 반복해서 확인한 원칙

1. 심리의 극단은 **크게 움직인다**는 건 알려주지만 **어느 쪽인지**는 알려주지 않는다
2. 효과가 있다고 **돈이 되는** 건 아니다 — 비용을 넣으면 대부분 사라진다
3. 처음부터 좋아 보이면 **일단 의심**한다

---

## 그 밖에

- **TradingView 지지/저항 지표** (무료 오픈소스) — 스윙 고저점 + 터치 횟수, ATR 기준 레벨 묶기 · [TradingView 스크립트](https://kr.tradingview.com/u/Han0315/#published-scripts)
- **전략 검증 리포트** — 공개된 매매 전략을 수수료·슬리피지 반영해 독립 검증해 드립니다
- 연락: betteryou0315@gmail.com

<sub>개인 연구 기록이며 투자 조언이 아닙니다.</sub>
