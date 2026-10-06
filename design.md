---
version: alpha
name: JYP-Entertainment-design-analysis
description: |
  아티스트 이미지가 화면의 유일한 "색"이 되는 모노크롬 갤러리 시스템. jype.com은 흰 캔버스(#ffffff)와 거의 검정(#101010)만으로 크롬을 구성하고, 채도는 오직 앨범 아트·아티스트 사진에서만 나온다. 홈은 화면 중앙을 세로로 관통하는 1px 헤어라인 위에 정사각 앨범 커버 하나를 세우는 "릴리즈 스포트라이트" 슬라이더이고, 아티스트 페이지는 3열 메이슨리 그리드(15px 거터)로 사진을 각진 모서리 그대로 타일링한다. 타이포는 넓게 퍼진 그로테스크 aktiv-grotesk-extended(한글 pretendardJP 폴백)를 대문자 영문 위주로 쓰며, 위계는 색이 아니라 굵기(400→700→800)와 크기로 만든다. 라운드·그림자·그라데이션 없음 — 모서리는 0px, 유일한 원형은 페이지네이션 활성 점뿐. 전체 메뉴는 화면을 덮는 거의 검정(#0f0e0e) 오버레이로 열린다.

colors:
  ink: "#101010"
  ink-pure: "#000000"
  heading: "#21252c"
  sub: "#42474e"
  meta: "#646b76"
  mute: "#868e9b"
  mute-faint: "rgba(134,142,155,0.34)"
  rule-vertical: "#707070"
  hairline: "#000000"
  divider: "#868e9b"
  canvas: "#ffffff"
  surface-card: "#f4f6f8"
  surface-image: "#000000"
  surface-dark: "#0f0e0e"
  on-dark: "#ffffff"
  on-dark-mute: "rgba(255,255,255,0.77)"
  on-dark-faint: "rgba(160,160,160,0.77)"
  pagination-active: "#42474e"
  on-pagination-active: "#ffffff"

typography:
  display-xl:
    fontFamily: aktiv-grotesk-extended
    fontSize: 28px
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: 0
  page-title:
    fontFamily: aktiv-grotesk-extended
    fontSize: 30px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0
  display-artist:
    fontFamily: aktiv-grotesk-extended
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: 0
  menu-category:
    fontFamily: aktiv-grotesk-extended
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0
  heading-md:
    fontFamily: aktiv-grotesk-extended
    fontSize: 18px
    fontWeight: 700
    lineHeight: 2
    letterSpacing: 0
  label-name:
    fontFamily: aktiv-grotesk-extended
    fontSize: 16px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0
  body-md:
    fontFamily: aktiv-grotesk-extended
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0
  body-strong:
    fontFamily: aktiv-grotesk-extended
    fontSize: 14px
    fontWeight: 600
    lineHeight: 1.6
    letterSpacing: 0
  tab-md:
    fontFamily: aktiv-grotesk-extended
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.5
    letterSpacing: 0
  tab-active:
    fontFamily: aktiv-grotesk-extended
    fontSize: 14px
    fontWeight: 700
    lineHeight: 1.5
    letterSpacing: 0
  caption-md:
    fontFamily: aktiv-grotesk-extended
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0
  caption-tight:
    fontFamily: aktiv-grotesk-extended
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: 0
  overline:
    fontFamily: aktiv-grotesk-extended
    fontSize: 10px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0

rounded:
  none: 0px
  full: 50%

spacing:
  xxs: 4px
  xs: 6px
  sm: 10px
  md: 15px
  lg: 24px
  xl: 38px
  xxl: 62px
  section: 100px

components:
  primary-nav:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 24px 62px
    height: 84px
  nav-sns-icon:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    size: 30px
  lang-select:
    backgroundColor: "transparent"
    textColor: "{colors.ink-pure}"
    typography: "{typography.tab-md}"
    rounded: "{rounded.none}"
    padding: 0px 24px 0px 0px
  menu-trigger:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: 10px
    size: 45px
  menu-overlay:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    typography: "{typography.menu-category}"
    rounded: "{rounded.none}"
  menu-link:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark-mute}"
    typography: "{typography.body-md}"
    padding: 6px 0px
  menu-link-sub:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark-faint}"
    typography: "{typography.body-md}"
    padding: 3px 0px 3px 10px
  release-spotlight:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-xl}"
    rounded: "{rounded.none}"
  release-cover:
    backgroundColor: "{colors.surface-image}"
    rounded: "{rounded.none}"
    size: 270px
  icon-button-square:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    size: 26px
  page-header:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.heading}"
    typography: "{typography.page-title}"
    rounded: "{rounded.none}"
  sub-tab:
    backgroundColor: "transparent"
    textColor: "{colors.sub}"
    typography: "{typography.tab-md}"
    padding: 0px 15px
  sub-tab-active:
    backgroundColor: "transparent"
    textColor: "{colors.heading}"
    typography: "{typography.tab-active}"
  artist-card:
    backgroundColor: "{colors.surface-image}"
    textColor: "{colors.on-dark}"
    typography: "{typography.label-name}"
    rounded: "{rounded.none}"
    padding: 0px
  artist-sns-icon:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.none}"
    size: 36px
  notice-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.heading}"
    typography: "{typography.heading-md}"
    rounded: "{rounded.none}"
    padding: 35px 38px
  pagination-item:
    backgroundColor: "transparent"
    textColor: "{colors.sub}"
    typography: "{typography.body-md}"
    rounded: "{rounded.none}"
    padding: 7px
    size: 34px
  pagination-item-active:
    backgroundColor: "{colors.pagination-active}"
    textColor: "{colors.on-pagination-active}"
    typography: "{typography.body-md}"
    rounded: "{rounded.full}"
    size: 34px
  footer-section:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.mute}"
    typography: "{typography.caption-md}"
    rounded: "{rounded.none}"
    padding: 0px 62px 68px
---

## Overview

JYP 웹사이트의 원칙은 하나다: **크롬은 흑백, 색은 아티스트가 가져온다.** 인터페이스는 흰 캔버스(`{colors.canvas}`)와 거의 검정 잉크(`{colors.ink}` — `#101010`) 두 값으로 거의 전부 만들어지고, 화면에 나타나는 모든 채도(노랑·빨강·파스텔)는 앨범 커버와 아티스트 사진에서만 온다. 브랜드 액센트 컬러가 없다 — Pinterest가 빨강 CTA 하나로 시스템을 묶는다면, JYP는 "색이 없다는 것" 자체로 묶는다. 회사 사이트가 소속 아티스트들의 서로 다른 컨셉 컬러를 모두 품어야 하기 때문에 생긴 구조다.

시스템은 세 가지 표면 모드로 나뉜다.

- **릴리즈 스포트라이트(홈 `/ko`)** — 화면 중앙을 위아래로 관통하는 1px 세로선(`{colors.rule-vertical}`) 위에 아티스트명·곡명(`{typography.display-xl}`), 270px 정사각 커버, 발매일, 한 줄 설명, 세로로 쌓인 정사각 아이콘 버튼 3개(+ / ▶ / △)가 일렬로 꿰어진다. 좌우 가로 슬라이더로 최신 릴리즈를 넘긴다.
- **갤러리 그리드(`/ko/Artist`)** — 3열 메이슨리, 15px 거터, 모서리 0px. 각 카드는 검정 배경 위 사진(opacity 0.92)이며 하단에 흰 아티스트명과 SNS 아이콘 행이 겹쳐 올라간다.
- **정보 보드(`/ko/board/notice` 등)** — 연회색(`{colors.surface-card}` — `#f4f6f8`) 정사각에 가까운 카드 2열, 제목은 카드 가운데, 날짜·조회수는 하단 디바이더 위.

모든 페이지 상단에는 84px 흰 헤더(좌: JYP 로고, 우: SNS 아이콘 4개 + 언어 선택 + 햄버거)가 있고, 햄버거를 누르면 화면 전체를 덮는 거의 검정(`{colors.surface-dark}` — `#0f0e0e`) 메뉴 오버레이가 열린다. 즉 **밝은 페이지 ↔ 어두운 메뉴**의 반전이 시스템의 유일한 대비 장치다.

**Key Characteristics:**
- 무채색 크롬: 액센트 컬러 없음. 색은 이미지 전용
- aktiv-grotesk-extended(넓은 그로테스크) 단일 서체, 영문 대문자 라벨 중심, 한글은 pretendardJP 폴백
- 0px 라운드 고정 — 카드·이미지·버튼 모두 각진 모서리. 유일한 원형은 페이지네이션 활성 표시
- 그림자·그라데이션 없음. 깊이는 사진과 흑백 반전에서만
- 홈 중앙 1px 세로 헤어라인이 레이아웃의 척추
- 메이슨리 사진 그리드(3열 → 1열), 거터 15px(모바일 5px)
- 서브 내비는 텍스트 탭 + 활성 1px 밑줄

## Colors

> **Source pages:** `/ko`(홈), `/ko/Artist`(아티스트), `/ko/board/notice`(공지), 전체 메뉴 오버레이. 2026-10-06 computed style 기준.

### Brand & Accent
- **없음.** JYP 크롬에는 브랜드 컬러 토큰이 없다. 강조는 굵기·크기·밑줄·흑백 반전(`{component.pagination-item-active}`, `{component.menu-overlay}`)으로만 한다. 소속 아티스트의 컨셉 컬러는 각 아티스트 서브사이트(예: `nexz.jype.com`)의 영역이다.

### Surface
- **Canvas** (`{colors.canvas}` — `#ffffff`): 모든 페이지 바탕, 헤더, 푸터.
- **Surface Card** (`{colors.surface-card}` — `#f4f6f8`): 공지 카드 배경. 아주 옅은 블루그레이 — 시스템에서 유일한 "회색 면".
- **Surface Image** (`{colors.surface-image}` — `#000000`): 아티스트 카드의 사진 뒤 바탕. 이미지를 opacity 0.92로 깔아 살짝 어둡게 만든다.
- **Surface Dark** (`{colors.surface-dark}` — `#0f0e0e`): 전체 메뉴 오버레이. 순수 검정이 아닌 미세하게 따뜻한 검정.

### Text
- **Ink** (`{colors.ink}` — `#101010`): 기본 본문·헤더·아이콘. 사용 빈도 압도적 1위.
- **Ink Pure** (`{colors.ink-pure}` — `#000000`): 언어 선택(KO), 햄버거 바 등 일부 UI.
- **Heading** (`{colors.heading}` — `#21252c`): 페이지 타이틀(ARTIST, JYP), 활성 탭, 공지 제목. 잉크보다 아주 살짝 푸른 차콜.
- **Sub** (`{colors.sub}` — `#42474e`): 비활성 서브탭, 페이지네이션 숫자.
- **Meta** (`{colors.meta}` — `#646b76`): 홈의 "Release Date"·발매일.
- **Mute** (`{colors.mute}` — `#868e9b`): 공지 날짜·조회수, 푸터 링크·카피라이트.
- **Mute Faint** (`{colors.mute-faint}` — `rgba(134,142,155,0.34)`): 공지 카드 상단 "NOTICE" 오버라인.

### On Dark (메뉴 오버레이)
- **On Dark** (`{colors.on-dark}` — `#ffffff`): 1차 카테고리(JYP, ARTIST, SUSTAINABILITY, IR, AUDITION, RECRUIT), 아티스트 카드 위 이름.
- **On Dark Mute** (`{colors.on-dark-mute}` — `rgba(255,255,255,0.77)`): 2차 메뉴 링크.
- **On Dark Faint** (`{colors.on-dark-faint}` — `rgba(160,160,160,0.77)`): 3차(들여쓴) 메뉴 링크.

### Lines
- **Rule Vertical** (`{colors.rule-vertical}` — `#707070`): 홈 중앙 세로선.
- **Hairline** (`{colors.hairline}` — `#000000`): 정사각 아이콘 버튼 1px 테두리, 활성 탭 밑줄.
- **Divider** (`{colors.divider}` — `#868e9b`): 공지 카드 하단 날짜 구분선.

### Semantic
- 에러·성공·포커스 색은 캡처한 공개 페이지에서 확인되지 않음(Known Gaps 참조).

## Typography

### Font Family
**aktiv-grotesk-extended** (Dalton Maag, Adobe Fonts 배포)가 모든 텍스트 역할의 1순위다. 가로로 넓게 벌어진 확장형 그로테스크라서 "ARTIST", "ESG STRATEGY" 같은 대문자 라벨이 자간 조정 없이도 넓고 단단하게 읽힌다. 웨이트 400/500/600/700(+ 홈 곡명에 800)을 쓴다. 폴백 스택: `aktiv-grotesk-extended` → `pretendardJP`(한글·일문) → `Noto Sans SC`(중문) → `sans-serif`. 같은 패밀리의 `aktiv-grotesk`, `aktiv-grotesk-condensed`도 로드되지만 메인 페이지에서는 extended가 지배적이다.

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.page-title}` | 30px | 700 | 1.5 (45px) | 0 | 서브페이지 타이틀("ARTIST", "JYP" 28px) |
| `{typography.display-xl}` | 28px | 800 | 1.1 | 0 | 홈 릴리즈 곡명("SAUCIN'") |
| `{typography.display-artist}` | 24px | 700 | 1.25 (30px) | 0 | 홈 아티스트명("NEXZ") |
| `{typography.menu-category}` | 22px | 700 | 1.5 (33px) | 0 | 전체 메뉴 1차 카테고리 |
| `{typography.heading-md}` | 18px | 700 | 2 (36px) | 0 | 공지 카드 제목 |
| `{typography.label-name}` | 16px | 700 | 1.5 | 0 | 아티스트 카드 이름 |
| `{typography.body-md}` | 14px | 400 | 1.5 (21px) | 0 | 기본 본문, 메뉴 링크 (body 기본값) |
| `{typography.body-strong}` | 14px | 600 | 1.6 | 0 | 홈 릴리즈 설명 문장 |
| `{typography.tab-md}` | 14px | 500 | 1.5 | 0 | 비활성 서브탭, 언어 선택 |
| `{typography.tab-active}` | 14px | 700 | 1.5 | 0 | 활성 서브탭(+1px 밑줄) |
| `{typography.caption-md}` | 12px | 400 | 1.5 | 0 | 날짜, 조회수, 푸터 |
| `{typography.caption-tight}` | 12px | 400 | 1.1 | 0 | 홈 "Release Date" 라벨 |
| `{typography.overline}` | 10px | 400 | 1.5 | 0 | 공지 카드 "NOTICE" 타입 표시 |

### Principles
- 최대 크기가 30px로 낮다. 헤드라인을 키우는 대신 이미지를 크게 쓰고, 텍스트는 이미지의 캡션처럼 작게 둔다.
- 위계는 색보다 **굵기**로 만든다: 같은 14px 안에서 400(본문) → 500(탭) → 600(설명) → 700(활성 탭).
- 메뉴·탭·라벨은 영문 대문자. 한글은 본문·공지 제목 같은 콘텐츠 영역에만.
- 자간은 전부 `normal`. extended 서체 자체가 넓으므로 추가 트래킹을 주지 않는다.

### Note on Font Substitutes
aktiv-grotesk-extended는 Adobe Fonts 라이선스 서체다. 오픈소스 대체는 **Archivo Expanded**(또는 Archivo의 wdth 125) 1순위, **Unbounded**는 디스플레이 전용 2순위. 한글은 **Pretendard**(원본과 같은 계열)를 그대로 쓰면 된다.

## Layout

### Spacing System
- **Base unit:** 뚜렷한 4/8 그리드가 아니라 5의 배수 경향(5 · 10 · 15 · 35 · 100)과 고정 거터(24 · 38 · 62)가 섞여 있다.
- **Tokens (front matter):** `{spacing.xxs}`(4px) · `{spacing.xs}`(6px) · `{spacing.sm}`(10px) · `{spacing.md}`(15px) · `{spacing.lg}`(24px) · `{spacing.xl}`(38px) · `{spacing.xxl}`(62px) · `{spacing.section}`(100px).
- **헤더:** 상하 24px, 좌우 62px, 높이 84px.
- **콘텐츠 래퍼:** 상단 100px(헤더 아래 여백), 하단 72px.
- **서브탭:** 좌우 15px 패딩, 탭 간 시각 간격 약 36px. 타이틀과 탭 사이 10px.
- **그리드 거터:** 15px(데스크톱), 5px(모바일).
- **메뉴 링크:** 상하 6px, 3차 링크 상하 3px + 왼쪽 들여쓰기 10px.

### Grid & Container
- **헤더 폭:** 풀폭, 좌우 62px 거터.
- **아티스트 그리드:** 3열 메이슨리(각 열 ≈ 321px + 15px 거터). 이미지 원래 비율 유지(세로형·가로형 혼재). 모바일 1열 풀블리드.
- **공지 그리드:** 2열, 카드 520×522px(거의 정사각), 카드 사이 1px 흰 경계.
- **홈 스포트라이트:** 단일 중앙 열(커버 270px), 세로선이 열의 축. 가로 슬라이드 트랙 위에 1440px 단위 페이지가 이어진다.
- **푸터:** 한 줄 — 좌측 정책 링크들(개인정보처리방침 · 영상정보 방침 · INQUIRY), 우측 © 카피라이트, FAMILY 사이트 드롭다운.

### Whitespace Philosophy
홈은 극단적으로 비어 있다 — 1440px 화면에 270px 커버 하나와 세로선뿐. 서브페이지는 반대로 그리드가 화면을 꽉 채운다(거터 15px). "비어 있는 무대 ↔ 꽉 찬 갤러리"의 대비가 리듬을 만든다.

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| 0 — Flat | 테두리·그림자 없음 | 헤더, 카드, 이미지, 푸터 — 사실상 전부 |
| 1 — Hairline | 1px solid `{colors.hairline}` | 정사각 아이콘 버튼, 활성 탭 밑줄, 공지 날짜 디바이더 |
| 2 — Full overlay | 화면 전체 `{colors.surface-dark}` | 전체 메뉴 |

`box-shadow`가 사이트 전체에서 0건이다. 깊이는 다음 두 가지로만 만든다.
- **이미지 딤:** 아티스트 사진을 검정 바탕 위 opacity 0.92로 깔아 흰 텍스트·아이콘이 읽히게 한다(그라데이션 스크림 없음).
- **흑백 반전:** 메뉴를 열면 흰 페이지가 통째로 검정으로 뒤집힌다.

### Motion
- 공지 리스트 진입: `transform 1s cubic-bezier(0.215, 0.61, 0.355, 1)` (easeOutCubic) — 아래에서 떠오르며 등장, `.on` 클래스로 트리거.
- 카드 내부 상태 변화: `0.2s`.
- 아티스트 그리드도 스크롤 진입 시 페이드인(`.grid-item.on`).

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.none}` | 0px | 모든 카드, 이미지, 버튼, 아이콘 박스 — 시스템 기본값 |
| `{rounded.full}` | 50% | 페이지네이션 활성 숫자만 |

라운드 어휘는 사실상 **0px 하나**다. 이것이 Pinterest(16px/32px/pill)와 가장 크게 갈리는 지점이다.

### Photography Geometry
- **릴리즈 커버:** 1:1 정사각, 270px(데스크톱), 각진 모서리.
- **아티스트 사진:** 원본 비율 보존(세로 3:4 전후, 가로 3:2 전후 혼재), 메이슨리 배치.
- **아이콘:** SNS 30px(헤더) / 36px(카드), 정사각 아이콘 버튼 26px.

## Components

> 호버 상태는 공개 DOM에서 정적으로 확인하지 않음. Default / Active 위주로 기술.

### Navigation

**`primary-nav`**
- 배경 `{colors.canvas}`, 패딩 `24px 62px`, 높이 84px, 라운드 `{rounded.none}`, 하단 선 없음.
- 좌: JYP 로고(100×36). 우: `{component.nav-sns-icon}` ×4(YouTube · Instagram · X · Facebook, 간격 20px) → `{component.lang-select}`("KO ▾", KO/EN/CH/JP/ES) → `{component.menu-trigger}`(25×14 햄버거, 2px 바 3개).
- 전역 GNB 텍스트 메뉴가 없다 — 모든 이동은 햄버거 → 오버레이.

**`menu-overlay`**
- 화면 전체 `{colors.surface-dark}`. 가로로 6개 컬럼: JYP · ARTIST · SUSTAINABILITY · IR · AUDITION · RECRUIT.
- 1차: `{typography.menu-category}` `{colors.on-dark}`. 2차: `{component.menu-link}`(`{colors.on-dark-mute}`). 3차: `{component.menu-link-sub}`(`{colors.on-dark-faint}`, 10px 들여쓰기).
- 열리면 헤더 아이콘·언어 선택도 흰색으로 반전.

**`sub-tab` + `sub-tab-active`**
- 페이지 타이틀 바로 아래 가운데 정렬 텍스트 탭(예: ARTIST / ALBUM / VIDEO).
- 기본: `{typography.tab-md}` `{colors.sub}`. 활성: `{typography.tab-active}` `{colors.heading}` + 1px solid 밑줄. 배경·박스 없음.

### Home

**`release-spotlight`**
- 세로 순서: 아티스트명(`{typography.display-artist}`) → 곡명(`{typography.display-xl}`) → `{component.release-cover}` → "Release Date"(`{typography.caption-tight}` `{colors.meta}`) + 날짜 → 세로선 구간 → 설명 1~2줄(`{typography.body-strong}`, 가운데 정렬) → `{component.icon-button-square}` ×3.
- 전체가 `{colors.rule-vertical}` 1px 세로선에 꿰어져 있다.

**`icon-button-square`**
- 26×26, 1px `{colors.hairline}` 테두리, 라운드 0, 흰 바탕. 아이콘: + (more → 디스코그래피), ▶ (YouTube MV), △ (접기/위로).
- 세 개가 붙어서 세로로 쌓인다(간격 0~1px).

### Cards

**`artist-card`**
- 배경 `{colors.surface-image}`, 패딩 0, 라운드 0. 이미지 풀블리드, opacity 0.92.
- 하단 오버레이: 이름(`{typography.label-name}` `{colors.on-dark}`, 가운데 정렬) → 56px 아래 `{component.artist-sns-icon}` 행(Instagram · X · Facebook · YouTube · FANS · SHOP, 36px, 간격 8px).

**`notice-card`**
- 배경 `{colors.surface-card}`, 520×522, 상단 35px 패딩.
- 상단 "NOTICE"(`{typography.overline}` `{colors.mute-faint}`) → 카드 중앙 제목(`{typography.heading-md}` `{colors.heading}`, 좌우 38px) → 하단 날짜·조회수(`{typography.caption-md}` `{colors.mute}`) + 1px `{colors.divider}` 하단선.

### Pagination

**`pagination-item` + `pagination-item-active`**
- 34×34, 패딩 7px, `{typography.body-md}`.
- 기본: 투명 배경, `{colors.sub}` 숫자. 활성: `{colors.pagination-active}` 원형(`{rounded.full}`) + 흰 숫자 — 시스템 유일의 원형 요소.

### Footer

**`footer-section`**
- 배경 `{colors.canvas}`, 좌우 62px, 하단 68px. 상단 구분선 없음.
- 좌: 개인정보처리방침 · 고정형 영상정보처리기기 운영·관리방침 · INQUIRY(`{typography.caption-md}` `{colors.mute}`, 간격 29px). 우: "© JYP ENTERTAINMENT Corp."(12px/500). FAMILY 사이트 링크(AUDITION, RECRUIT, FANS, PUBLISHING, SHOP, BLUE GARAGE, PARTNERS) 드롭다운.

## Do's and Don'ts

### Do
- 크롬은 `{colors.canvas}`와 `{colors.ink}` 두 값으로 끝낸다. 색은 이미지에 맡긴다.
- 모든 카드·이미지·버튼은 `{rounded.none}`. 원형은 페이지네이션 활성 상태에만.
- 위계는 굵기(400 → 500 → 700 → 800)로 만든다. 크기는 30px을 넘기지 않는다.
- 메뉴·탭·라벨은 aktiv-grotesk-extended 영문 대문자로.
- 이미지 위 텍스트는 그라데이션 대신 검정 바탕 + 이미지 opacity 0.92로 가독성을 확보한다.
- 활성 상태는 밑줄 1px 또는 흑백 반전으로 표시한다.
- 홈처럼 "하나만 보여주는" 화면은 여백을 과감하게 비워 두고 중앙 세로선으로 축을 잡는다.

### Don't
- 브랜드 액센트 컬러(빨강·파랑 등)를 크롬에 추가하지 않는다 — 특정 아티스트 컬러와 충돌한다.
- 그림자·그라데이션·블러를 쓰지 않는다. `box-shadow`는 0건이 원칙.
- 라운드 버튼·라운드 카드를 만들지 않는다(Pinterest식 16px pill 금지).
- 본문에 자간을 주지 않는다. extended 서체가 이미 넓다.
- `{colors.surface-card}`(#f4f6f8)를 공지·정보성 카드 외에 남용하지 않는다. 이미지 카드 배경은 검정이다.
- 전역 텍스트 GNB를 헤더에 펼치지 않는다. 내비게이션은 햄버거 → 풀스크린 오버레이로 통일.

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| desktop | 1440px | 기준 — 헤더 좌우 62px, 3열 아티스트 그리드, 2열 공지 |
| desktop-small | ~1100px | 같은 구조, 열 폭만 축소 |
| mobile | 375px | 헤더 패딩 ≈ 16–20px, 로고 70×24, SNS 아이콘 숨김(햄버거·언어만), 페이지 타이틀 30 → 22px, 콘텐츠 상단 94px, 그리드 1열 풀블리드 |

### Touch Targets
햄버거는 모바일에서 40×32(패딩 10px 포함). SNS 아이콘 30px, 홈 정사각 아이콘 버튼 26px은 WCAG 44px 미만 — 신규 구현 시 히트 영역을 44px로 확장할 것.

### Collapsing Strategy
- **헤더:** SNS 아이콘 → 모바일에서 `display:none`. 로고·언어·햄버거만 유지.
- **아티스트 그리드:** 3열 → 1열, 거터 15px → 5px, 좌우 여백 0(풀블리드).
- **페이지 타이틀:** `{typography.page-title}` 30px → 22px.
- **홈 스포트라이트:** 단일 열 구조 그대로, 커버·텍스트가 화면 폭에 맞춰 축소.

### Image Behavior
- 아티스트 사진은 모든 폭에서 원본 비율 유지 — 열 수만 바뀐다.
- 릴리즈 커버는 항상 1:1.
- 그리드 아이템은 스크롤 진입 시 `.on` 클래스로 페이드/슬라이드 인.

## Iteration Guide

1. 한 번에 컴포넌트 하나. YAML 항목을 먼저 확인하고 모든 참조가 풀리는지 본다.
2. 토큰 이름으로 참조한다(`{colors.ink}`, `{component.sub-tab-active}`, `{rounded.none}`).
3. 편집 후 `npx @google/design.md lint design.md`로 `broken-ref`·`contrast-ratio`·`orphaned-tokens`를 확인한다.
4. 상태 변형은 별도 항목으로 추가한다(`-active`, `-disabled`, `-focused`).
5. 기본 본문은 `{typography.body-md}`(14px). 영문 라벨은 대문자, 한글 콘텐츠는 그대로.
6. 새 색이 필요하다고 느끼면 먼저 흑백 반전·밑줄·굵기로 풀 수 있는지 본다. 이 시스템의 강점은 색을 추가하지 않는 것.
7. 새 컴포넌트는 "각진 사각형 + 흑/백 + 이미지" 어휘로 표현 가능한지 먼저 검토한다.

## Known Gaps

- **호버 상태 미확인** — 정적 computed style만 수집. 메뉴·카드 호버 반응은 실제 브라우저에서 추가 확인 필요.
- **폼 요소(입력창·버튼·포커스·에러) 미수집** — CONTACT/INQUIRY, IR INQUIRY 폼은 이번 분석 범위 밖.
- **Semantic 컬러(에러·성공·포커스 링) 없음** — 공개 페이지에서 확인되지 않음.
- **태블릿 구간 브레이크포인트 정확값 미측정** — 375px와 1100/1440px만 확인.
- **아티스트 서브사이트(`*.jype.com`)·AUDITION·RECRUIT·FANS** — 별도 디자인 시스템이며 여기 포함하지 않음.
- **ALBUM·VIDEO·HISTORY·SUSTAINABILITY·IR 페이지** — 같은 헤더·탭 규칙을 공유할 것으로 보이나 개별 컴포넌트는 미수집.
