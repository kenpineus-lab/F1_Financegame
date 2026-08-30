# Pit Wall GP

**F1 팀을 운영하며 경제를 배우는 게임 · An F1 team-principal game that teaches economics**

▶ **[지금 플레이 / Play now](https://kenpineus-lab.github.io/F1_Financegame/)**

한국어와 영어를 함께 지원합니다. 화면 왼쪽 위에서 `한+EN` / `한국어` / `English` 를 고를 수 있습니다.
Bilingual Korean/English — switch at the top left.

---

## 무엇을 하는 게임인가 · What is it

F1 팀의 **팀 대표(Team Principal)** 가 되어 10라운드 시즌을 운영합니다. 차를 직접 몰지는 않습니다.
**돈을 어디에 쓸지** 정합니다 — 그게 이 스포츠에서 실제로 순위를 만드는 일입니다.

You are the **Team Principal** of an F1 team for a 10-round season. You don't drive.
You decide **where the money goes** — which is what actually creates results in this sport.

시즌 목표는 세 가지를 **동시에** 달성하는 것입니다. 이 셋은 서로를 잡아먹습니다.
The season is won by hitting three things **at once**. They fight each other.

| | 조건 · Condition |
|---|---|
| 1 | 팀별 목표 순위 안에 들기 · Finish inside your team's target position |
| 2 | 파산하지 않기 (최종 순자산 0 이상) · Don't go bankrupt |
| 3 | FIA 비용 상한 $135M 지키기 · Stay under the cost cap |

---

## 팀 선택 = 난이도 · Team choice is the difficulty

| 팀 | 난이도 | 목표 | 고정비/라운드 | 배우는 것 |
|---|---|---|---|---|
| **HALCYON** | 하 · Easy | P6 | $3.2M | 투자하면 순위가 오른다 |
| **MERIDIAN** | 중 · Medium | P4 | $10.1M | 대출이 도움이 된다 |
| **APEX BULLS** | 상 · Hard | P1 | $21.5M | 대출은 죽는다, 현금이 이긴다 |

같은 "풀레버리지" 전략이 MERIDIAN에서는 승률 89%, APEX에서는 9%(파산 91%)입니다.
고정비 기반이 다르기 때문입니다.

The same all-in leverage strategy wins 89% of the time with MERIDIAN and 9% with APEX
(bankrupt 91%) — because their fixed-cost bases are different.

---

## 주말 진행 · The race weekend

1. **팀 운영 (패독)** — 개발·마케팅·스폰서 계약·전략·자금 조달·드라이버 결정
2. **금요일 연습** — 드라이버 컨디션이 드러남 (매주 다름, 페이스에 직접 반영)
3. **토요일 퀄리파잉** — 결승 그리드 결정
4. **일요일 결승** — 서킷별 실제 랩 수만큼 **랩 바이 랩 중계**
   (타이밍 타워 20대 + 추월·피트인·세이프티카·리타이어 실황, 속도 조절 가능)

드라이버는 2명이고 **둘 다 실제 F1 배점**(25-18-15-12-10-8-6-4-2-1, 패스티스트랩 +1)으로 득점합니다.

---

## 경제 모델 · The economic model

**수익 3종** — 상금(순위별, 차 1대당) / 스폰서(계약 형태 × 브랜드 배수) / 머천다이즈·중계권(브랜드에만 비례)

**비용 4종** — 어디에 쓰이는지 항목별로 표시됩니다
- 고정비 · 기본 운영: 팩토리 임대료, 엔지니어·미캐닉 급여, 물류·운송
- 고정비 · 드라이버 연봉: 성적과 무관하게 나감
- 변동비 · 타이어와 부품: 전략에 따라 변동
- 변동비 · 사고 수리와 연습 셋업: 사건이 있을 때만

**자금 조달 2종** — 대출(이자 4%/라운드, 성적 무관) vs 지분 매각(상금 25% 영구 양도, 성공할수록 비쌈)

매 라운드 손익과 시즌 **손익계산서**(매출 → 영업비용 → 영업이익 → 이자 → 순이익)가 나옵니다.
숫자는 자본 변화와 정확히 일치합니다.

---

## 배우는 경제 개념 11가지 · Eleven concepts

희소성 · 기회비용 · 한계수확체감 · 고정비와 변동비 · 기대값 · 리스크와 수익의 교환 ·
투자수익률 · 부채와 지분 조달 · 브랜드 자산과 회수기간 · 경쟁과 상대성과 · 인적자본 투자

개념은 설명으로 먼저 나오지 않습니다. **돈을 잃거나 벌었을 때 그 자리에서** 이름이 붙습니다.
전체 설명은 게임 안 **설명서** 버튼에 한국어·영어로 정리돼 있습니다.

Concepts are named **the moment they cost or earn you money**.
All of them are written out up front in the in-game **Manual**.

---

## 밸런스 · Balance

시뮬레이션 2,500회 × 팀별로 검증했습니다. 라이벌 9팀도 매 라운드 개발하며,
**상위 팀일수록 더 빨리** 개발합니다(실제 F1처럼). 가만히 있으면 어느 팀이든 승률 0~1%입니다.

Verified with 2,500 simulated seasons per team. All nine rival teams develop every round,
and **stronger teams develop faster** — as in real F1. Doing nothing wins 0–1% of the time.

---

## 기술 · Technical

의존성 없는 단일 HTML 파일입니다. 빌드 도구도 서버도 필요 없습니다.
진행 상황은 브라우저 `localStorage`에 저장되므로 창을 닫아도 이어서 할 수 있습니다.

A single dependency-free HTML file — no build step, no server.
Progress is saved to `localStorage`, so you can close the tab and continue later.

로컬에서 열려면 `index.html`을 브라우저로 열기만 하면 됩니다.

---

이 게임은 실존 F1 팀·드라이버를 사용하지 않습니다. 팀과 드라이버는 모두 가상입니다.
This game uses no real F1 teams or drivers. All teams and drivers are fictional.
