# 한국문화관광연구원(KCTI) 현황 및 주요 현안 대시보드

문화체육관광부 소관 연구개발목적기관인 **한국문화관광연구원(Korea Culture & Tourism Institute)** 의 조직·예산·연구사업·핵심 현안을 한 페이지로 요약한 정적(Static) 웹 대시보드입니다.

> 데이터 기준: 2026년(‘26.8.21. 기준)

---

## 📌 주요 특징

- **완전한 단일 파일 (`index.html`)** — 별도 빌드 도구 없이 브라우저에서 바로 열람 가능
- **반응형(Responsive) 디자인** — PC / 태블릿 / 스마트폰에서 모두 최적화
- **`clamp()` 기반 유동 타이포그래피** — 화면 크기에 따라 글자·간격이 자연스럽게 확대/축소
- **접근성 준수** — `aria-*`, `role`, `focus-visible`, `prefers-reduced-motion` 지원
- **모바일 친화적 테이블** — 좌우 스크롤 힌트 + 부드러운 그림자 인디케이터
- **모바일 햄버거 메뉴** — 좁은 화면에서 자동 전환
- **Chart.js 인터랙티브 차트** — 툴팁, 백분율 표시, 통화 포맷팅
- **연구과제 필터링** — 39건 과제를 유형/분야별 실시간 필터
- **인쇄(Print) 최적화** — 보고서/자료 출력용 스타일 포함

---

## 🖥 구성 섹션

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

## 🚀 사용 방법

### 로컬에서 열기
```bash
git clone <this-repo>
cd <this-repo>
# 파일을 브라우저로 열기
open index.html    # macOS
start index.html   # Windows
xdg-open index.html # Linux
```

### 로컬 서버로 서빙 (권장)
```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve .
```

브라우저에서 `http://localhost:8080` 접속

---

## 🌐 GitHub Pages 배포

1. GitHub 저장소에 이 리포지토리 업로드
2. **Settings → Pages** 이동
3. **Source: Deploy from a branch** 선택
4. **Branch: `main` / (root)** 지정 후 Save
5. 1~2분 후 `https://<username>.github.io/<repo-name>/` 로 접속

---

## 🎨 사용 기술

- **HTML5 · CSS3 · Vanilla JavaScript** (프레임워크 無)
- **[Chart.js](https://www.chartjs.org/)** — 데이터 시각화
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

## 🔧 커스터마이징

CSS 상단의 `:root` 디자인 토큰을 수정하여 색상·간격·폰트 크기를 한 번에 조정할 수 있습니다.

```css
:root {
  --primary: #1e3a8a;      /* 주요 색상 */
  --primary-light: #2563eb;
  --accent: #d97706;
  --bg-body: #f5f7fb;
  /* ... */
}
```

---

## 📄 라이선스

본 대시보드의 **데이터**는 한국문화관광연구원의 공식 자료를 기반으로 하며, 각 항목의 저작권은 원 저작자에게 귀속됩니다.

대시보드의 **소스 코드(레이아웃/스타일/스크립트)** 는 자유롭게 참고·수정하실 수 있습니다.

---

## 🔗 관련 링크

- [KCTI 공식 웹사이트](https://www.kcti.re.kr)
- [문화예술지식정보시스템 (ACKIS)](https://policydb.kcti.re.kr)
- [관광지식정보시스템 (TourGo)](https://know.tour.go.kr)
- [관광개발정보시스템 (TDSS)](https://www.tdss.kr)
