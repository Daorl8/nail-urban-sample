# STRUCTURE — nail-urban-sample

단일 파일 정적 사이트 (스탠다드형 · 문의받기). Cloudflare Workers 정적 자산 배포.

```
nail-urban-sample/
├─ index.html        # 배포 후보 = 그레이지/오트밀 브랜드톤 (인라인 CSS/JS 단일 파일)
├─ index_green.html  # 변형 = 차분한 세이지 그린 (최신 index.html 복사 후 재색상, 미리보기 위해 현재 /index_green.html로 배포)
├─ nu-hero.jpg       # 히어로 배경 (레이스·펄 젤네일)
├─ nu-about.jpg      # 소개 섹션 (핑크 보우 시그니처)
├─ nu-g1~g6.jpg      # 갤러리 6컷 (라이트박스)
├─ wrangler.toml     # CF Workers 배포 설정 (name=nail-urban-sample)
├─ .assetsignore     # 배포 제외 (.git 노출 방지 등)
├─ CHANGELOG.md      # 변경 이력
└─ STRUCTURE.md      # 이 파일
```

## 섹션 순서
헤더(스티키) → 히어로 → 소개(About) → 시술 안내(Menu 4카드) → 갤러리(Gallery 6·라이트박스) → 예약·문의(Reserve: 채널 3 + 폼) → 오시는 길(Location) → 푸터 + 모바일 퀵바.

## 디자인 토큰
- 팔레트: 펄 화이트 `#FAF8FA` + 로즈쿼츠 `#C99DAE` / `#A56E85` + 딥 플럼 잉크 `#322B31`. 실버-로즈 이리데센트 샤인(절제).
- 타이포: 디스플레이 Cormorant Garamond + 국문 Nanum Myeongjo(명조) / 본문 Pretendard. 폴백=안전 산세리프.
- 무드: 청순·여리여리·우아·고급 (사장님 인스타 톤 기반).

## 배포
- 레포: github.com/Daorl8/nail-urban-sample → Cloudflare 연결 → nail-urban-sample.lgt3232.workers.dev
- 폼=데모(전송 없음). 실제 정보(가격·주소·영업시간·예약 링크)는 플레이스홀더 → 원장님 확인 후 교체.
