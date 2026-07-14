# STRUCTURE — nail-urban-pink-sample (C안 · 클린 뉴트럴 + 쿨로즈)

단일 파일 정적 사이트 (스탠다드형 · 문의받기). Cloudflare Workers 정적 자산 배포.
**A안(nail-urban-sample)과 콘텐츠·구조 동일. 색 = 쿨 뉴트럴 + 쿨로즈 포인트, 레이아웃 = 각진(플랫) + 모자이크 갤러리.**
※ 레포명이 "pink"지만 오로라/글리터 이펙트는 없음(폐기됨). 이름은 히스토리상 유지.

```
nail-urban-pink-sample/
├─ index.html        # 확정본 (쿨 뉴트럴 + 쿨로즈, 각진 레이아웃, 모자이크 갤러리)
├─ nu-hero.jpg / nu-about.jpg / nu-g1~g6.jpg   # self-host 이미지 8종
├─ wrangler.toml     # CF Workers 배포 설정 (name=nail-urban-pink-sample)
├─ .assetsignore     # 배포 제외 (.git·문서·index_*.html 백업)
├─ CHANGELOG.md / STRUCTURE.md
└─ index_*.html      # 롤백/대안 스냅샷 (배포 제외)
```

## 디자인 토큰 (실제 코드 기준)
- 베이스: bg `#F8F8FA` / bg2 `#EEEDF1` / card `#FFFFFF` / taupe `#ABA9B2` (쿨 뉴트럴)
- 텍스트: ink `#2F2E33` / ink-soft `#6B6873`(AA 통과) / ink-faint `#8A8794`
- 포인트: gold(=로즈 액센트) `#DB5E88` / gold-mark `#F5C6D7` / CTA `#C1467A`(흰텍 ~4.7:1) / cta-dk `#A73A67`
- 라인: line `#E6E4EA` / line-soft `#F1EFF4`
- ⚠️ 변수명 `--gold`는 3톤 공통 find-replace 편의로 유지(실제 색은 로즈)

## 레이아웃 규칙 (아뜰리에 실측 기반)
- **border-radius 전부 0** (버튼·카드·사진·지도·입력창)
- **box-shadow 0 · 호버 들림(translateY) 없음** = 플랫
- 사진: about 1:1 정사각 / 갤러리 = 모자이크
- **모자이크 갤러리**: 데스크톱 4열×3행(aspect 4/3) — 큰 정사각(2×2) 1 + 가로형(2×1) 3 + 작은 정사각(1×1) 2 = 12셀 정확히 채움(빈틈 0). 모바일 2열×5행.
- 시그니처 카드: 흰 배경 + 로즈 테두리 + 배지 (그라데이션 없음)

## 스크립트
등장 리빌(IntersectionObserver + 1.5s 강제표시 폴백) · 라이트박스(role=dialog/aria-modal, alt 승계) · 폼(데모 가짜성공, 검증+focus, role=alert, 중복제출 가드)

## 배포 / 3톤
- 레포 github.com/Daorl8/nail-urban-pink-sample → CF → nail-urban-pink-sample.lgt3232.workers.dev
- A안=그레이지 nail-urban-sample / B안=세이지그린 nail-urban-green-sample / **C안=이 레포(확정)**
