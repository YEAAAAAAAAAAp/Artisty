# 🚀 Artisty 배포 가이드

## 📋 배포 전 체크리스트

### ✅ 코드 품질
- [x] HTML/CSS/JavaScript 문법 오류 없음
- [x] GA4 이벤트 추적 정상 작동
- [x] 반응형 디자인 모든 디바이스에서 테스트 완료
- [x] 접근성 개선 (다크모드, 애니메이션 감소 지원)
- [x] 성능 최적화 (will-change, 이미지 지연 로딩)

### ✅ 기능 테스트
- [x] 탭 전환 기능
- [x] 모달 열기/닫기
- [x] 폼 검증
- [x] GA4 이벤트 전송
- [x] 스크롤 애니메이션

## 🌐 배포 옵션

### 1. GitHub Pages (무료)
```bash
# 저장소 생성 후
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-username/artisty-landing.git
git push -u origin main

# GitHub Pages 설정
# Settings > Pages > Source: Deploy from a branch > main
```

### 2. Netlify (무료)
```bash
# Netlify CLI 설치
npm install -g netlify-cli

# 배포
netlify deploy --prod --dir .
```

### 3. Vercel (무료)
```bash
# Vercel CLI 설치
npm install -g vercel

# 배포
vercel --prod
```

### 4. Firebase Hosting
```bash
# Firebase CLI 설치
npm install -g firebase-tools

# 초기화
firebase init hosting

# 배포
firebase deploy
```

## 🔧 로컬 개발 환경

### Node.js 사용
```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev
# 또는
npm start
```

### Python 사용
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

### VS Code Live Server
- VS Code에서 Live Server 확장 설치
- index.html 우클릭 > "Open with Live Server"

## 📊 GA4 설정 확인

### 추적 ID 확인
- GA4 추적 ID: `G-01JMZ0MSB7`
- gtag 스크립트 정상 로딩 확인
- 이벤트 전송 테스트

### 배포 후 확인사항
1. GA4 실시간 리포트에서 데이터 수신 확인
2. 이벤트 발생 현황 모니터링
3. 전환율 추적 정상 작동 확인

## 🎯 성능 최적화

### 이미 최적화된 항목
- ✅ CSS 최적화 (will-change 속성)
- ✅ 이미지 지연 로딩
- ✅ 폰트 최적화 (Google Fonts)
- ✅ 애니메이션 최적화
- ✅ 접근성 개선

### 추가 최적화 권장사항
- CDN 사용 (Cloudflare, AWS CloudFront)
- 이미지 압축 (WebP 형식)
- Gzip 압축 활성화
- 브라우저 캐싱 설정

## 🔒 보안 설정

### HTTPS 강제
- 모든 배포 플랫폼에서 HTTPS 자동 적용
- HTTP → HTTPS 리다이렉트 설정

### 콘텐츠 보안 정책 (CSP)
```html
<meta http-equiv="Content-Security-Policy" 
      content="default-src 'self'; 
               script-src 'self' 'unsafe-inline' https://www.googletagmanager.com; 
               style-src 'self' 'unsafe-inline' https://fonts.googleapis.com;
               font-src 'self' https://fonts.gstatic.com;
               img-src 'self' https://images.unsplash.com data:;">
```

## 📱 모바일 최적화

### 테스트 완료된 디바이스
- ✅ iPhone (Safari)
- ✅ Android (Chrome)
- ✅ iPad (Safari)
- ✅ 태블릿 (다양한 크기)

### PWA 설정 (선택사항)
```json
{
  "name": "Artisty",
  "short_name": "Artisty",
  "description": "예술가-콜렉터 상거래 플랫폼",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#ffffff",
  "theme_color": "#3b82f6"
}
```

## 🚨 배포 후 모니터링

### GA4 대시보드 확인
1. **실시간 사용자**: 현재 활성 사용자 수
2. **이벤트 발생**: 8개 이벤트 실시간 추적
3. **전환율**: 사전예약 신청 전환율
4. **사용자 타입**: 콜렉터 vs 예술가 비율

### 성능 모니터링
- 페이지 로딩 속도
- 모바일 성능 점수
- Core Web Vitals 지표

### 오류 모니터링
- JavaScript 오류
- 404 오류
- 폼 제출 오류

## 📞 지원 및 문의

배포 과정에서 문제가 발생하면:
1. 브라우저 개발자 도구에서 오류 확인
2. GA4 실시간 리포트에서 이벤트 전송 확인
3. 모바일 디바이스에서 반응형 테스트

---

**배포 성공을 기원합니다! 🎨✨**
