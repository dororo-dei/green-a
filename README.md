# 🌿 GREEN-A

**HTML, CSS, JavaScript를 활용한 반응형 기업형 웹사이트 제작 프로젝트**

GREEN-A는 웹 퍼블리싱과 JavaScript 기초 학습을 바탕으로 제작한 반응형 웹사이트입니다.

Flexbox를 활용한 레이아웃 구성, 미디어 쿼리를 이용한 반응형 디자인, JavaScript DOM 조작을 통한 모바일 메뉴, Swiper.js를 활용한 상품 슬라이더를 구현했습니다.

## 🛠 기술 스택

| 기술 | 활용 내용 |
|---|---|
| HTML5 | 웹페이지 구조 및 시맨틱 요소 구성 |
| CSS3 | Flexbox, 반응형 레이아웃, 애니메이션 |
| JavaScript (ES6+) | DOM 조작, 이벤트 처리, 클래스 제어 |
| Swiper.js v11 | 반응형 상품 이미지 슬라이더 |

## ✨ 주요 기능

### 1. 반응형 헤더 및 모바일 메뉴

- Flexbox를 활용한 로고와 내비게이션 배치
- `position: sticky`를 이용한 상단 헤더 고정
- 모바일 화면에서 햄버거 메뉴 표시
- JavaScript `classList`를 이용한 사이드 메뉴 열기·닫기
- 메뉴 활성화 시 오버레이 표시 및 본문 스크롤 방지

### 2. 메인 비주얼

- HTML5 `<video>` 태그를 이용한 배경 영상
- `object-fit: cover`를 활용한 영상 크기 조절
- `aspect-ratio`를 이용한 비율 설정
- `clamp()`를 이용한 반응형 텍스트 크기 적용

### 3. 뉴스 카드 리스트

- Flexbox와 `flex-wrap`을 활용한 카드 배치
- `calc()`를 이용한 카드 너비 계산
- 화면 너비에 따른 4열 → 2열 → 1열 구성
- `aspect-ratio`를 활용한 이미지 영역 비율 유지
- `text-overflow`와 `-webkit-line-clamp`를 활용한 텍스트 말줄임

### 4. 상품 슬라이더

Swiper.js 라이브러리를 활용한 반응형 상품 슬라이더입니다.

- 무한 반복 슬라이드 (`loop`)
- 화면 크기에 따른 슬라이드 개수 변경
- 이전·다음 버튼
- 페이지네이션
- Swiper 기본 UI 스타일 커스터마이징

## 📱 반응형 디자인

CSS 미디어 쿼리와 Swiper의 `breakpoints` 옵션을 사용하여 화면 크기에 맞는 레이아웃을 구성했습니다.

| 화면 너비 | 주요 변화 |
|---|---|
| 900px 이하 | 내비게이션 글자 크기 축소 |
| 768px 이하 | 모바일 메뉴 전환, 뉴스 카드 2열 |
| 390px 이하 | 뉴스 카드 1열, 상품 슬라이더 화살표 숨김 |

Swiper 슬라이더는 별도의 반응형 기준을 적용했습니다.

| 화면 너비 | 표시 슬라이드 수 |
|---|---|
| 390px 미만 | 1.3개 |
| 390px 이상 | 2.3개 |
| 768px 이상 | 3.3개 |

## 📁 프로젝트 구조

```text
GREEN-A/
├── index.html
├── css/
│   ├── main.css
│   ├── header.css
│   ├── visual.css
│   ├── news.css
│   ├── product.css
│   ├── footer.css
│   └── responsive.css
├── js/
│   ├── main.js
│   └── swiper_pro.js
└── images/
    ├── visual.mp4
    ├── news1.jpg
    ├── news2.jpg
    ├── news3.jpg
    ├── news4.jpg
    └── ...
```

## 🚀 실행 방법

1. 프로젝트 파일을 다운로드하거나 Git 저장소를 클론합니다.
2. 프로젝트 폴더의 `index.html`을 브라우저에서 실행합니다.
3. VS Code의 Live Server 확장 기능을 사용해 실행할 수도 있습니다.

Swiper.js는 CDN 방식으로 연결되어 있으므로 해당 리소스를 불러오려면 인터넷 연결이 필요합니다.

## 📖 학습 및 구현 내용

이번 프로젝트를 통해 다음 개념을 학습하고 코드에 적용했습니다.

- **HTML 구조 설계:** 공통 컨테이너와 섹션별 콘텐츠 구성
- **CSS 레이아웃:** Flexbox, `position`, `calc()` 활용
- **반응형 디자인:** 미디어 쿼리와 `clamp()` 활용
- **DOM 조작:** `querySelector()`, `classList.add()`, `classList.remove()`
- **이벤트 처리:** `addEventListener()`를 이용한 사용자 인터랙션
- **외부 라이브러리:** Swiper.js 설정 및 커스터마이징

## 🔧 개선 예정 사항

- 모바일 메뉴의 접근성 및 키보드 조작 개선
- 모바일 메뉴 슬라이드 애니메이션 개선
- CSS 파일 로딩 순서 및 중복 스타일 정리
- 이미지 대체 텍스트 개선
- 반응형 레이아웃 및 브라우저별 동작 검증

## 📌 프로젝트 정보

- **프로젝트명:** GREEN-A
- **프로젝트 유형:** 반응형 웹 퍼블리싱 학습
- **제작 시기:** 2026년 10월
- **개발 환경:** Visual Studio Code
- **주요 기술:** HTML5, CSS3, JavaScript, Swiper.js
