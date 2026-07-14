# STRUCTURE — nail-urban-pink-sample (C안 · 누디핑크 소프트오로라)

단일 파일 정적 사이트 (스탠다드형 · 문의받기). Cloudflare Workers 정적 자산 배포.
**A안(그레이지)=nail-urban-sample와 구조·기능 동일. 색=누디핑크+실버 펄, 히어로에 오로라/글리터/홀로 이펙트 추가(본문 절제).**

```
nail-urban-pink-sample/
├─ index.html        # 핑크 오로라 버전 (A안 복사 → 재색상 + 히어로 이펙트)
├─ nu-hero.jpg       # 히어로 배경
├─ nu-about.jpg      # 소개 섹션
├─ nu-g1~g6.jpg      # 갤러리 6컷 (라이트박스)
├─ wrangler.toml     # CF Workers 배포 설정 (name=nail-urban-pink-sample)
├─ .assetsignore
├─ CHANGELOG.md
└─ STRUCTURE.md
```

## 디자인 토큰
- 팔레트: bg `#FBF7F9` / bg2 `#F4EAF0` / ink 플럼 `#3E2F38` / accent 로즈 `#C486A0` / CTA 플럼로즈 `#8E4E6E` / silver `#C9CDD6` + 이리데센트 `--iri1~5`.
- 이펙트: 히어로 전용 `.hero-aurora`(soft-light) + `.hero-sheen`(screen) + `.hero-glitter`(스파클) + `h1.holo`(홀로그래픽 텍스트) + `.mark-soft`(펄 밴드).
- 타이포·구조·섹션 순서·스크립트는 A안과 동일.

## 톤 3종 (동일 콘텐츠, 색/무드만)
- A안=그레이지(메인/우선): nail-urban-sample.lgt3232.workers.dev
- B안=세이지 그린: nail-urban-green-sample.lgt3232.workers.dev
- C안=누디핑크 오로라(이 레포): nail-urban-pink-sample.lgt3232.workers.dev (CF 연결 후)
