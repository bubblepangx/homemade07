# 무음 카메라

> silent moments, captured softly

킨포크 감성의 올인원 무음 카메라 웹앱 (PWA)

---

## 기능

- **무음 촬영** — 시스템 셔터음 없이 조용하게
- **자동 저장** — 촬영 즉시 다운로드
- **전면/후면 전환** · **줌 1.0~3.0x** · **격자 가이드**
- **타이머** 3/5/10초 · **연속촬영** 15초 간격
- **46종 필터** — 감성, 필름, 일본, 아트, 증명 6개 카테고리
- **뷰티 보정** — 8종 프리셋 + Skin/V-Line/Eyes 조절
- **사진 편집** — 밝기/대비/채도, 텍스트, 스티커 25종, 프레임 7종
- **AI 스타일** — 웹툰/지브리/치비/픽셀아트 등 8종
- **갤러리** — 촬영/편집 사진 관리, 공유, 삭제
- **PWA** — 홈화면 설치, 오프라인 지원

---

## GitHub Pages 배포 (5분)

### 1. 저장소 만들기
- github.com → **+** → **New repository**
- 이름: `mueum-camera` → **Public** → **Create**

### 2. 파일 업로드
- **Add file** → **Upload files**
- 5개 파일 모두 업로드:
  - `index.html`
  - `manifest.json`
  - `sw.js`
  - `icon-192.svg`
  - `icon-512.svg`
- **Commit changes**

### 3. Pages 활성화
- **Settings** → **Pages**
- Branch: **main** / **(root)** → **Save**

### 4. 접속
- 약 1~2분 후: **https://[아이디].github.io/mueum-camera/**

---

## 홈화면 설치

### iPhone
Safari → 공유(□↑) → **홈 화면에 추가**

### Android
Chrome → 메뉴(⋮) → **앱 설치** 또는 **홈 화면에 추가**

---

## 파일 구조

```
mueum-camera/
├── index.html      ← 앱 전체
├── manifest.json   ← PWA 설정
├── sw.js           ← 서비스 워커
├── icon-192.svg    ← 앱 아이콘
└── icon-512.svg    ← 앱 아이콘 (큰 사이즈)
```
