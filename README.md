# 최민호 포트폴리오 웹사이트

안녕하세요! 저는 최민호 입니다. 프롭테크 기술을 공부하고 있는 대학생입니다. 이 저장소는 제 개인 포트폴리오 웹사이트입니다.

## 프로젝트 정보

- **이름**: 최민호
- **직업 및 소속**: 대학생
- **소개**: 프롭테크 기술을 공부하고 있어요
- **특기/취미**: 집값 분석

## 기술 스택

- HTML5
- CSS3 (반응형 디자인)
- Vanilla JavaScript (프레임워크 없음)
- GitHub Pages (배포)

## 프로젝트 구조

```
.
├── index.html              # 메인 페이지
├── styles/
│   └── main.css           # 메인 스타일시트
├── scripts/
│   └── main.js            # 메인 JavaScript
├── assets/
│   └── images/            # 이미지 파일 (프로필 사진 등)
├── README.md              # 프로젝트 설명 (이 파일)
└── .gitignore             # Git 무시 파일

```

## 기능

### 핵심 기능
- ✅ 반응형 디자인 (모바일, 태블릿, 데스크톱)
- ✅ 부드러운 스크롤 네비게이션
- ✅ 모바일 메뉴 토글
- ✅ 활성 링크 강조
- ✅ 섹션 스크롤 애니메이션
- ✅ Scroll to Top 버튼
- ✅ 다크모드 지원 (브라우저 설정)
- ✅ 접근성 고려 (ARIA 레이블, 키보드 네비게이션)

### 섹션

1. **Hero Section** - 이름, 직업, 자기소개 및 CTA 버튼
2. **About Section** - 상세 소개 및 교육 정보
3. **Skills Section** - 특기 및 관심사 카드
4. **Contact Section** - 연락처 정보 및 소셜 미디어 링크
5. **Navigation** - 부드러운 스크롤 네비게이션
6. **Footer** - 저작권 정보

## GitHub Pages 배포 방법

### 1단계: GitHub Pages 활성화

```bash
# 1. 저장소 설정으로 이동
# GitHub의 이 저장소 > Settings > Pages

# 2. 배포 설정
# - Source: Deploy from a branch
# - Branch: main (또는 gh-pages)
# - Directory: / (root)

# 3. Save 클릭
```

### 2단계: 저장소 이름 확인

**방법 A: 사용자명 저장소 (권장)**
```
저장소명: <username>.github.io
URL: https://<username>.github.io
```

**방법 B: 프로젝트 저장소**
```
저장소명: inu-lecture-resume
URL: https://<username>.github.io/inu-lecture-resume
```

### 3단계: 배포

```bash
# 로컬 저장소에서
git add .
git commit -m "Initial portfolio setup"
git push origin main
```

### 4단계: 확인

- GitHub 저장소의 Settings > Pages에서 배포 상태 확인
- 5-10분 후 제공된 URL에서 웹사이트 접속 가능

## 로컬 개발

### 미리보기

로컬에서 웹사이트를 미리볼 수 있습니다:

```bash
# Python이 있는 경우
python -m http.server 8000

# Node.js가 있는 경우
npx http-server

# PHP가 있는 경우
php -S localhost:8000
```

그 후 브라우저에서 `http://localhost:8000` 접속

### 파일 수정

- `index.html` - 콘텐츠 수정
- `styles/main.css` - 스타일 변경
- `scripts/main.js` - 기능 추가/수정
- `assets/images/` - 프로필 사진 추가

## 프로필 사진 추가

1. `assets/images/` 폴더에 `profile.jpg` 파일 추가
2. 최적 크기: 150x150px 이상
3. 권장 형식: JPG 또는 PNG

## 카스터마이징

### 색상 변경

`styles/main.css`의 CSS 변수를 수정:

```css
:root {
    --primary-color: #3B82F6;      /* 주색 */
    --secondary-color: #1E40AF;    /* 보조색 */
    --accent-color: #EC4899;       /* 강조색 */
    /* ... 다른 변수들 */
}
```

### 폰트 변경

Google Fonts에서 선택: https://fonts.google.com

`index.html`의 `<head>` 섹션에 추가:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=YOUR_FONT&display=swap" rel="stylesheet">
```

그 후 `styles/main.css`에서 `--font-sans` 변수 수정

### 내용 수정

`index.html` 파일에서:
- 이름, 직업, 자기소개 수정
- 연락처 정보 업데이트
- 소셜 미디어 링크 추가/수정

## 성능 최적화

### 이미지 최적화
- TinyPNG (https://tinypng.com) - 이미지 압축
- WebP 포맷 변환으로 더 작은 파일 크기 달성

### 성능 측정
- Google PageSpeed Insights: https://pagespeed.web.dev
- GTmetrix: https://gtmetrix.com

## SEO 최적화

- ✅ 메타 태그 설정 (`description`, `og:title` 등)
- ✅ 구조화된 데이터 (Schema.org JSON-LD)
- ✅ 시맨틱 HTML5
- ✅ 접근성 고려

### Google Search Console 등록
1. https://search.google.com/search-console 방문
2. 웹사이트 URL 추가
3. 소유권 확인 (DNS/HTML 태그)

## 접근성

- ✅ 충분한 색상 대비
- ✅ ARIA 레이블
- ✅ 키보드 네비게이션 지원
- ✅ 이미지 alt 텍스트
- ✅ 시맨틱 HTML

## 브라우저 호환성

- Chrome/Chromium ✅
- Firefox ✅
- Safari ✅
- Edge ✅
- Mobile browsers ✅

## 라이선스

개인 포트폴리오 웹사이트입니다.

## 연락처

- **이메일**: min17191601@gmail.com
- **전화**: 010-xxxx-xxxx

---

마지막 업데이트: 2024년
