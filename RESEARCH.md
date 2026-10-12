# FOURTH ME V12 · 연구 근거와 제품 설계 판단

검토 기준: 2026-10-12. 사용자가 제공한 유튜브 영상 요약과 학술·연구기관·UX 원문을 대조했습니다. **제공 영상 전체를 독립적으로 시청·전사 검증했다고 주장하지 않습니다.** 11:00~11:53, 17:48~21:42의 내용은 사용자 제공 요약을 근거로 사용했습니다.

## 1. 사용자 목적의 재정의

이 앱의 목표는 21일 습관 완주가 아니라 **평생에 걸쳐 삶의 방향, 원칙, 감정, 행동, 관계, 건강, 성과 및 정체성 변화를 기록하고 나중에 시간의 흐름으로 되돌아보는 것**입니다. ‘4차원의 나’는 미래를 예언한다는 뜻이 아니라, **과거·현재·가능한 미래를 연결해 관찰하는 시간적 관점**으로 정의했습니다.

## 2. 근거별 설계 결정

| 연구·근거 | 신뢰할 수 있는 핵심 내용 | V12 실제 적용 | 주의할 해석 |
|---|---|---|---|
| McAdams & McLean (2013), *Narrative Identity* | 서사적 정체성은 재구성된 과거와 상상한 미래를 통합하는 변화하는 삶의 이야기 | '나의 인생 영화'의 이야기·메시지·버전 이력과 시간별 전환점 | 앱이 사용자의 정체성 성장 자체를 자동 측정한다고 주장하지 않음 |
| Harkin et al. (2016), *Psychological Bulletin*, 138개 연구/19,951명 | 진행 상황 기록 개입은 목표 달성 개선과 관련(d≈0.40) | 완료 행동, 기록일, 월별 변화의 자동 집계 | 행동 건수가 곧 삶의 가치나 건강 개선을 뜻하지 않음 |
| Gollwitzer & Sheeran (2006), 94개 독립 검증 | '상황이 오면 행동한다'는 실행 의도는 목표 달성에 도움(d≈0.65) | 아침 루틴의 선택적 장애물·대응 계획, 오늘의 작은 행동 | 실행 의도는 만능 처방이 아니며 개인차가 있음 |
| Kappes & Oettingen (2011), *JESP* | 긍정적 미래 상상만 하는 것은 행동 에너지를 낮출 수 있음 | 감정 상상 다음에 오늘의 행동·장애물 선택 | '이미 이룬 감정'만으로 현실이 바뀐다는 주장을 채택하지 않음 |
| Ryan & Deci (2000), 자기결정성이론 | 자율성·유능감·관계성은 동기와 안녕감에 중요한 요인 | 감정 강요·강제 분류·실패 낙인 제거, 자유 입력 | 심리치료·정신건강 효과를 입증한 앱이 아님 |
| BJ Fogg, Behavior Model | 행동은 동기·실행 용이성·계기의 결합으로 설명됨 | 2분 시작, 적은 입력량, 한 번에 한 행동 | '2분'은 실용적 설계 선택이며 본 앱의 최적 길이로 검증된 값은 아님 |
| NN/g, Recognition over Recall (2024) | 사용자가 정보를 매번 떠올리기보다 보이는 맥락에서 인식하게 하는 편이 쉬움 | 아침에 저장된 영화 자동 표시, 탭 4개로 통합, 상세 기능 접기 | UX 휴리스틱이지 앱의 효과에 대한 임상 검증은 아님 |
| Stanford Life Design Lab, Odyssey Planning 자료·영상 | 인생 방향은 하나의 정답보다 가능한 삶을 탐색하고 시험하는 과정 | 영화의 방향 수정 시 이전 버전 보존, 전환점을 실패로 취급하지 않음 | 진로 설계 프레임워크이며 모든 삶의 결과를 보장하지 않음 |

## 3. 사용자 제공 영상의 개념과 과학적 구분

- **명확한 의도:** 삶의 영화·메시지를 저장하는 기능으로 구현. 이는 선택의 기준이지 미래를 예측하는 기능이 아닙니다.
- **충만한 감정:** 경험하고 싶은 감정과 음악·환경을 기록하되, 실제 기분과 다를 수 있음을 허용합니다. 긍정적 감정 강요는 제외했습니다.
- **행동:** 즉시 입력·실행할 수 있는 행동과 2분 타이머를 구현. 영상의 '끌어당김'을 과학적 인과법칙으로 주장하지 않습니다.
- **시간:** 의도·감정·행동·사건을 날짜별로 나란히 표시하고, 선택적 월간 회고로 스스로 의미를 해석하도록 설계했습니다.
- **아침·밤 5~10분:** 시간과 횟수는 사용자의 선호에 맞춘 권장 루틴입니다. 반드시 매일 지켜야 하거나 모든 사람에게 최적이라는 근거는 없습니다.

## 4. 기존 버전에서 삭제·유지·변경한 것

- 대시보드와 실행 중복: **삭제** → '오늘'로 통합.
- 건강·경제·성장·관계 강제 분류: **기본 흐름에서 제외** → 자유 입력 우선, 과거 분류는 원본 화면에 보존.
- 마인드맵의 6개 노드 편집: **기본 화면에서 제외** → 의도·감정·행동·시간 연결 지도 자동 표시. 원본 편집은 `legacy.html`로 보존.
- '완료 횟수 = 성장' 해석: **배제** → 행동 기록과 월간 자기관찰을 분리.
- 하루의 성찰: **선택적·짧은 루틴**으로 재설계.
- V11 삶의 흐름 별도 백업: **V12 통합 백업**에 포함.

## 5. 읽고 검토한 원문 및 영상 안내

1. McAdams, D. P., & McLean, K. C. (2013). Narrative Identity. Association for Psychological Science. https://www.psychologicalscience.org/journals/current-directions/0963721413475622/
2. Harkin, B., et al. (2016). Does monitoring goal progress promote goal attainment? *Psychological Bulletin*. https://pubmed.ncbi.nlm.nih.gov/26479070/
3. Gollwitzer, P. M., & Sheeran, P. (2006). Implementation Intentions and Goal Achievement. https://doi.org/10.1016/S0065-2601(06)38002-1
4. Kappes, H. B., & Oettingen, G. (2011). Positive fantasies about idealized futures sap energy. https://doi.org/10.1016/j.jesp.2011.02.003
5. Ryan, R. M., & Deci, E. L. (2000). Self-determination theory and the facilitation of intrinsic motivation. https://pubmed.ncbi.nlm.nih.gov/11392867/
6. Stanford Behavior Design Lab. Fogg Behavior Model. https://behaviordesign.stanford.edu/resources/fogg-behavior-model
7. Nielsen Norman Group. Memory Recognition and Recall in User Interfaces (2024). https://www.nngroup.com/articles/recognition-and-recall/
8. Nielsen Norman Group. Recognition vs. Recall (영상 자료). https://www.nngroup.com/videos/recognition-vs-recall/
9. Stanford Life Design Lab. Resources / Odyssey Planning Videos. https://lifedesignlab.stanford.edu/resources
10. WOOP (Wish–Outcome–Obstacle–Plan), 공식 설명. https://woopmylife.org/
11. 사용자 제공 유튜브 영상(제공된 요약만 사용): https://youtu.be/1B5_xG7jmY8

## 6. 검증되지 않은 부분

- FOURTH ME V12 자체의 임상적 효과, 정체성 변화 효과, 습관 형성 효과는 별도로 검증하지 않았습니다.
- 장기 성장의 인과관계, '점들의 연결'의 필연성, 외부 현실의 끌어당김 효과는 과학적으로 확정된 사실로 취급하지 않습니다.
- 연도별 완료 행동 그래프는 **기록된 행동 수**만 나타냅니다. 사용자가 기록하지 않은 실천과 삶의 질 변화는 포착하지 못합니다.
