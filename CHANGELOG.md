# CHANGELOG — nail-urban-pink-sample (네일어반 누디핑크·소프트오로라 · C안)

## 2026-07-14 — 소프트 오로라 펄 변형 생성 (독립 레포)
- A안(그레이지) index.html 복사 → **누디핑크+실버 파스텔 펄**로 재색상 + **히어로 몰입 이펙트**(본문 절제).
- 팔레트: bg #FBF7F9 / bg2 #F4EAF0 / ink 플럼 #3E2F38 / accent 로즈 #C486A0 / CTA 플럼로즈 #8E4E6E(흰텍 ~6:1 통과) / silver #C9CDD6 + 이리데센트 5색(--iri1~5).
- 히어로 이펙트(§2 "의도된 효과 예외"로 히어로에만 가둠):
  - `.hero-aurora` = 파스텔 이리데센트 그라데(soft-light 블렌드, 24s 슬로우 시프트) — 사진 위 은은한 오로라 시트.
  - `.hero-sheen` = 우상단 화이트 하이라이트(screen 블렌드) 펄광.
  - `.hero-glitter` = 미세 스파클(1.2~1.7px 라디얼 도트 9개, 5s 트윙클).
  - `h1.holo` = 홀로그래픽 그라데 텍스트(로즈→바이올렛→틸→모브, 대비 위해 딥톤 스톱; 9s 스윕). 국문 서브라인은 솔리드 ink 유지.
  - `.mark-soft` = 핑크→라일락→민트 펄 밴드.
- 본문(About/Menu/Gallery/Reserve/Location)은 이펙트 없이 핑크 뉴트럴+대비 확보. 구조·지도(구글Embed)·길찾기·폼·§11/§12 방어는 A안 상속.
- reduced-motion=장식 모션 유지(프로젝트 §12 결정). CF 연결은 사용자.
