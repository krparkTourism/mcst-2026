# 한국문화관광연구원(KCTI) 현황 및 주요 현안 대시보드

문화체육관광부 소관 연구개발목적기관인 **한국문화관광연구원(Korea Culture & Tourism Institute)** 의 조직·예산·연구사업·핵심 현안을 한 페이지로 요약한 정적(Static) 웹 대시보드입니다.

> **🔗 배포 URL:** https://krparktourism.github.io/mcst-2026/
> **📅 데이터 기준:** 2026년 (‘26.8.21. 기준)

---

## 📌 주요 특징

- **QR 코드 접속 지원** — 상단 카드의 QR 코드로 모바일에서 즉시 접속
- **원본 HWP 자료 다운로드** — `문화전략담당관 기관 및 현안설명 자료(2026.8.21)` 첨부
- **완전한 단일 파일 (`index.html`)** — 별도 빌드 도구 없이 브라우저에서 바로 열람
- **반응형(Responsive) 디자인** — PC / 태블릿 / 스마트폰 모두 최적화
- **`clamp()` 유동 타이포그래피** — 화면 크기에 따라 글자·간격이 자연스럽게 확대/축소
- **접근성** — `aria-*`, `role`, `focus-visible`, `prefers-reduced-motion` 지원
- **모바일 친화적 테이블** — 좌우 스크롤 힌트 + 그림자 인디케이터
- **모바일 햄버거 메뉴** — 좁은 화면 자동 전환
- **Chart.js 인터랙티브 차트** — 툴팁, 백분율 표시, 통화 포맷팅
- **연구과제 실시간 필터** — 39건 과제를 유형·분야별 즉시 필터링
- **인쇄(Print) 최적화** — 보고서 출력용 스타일 포함

---

## 📁 저장소 파일 구성

```
mcst-2026/
├─ index.html                                             # 대시보드 본체
├─ README.md                                              # 이 문서
└─ 문화전략담당관_기관_및_현안설명_자료_2026.8.21.hwp    # 원본 자료 (다운로드용)
```

---

## 🚀 GitHub 저장소에 파일 업로드하는 방법

### ✅ 방법 1. **웹 브라우저에서 직접 업로드** (가장 쉬움 - 추천)

1. GitHub 로그인 후 https://github.com/new 로 이동
2. **Repository name**: `mcst-2026` 입력
3. **Public** 선택 (Pages는 무료 계정에서 Public만 지원)
4. **Add a README file** 체크 해제 (기존 README를 올릴 예정이므로)
5. **Create repository** 클릭
6. 새로 만들어진 저장소 화면에서 **Add file → Upload files** 클릭
7. 3개 파일을 드래그 앤 드롭:
   - `index.html`
   - `README.md`
   - `문화전략담당관_기관_및_현안설명_자료_2026.8.21.hwp`
8. 아래 **Commit changes** 클릭 → 업로드 완료

> ⚠️ 한글 파일명이 업로드 후 깨져 보이면 파일명을 영문으로 변경하고 `index.html`의 다운로드 링크(`href="..."`)도 함께 수정하세요.

---

### ✅ 방법 2. **Git 명령어로 업로드** (개발자용)

```bash
# 1) 로컬 폴더 준비
mkdir mcst-2026 && cd mcst-2026
# index.html, README.md, HWP 파일을 이 폴더에 복사

# 2) Git 초기화
git init
git branch -M main

# 3) 파일 커밋
git add .
git commit -m "Initial: KCTI 2026 대시보드 업로드"

# 4) GitHub 저장소 연결 (본인 아이디로 수정)
git remote add origin https://github.com/krparktourism/mcst-2026.git

# 5) 원격 저장소로 푸시
git push -u origin main
```

> 💡 처음이라면 GitHub 로그인 창이 뜹니다. 비밀번호 대신 **Personal Access Token(PAT)** 을 입력해야 합니다.
> - PAT 발급: https://github.com/settings/tokens → **Generate new token (classic)** → `repo` 권한 체크

---

### ✅ 방법 3. **GitHub Desktop** (GUI - 초보자 친화적)

1. https://desktop.github.com/ 에서 GitHub Desktop 설치
2. **File → New Repository** → 이름 `mcst-2026`
3. 로컬 폴더에 위 3개 파일을 복사
4. GitHub Desktop 화면에서 **Commit to main** 클릭
5. **Publish repository** 클릭 → Public 설정 → 완료

---

## 🌐 GitHub Pages 배포 방법

파일 업로드가 완료되면 아래 순서로 무료 웹호스팅을 활성화합니다.

1. 저장소 페이지에서 상단 **Settings** 클릭
2. 왼쪽 사이드바에서 **Pages** 클릭
3. **Source** 섹션에서:
   - **Deploy from a branch** 선택
   - **Branch:** `main` / **Folder:** `/ (root)` 지정
4. **Save** 클릭
5. 1~2분 대기 후 페이지 상단에 표시되는 URL 확인:
   ```
   https://krparktourism.github.io/mcst-2026/
   ```

### 배포 확인 방법
- 위 URL에 접속하여 대시보드가 정상 표시되는지 확인
- 대시보드 상단의 **QR 코드**를 스마트폰으로 스캔하여 모바일 확인
- **원본 HWP 다운로드** 버튼 클릭 시 파일이 정상적으로 내려받아지는지 확인

---

## 🔧 파일 수정 후 재배포

```bash
# 파일 수정 후
git add .
git commit -m "대시보드 데이터 업데이트"
git push
```

푸시하면 자동으로 GitHub Pages가 재빌드되며, **1~2분 후** 반영됩니다.

---

## 🖥 대시보드 구성 섹션

| # | 섹션 | 내용 |
|---|------|------|
| Ⅰ | 연구원 개요 및 설립 근거 | 법정 근거, 기관 성격, 주요 연혁 타임라인 |
| Ⅱ | 조직 및 인력 현황 | 5개 본부·1실 체제 표 + 도넛 차트 |
| Ⅲ | 예산 및 재무 구조 | 연도별 예산 추이, 수입/지출 구성, 상세 비교표 |
| Ⅳ | 주요 사업 포트폴리오 | 기본연구 단가, 특정목적출연금사업 현황 |
| Ⅴ | 3대 핵심 현안 | 인력·출연금, 지방이전, 정보화 전담인력 |
| Ⅵ | 붙임 자료 | 39건 연구과제, 국가승인통계 9종, 평가 근거 |
| Ⅶ | 대국민 데이터 서비스 | ACKIS · TourGo · TDSS 플랫폼 링크 |

---

## 💻 로컬에서 실행

```bash
# 파일을 브라우저로 열기
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux

# 또는 로컬 서버로 (권장 - HWP 다운로드가 정상 동작)
python3 -m http.server 8080
# → http://localhost:8080
```

---

## 🎨 사용 기술

- **HTML5 · CSS3 · Vanilla JavaScript** (프레임워크 無)
- **[Chart.js](https://www.chartjs.org/)** — 데이터 시각화
- **[QRCode.js](https://github.com/davidshimjs/qrcodejs)** — QR 코드 생성
- **[Pretendard](https://cactus.tistory.com/306)** — 한글 최적화 웹폰트
- **[Font Awesome 6](https://fontawesome.com/)** — 아이콘

---

## 📱 반응형 브레이크포인트

| 화면 크기 | 레이아웃 |
|-----------|----------|
| ≤ 480px | 모바일 (단일 컬럼, 축소 패딩) |
| 481 ~ 767px | 태블릿 세로 (2 컬럼 KPI) |
| 768 ~ 899px | 태블릿 가로 |
| 900 ~ 1023px | 소형 데스크톱 (햄버거 메뉴 해제) |
| ≥ 1024px | 데스크톱 (풀 4 컬럼) |

---

## 🎨 커스터마이징

CSS 상단의 `:root` 디자인 토큰을 수정하여 색상·간격·폰트 크기를 한 번에 조정할 수 있습니다.

```css
:root {
  --primary: #1e3a8a;
  --primary-light: #2563eb;
  --accent: #d97706;
  --bg-body: #f5f7fb;
  /* ... */
}
```

QR 코드가 가리키는 URL을 변경하려면 `index.html`에서 `targetUrl` 및 `access-url` 항목을 수정하면 됩니다.

---

## ❓ 자주 발생하는 문제 (FAQ)

**Q. QR 코드가 표시되지 않아요.**
→ 인터넷 연결을 확인하세요. `qrcodejs` CDN이 로딩되지 않으면 `api.qrserver.com`으로 자동 폴백됩니다.

**Q. HWP 다운로드가 안 돼요.**
→ 로컬에서 `file://` 프로토콜로 열면 다운로드가 차단될 수 있습니다. `python3 -m http.server`로 서버 실행 후 확인하세요. GitHub Pages 배포 후에는 정상 작동합니다.

**Q. 한글 파일명이 깨져요.**
→ HWP 파일명을 영문(예: `kcti-2026-briefing.hwp`)으로 바꾸고 `index.html`의 `href` 속성도 함께 수정하세요.

**Q. GitHub Pages URL이 다르게 나와요.**
→ 저장소 이름을 `mcst-2026`으로, 소유자 계정을 `krparktourism`으로 정확히 맞춰야 `https://krparktourism.github.io/mcst-2026/` URL이 됩니다.

---

## 📄 라이선스

본 대시보드의 **데이터**는 한국문화관광연구원의 공식 자료를 기반으로 하며, 저작권은 원 저작자에게 귀속됩니다.
**소스 코드(레이아웃/스타일/스크립트)** 는 자유롭게 참고·수정하실 수 있습니다.

---

## 🔗 관련 링크

- 🌐 [KCTI 공식 웹사이트](https://www.kcti.re.kr)
- 🎨 [문화예술지식정보시스템 (ACKIS)](https://policydb.kcti.re.kr)
- ✈️ [관광지식정보시스템 (TourGo)](https://know.tour.go.kr)
- 🗺️ [관광개발정보시스템 (TDSS)](https://www.tdss.kr)
