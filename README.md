# 📷 무음 카메라 (Silent Camera)

> 완전 무음 카메라 PWA — 아이폰 홈화면에 추가해서 앱처럼 사용하세요!

---

## ✨ 기능

- 🔇 **완전 무음** 촬영 (웹앱이라 셔터 소리 없음)
- 📐 **전체화면** 카메라 프리뷰
- 🔍 **20× 디지털 줌** — 반원형 슬라이더 + 핀치 줌
- 🎨 **8가지 필터** — Kodak, Sony, Vintage, Neon, Cyberpunk, Old Film, 日本カメラ
- 🔄 **전면/후면** 카메라 전환
- 📱 **PWA** — 아이폰 홈화면에 추가 가능
- ⚡ **플래시** & **그리드** 지원
- 💾 **자동 저장** — 공유 시트를 통해 사진앱에 저장

---

## 🚀 GitHub Pages에 올리기

### 1단계: GitHub 저장소 만들기

```bash
# 이 폴더를 GitHub에 올리세요
git init
git add .
git commit -m "무음 카메라 v1.0"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/silent-camera.git
git push -u origin main
```

### 2단계: GitHub Pages 활성화

1. GitHub 저장소 → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** / **(root)**
4. **Save** 클릭
5. 약 1-2분 후 URL 생성됨: `https://YOUR_USERNAME.github.io/silent-camera/`

### 3단계: 아이폰 홈화면에 추가

1. 아이폰 **Safari**로 위 URL 접속
2. 하단 **공유 버튼** (□↑) 탭
3. **"홈 화면에 추가"** 선택
4. 이름 확인 후 **"추가"** 탭
5. 홈화면에 앱 아이콘 생성 완료! 🎉

---

## 📸 사용법

| 기능 | 사용법 |
|------|--------|
| 촬영 | 하단 큰 원형 버튼 탭 |
| 줌 조절 | 오른쪽 반원 슬라이더 드래그 또는 두 손가락 핀치 |
| 줌 초기화 | 반원 슬라이더 더블탭 |
| 카메라 전환 | 우하단 전환 버튼 |
| 필터 변경 | 하단 필터 칩 스와이프 & 탭 |
| 그리드 | 좌상단 그리드 버튼 |
| 플래시 | 우상단 플래시 버튼 |
| 사진 공유/저장 | 좌하단 썸네일 탭 |

---

## ⚠️ 알아두세요

### 사진 저장 방식
- **iOS (iPhone)**: 촬영 시 **공유 시트**가 뜹니다. "이미지 저장"을 탭하면 사진앱에 저장됩니다.
- **Android**: 자동으로 다운로드 폴더에 저장됩니다.

### 화질 안내
- 웹 카메라 API의 해상도는 보통 **1080p~4K**입니다.
- 네이티브 카메라 앱의 12MP+ 촬영과는 차이가 있을 수 있습니다.
- JPEG 품질 95%로 최대한 고화질을 유지합니다.

### 무음 원리
- 웹 앱은 기본적으로 셔터 소리를 재생하지 않습니다.
- 별도의 음소거 트릭이 필요 없이 **원래 무음**입니다! 🔇

---

## 📁 파일 구조

```
silent-camera/
├── index.html          # 메인 앱 (HTML + CSS + JS 올인원)
├── manifest.json       # PWA 매니페스트
├── sw.js              # 서비스 워커 (오프라인 지원)
├── apple-touch-icon.png # iOS 홈화면 아이콘
├── icons/             # PWA 아이콘 (다양한 크기)
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-180.png
│   ├── icon-192.png
│   ├── icon-384.png
│   └── icon-512.png
├── generate_icons.py  # 아이콘 생성 스크립트 (선택)
└── README.md          # 이 파일
```

---

## 🛠 로컬 테스트

```bash
# Python 간단 서버로 테스트
cd silent-camera
python3 -m http.server 8080

# 브라우저에서 http://localhost:8080 접속
# ※ HTTPS가 아니면 카메라 접근이 제한될 수 있습니다.
# localhost는 예외적으로 HTTP에서도 카메라 사용 가능
```

---

Made with ❤️ | 무음 카메라 v1.0
