# 🌿 agri-insights

> 스마트팜 환경 데이터(온·습도, CO₂, 지온, 일사량) 분석 및 작물 생산량 예측 모니터링 시스템

`agri-insights`는 농림축산식품 공공데이터 포털의 스마트팜 빅데이터 API를 연동하여 시계열 환경 데이터를 시각화하고, 작물 생육 상태 및 생산성 예측 인사이트를 제공하는 반응형 웹 대시보드 프로젝트입니다.

---

## 📸 Key Features

* **실시간 온실 환경 모니터링**: 온·습도, CO₂ 농도, 지온, 적산일사량 등 주요 환경 센서 데이터 시각화 (차트 및 카드 UI)
* **생산량 및 생육 예측 인사이트**: 수집된 시계열 데이터 기반 작물 수확량 예측 모델 데이터 연동
* **반응형 대시보드 UI**: 모바일, 태블릿, 데스크톱 환경에 최적화된 웹 표준 및 접근성 준수 레이아웃
* **공통 UI 컴포넌트화**: 차트 카드, 환경 상태 뱃지, 데이터 테이블 등 재사용 가능한 컴포넌트 구조

---

## 🛠 Tech Stack

### Web Front-End
* **Language / Core**: HTML5, CSS3, JavaScript (ES6+)
* **UI Components & Layout**: HTML5 Semantic Elements, CSS Grid & Flexbox
* **Data Visualization**: Chart.js (또는 D3.js, Recharts 등)

### Data Processing & Integration
* **API Integration**: 농림축산식품부 스마트팜 데이터 마트 Open API (JSON)
* **Data Automation**: Python (Pandas, Requests) 데이터 수집 및 전처리

---

## 📂 Project Structure

```text
agri-insights/
├── assets/
│   ├── css/           # 공통 및 컴포넌트 스타일시트 (reset, layout, components)
│   ├── js/            # API 데이터 연동, 차트 렌더링, UI 컨트롤러
│   └── images/        # 아이콘 및 정적 이미지 리소스
├── data/              # API 수집 데이터 샘플 및 전처리 결과 (CSV/JSON)
├── scripts/           # 스마트팜 API 데이터 자동 수집 Python 스크립트
├── index.html         # 메인 스마트팜 대시보드 페이지
└── README.md