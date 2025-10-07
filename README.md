# 🎨 Artisty - 예술가-콜렉터 상거래 플랫폼

> 예술가와 콜렉터를 연결하는 프리미엄 플랫폼의 랜딩페이지

## 📋 프로젝트 개요

Artisty는 예술가와 콜렉터를 연결하는 혁신적인 상거래 플랫폼의 랜딩페이지입니다. AI 기반 작품 분석, 안전한 거래 시스템, 그리고 전문적인 포트폴리오 제작 도구를 통해 예술의 진정한 가치를 발견할 수 있습니다.

## ✨ 주요 기능

### 🎯 콜렉터 전용 기능
- **AI 기반 스토리 탐색**: 인공지능이 분석한 작품의 숨겨진 스토리와 의미 발견
- **안심 거래**: 검증된 작가와의 안전한 거래 시스템
- **즉시 소통·견적**: 작가와 직접 대화하며 맞춤형 견적 받기

### 🧑‍🎨 예술가 전용 기능
- **포트폴리오 최적화**: 전문적인 포트폴리오 쉽게 제작
- **거래 관리**: 작품 판매부터 배송까지 체계적 관리
- **고객 관계 관리**: 콜렉터와의 지속적인 관계 구축

## 🚀 기술 스택

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Analytics**: Google Analytics 4 (GA4)
- **Design**: 반응형 웹 디자인, 모던 UI/UX
- **Fonts**: Google Fonts (Inter)
- **Images**: Unsplash API

## 📊 GA4 이벤트 추적

### 🎯 추적되는 이벤트 (8개)

| 이벤트명 | 카테고리 | 설명 | 전환 여부 |
|---------|---------|------|----------|
| `page_view` | engagement | 페이지 로드 | ❌ |
| `tab_switched` | navigation | 탭 전환 (콜렉터/예술가) | ❌ |
| `preorder_modal_opened` | engagement | 사전예약 모달 열림 | ❌ |
| `preorder_submitted` | conversion | 사전예약 신청 완료 | ✅ |
| `feature_coming_soon_viewed` | engagement | 준비중 기능 모달 열림 | ❌ |
| `feature_notification_requested` | engagement | 기능 알림 신청 | ❌ |
| `collector_experience_started` | engagement | 콜렉터 체험 시작 | ❌ |
| `artist_experience_started` | engagement | 예술가 체험 시작 | ❌ |

### 🎨 추적되는 CTA 버튼 (12개)

#### 탭 네비게이션 (2개)
- 콜렉터 탭 버튼
- 예술가 탭 버튼

#### 메인 CTA (2개)
- 콜렉터 체험하기 버튼
- 예술가 체험하기 버튼

#### 기능별 CTA (6개)
- AI 작품 탐색 버튼
- 거래 프로세스 보기 버튼
- 작가와 대화하기 버튼
- 포트폴리오 만들기 버튼
- 거래 정보 설정 버튼
- 고객 정보 시작 버튼

#### 모달 내부 CTA (2개)
- 사전예약 신청 버튼
- 출시 알림 받기 버튼

## 🎨 디자인 특징

### 🎯 디자인 시스템
- **컬러 팔레트**: 파란색(#3b82f6)과 보라색(#8b5cf6) 포인트 컬러
- **배경**: 흰색 기반 그라데이션
- **타이포그래피**: Inter 폰트 패밀리
- **레이아웃**: 2단 그리드 레이아웃 (데스크톱), 1단 세로 레이아웃 (모바일)

### 📱 반응형 디자인
- **데스크톱**: 1200px 이상
- **태블릿**: 768px - 1199px
- **모바일**: 768px 이하

### ✨ 인터랙션
- **애니메이션**: CSS3 transitions, transforms
- **호버 효과**: 버튼, 카드, 이미지 호버 애니메이션
- **모달**: 부드러운 fade-in/out 효과
- **스크롤**: Intersection Observer API 활용

## 📁 파일 구조

```
Artisty/
├── index.html          # 메인 HTML 파일 (모든 기능 포함)
├── README.md          # 프로젝트 문서
└── .gitignore         # Git 무시 파일
```

## 🚀 설치 및 실행

### 1. 저장소 클론
```bash
git clone [repository-url]
cd Artisty
```

### 2. 로컬 서버 실행
```bash
# Python 3
python -m http.server 8000

# Node.js (http-server)
npx http-server

# VS Code Live Server 확장 사용
```

### 3. 브라우저에서 확인
```
http://localhost:8000
```

## 📊 GA4 설정

### 추적 ID
```
G-01JMZ0MSB7
```

### 이벤트 파라미터
- `event_category`: 이벤트 카테고리
- `event_label`: 이벤트 라벨
- `user_type`: 사용자 타입 (collector/artist)
- `feature_name`: 기능명
- `value`: 전환 값 (사전예약 신청 시 1)

## 🎯 사용자 여정

### 콜렉터 여정
1. **랜딩** → 페이지 로드 이벤트
2. **탭 선택** → 콜렉터 탭 클릭
3. **기능 탐색** → AI 작품 탐색, 안심 거래, 즉시 소통 버튼 클릭
4. **체험 시작** → 체험하기 버튼 클릭
5. **사전예약** → 이름/이메일 입력 후 신청

### 예술가 여정
1. **랜딩** → 페이지 로드 이벤트
2. **탭 선택** → 예술가 탭 클릭
3. **기능 탐색** → 포트폴리오, 거래 관리, 고객 관계 버튼 클릭
4. **체험 시작** → 체험하기 버튼 클릭
5. **사전예약** → 이름/이메일 입력 후 신청

## 📈 성과 지표

### 주요 KPI
- **전환율**: 사전예약 모달 열림 대비 신청 완료 비율
- **참여도**: 기능별 CTA 클릭률
- **사용자 타입**: 콜렉터 vs 예술가 비율
- **기능 관심도**: 준비중 기능별 관심도

### GA4 대시보드 확인 항목
- 실시간 사용자 수
- 이벤트 발생 현황
- 전환 퍼널 분석
- 사용자 행동 플로우

## 🔧 개발 정보

### 브라우저 지원
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### 성능 최적화
- **이미지 최적화**: Unsplash API 활용
- **폰트 최적화**: Google Fonts 비동기 로딩
- **CSS 최적화**: 효율적인 선택자 사용
- **JavaScript 최적화**: 이벤트 위임 활용

## 📝 라이선스

© 2025 Artisty Platform. All rights reserved.

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 문의

프로젝트에 대한 문의사항이 있으시면 언제든지 연락주세요.

---

**Artisty** - 예술의 진정한 가치를 발견하는 곳 🎨✨