# 김성민 (Kimseongmin) 👋  
**Full-stack Developer** | 사용자 흐름 중심의 기능 구현 + DB 설계/연동 + 배포/운영까지 한 번에 만드는 걸 좋아합니다.

- ✉️ Email: sungmin3790@gmail.com
- 🌱 관심: 서비스 아키텍처 / 성능 개선 / 협업을 위한 문서화

---

## 🔥 Highlights
- 팀 프로젝트에서 **공통 템플릿(header/footer) 모듈화 + UI 일관성 유지**로 유지보수성 개선
- **DB 모델링(Oracle/MySQL) + API 설계 + 화면 연동**까지 End-to-End 구현 경험
- 실서비스 수준 기능(인증/JWT, 실시간 채팅, 결제, 이미지 업로드, 검색/필터링) 구현 경험

---

## 🧰 Tech Stack
**Backend**
- Spring Boot, Spring MVC, MyBatis
- Node.js (Express), REST API, JWT

**Frontend**
- React (Router/Context/MUI), JSP, Vue3
- HTML/CSS/JS, AJAX

**Database**
- Oracle, MySQL

**Infra & Tools**
- AWS, Git/GitHub
- Socket.io, PortOne(결제), Kakao Maps API, RAWG Games API

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-000?logo=springboot)
![React](https://img.shields.io/badge/React-000?logo=react)
![Node.js](https://img.shields.io/badge/Node.js-000?logo=node.js)
![MySQL](https://img.shields.io/badge/MySQL-000?logo=mysql)
![Oracle](https://img.shields.io/badge/Oracle-000?logo=oracle)
![AWS](https://img.shields.io/badge/AWS-000?logo=amazonaws)

---

## 🚀 Featured Projects

### 1) AGRICOLA (팀 프로젝트) — 농수산물 직거래 이커머스 플랫폼
- **기간**: 2025.10 ~ 2025.11  | **인원**: 4명  
- **한 줄 소개**: 판매자/구매자/관리자 흐름을 갖춘 직거래 커머스 플랫폼 (상품/옵션/이미지/카테고리/결제/관리 기능)
- **Role**
  - 공통 UI 템플릿 분리(header/footer) 및 화면 구성 일관화
  - DB 설계/연동 및 CRUD API 구현(상품/카테고리/이미지/옵션 등)
  - 결제/주소/외부 API 연동(PortOne, Kakao Maps 등)

- **Key Features**
  - 3단 카테고리 트리/드롭다운 UI, 검색/정렬
  - 상품 등록(옵션/이미지 다중 업로드), 썸네일/정렬 처리
  - 관리자 페이지(회원/상품/카테고리 관리)

- **Tech**
  - Spring Boot, JSP, Vue3, jQuery, MyBatis
  - Oracle, PortOne(결제), Kakao Maps API

- **Links**
  - Repo: https://github.com/Kimseongmin3790/Team2_SpringProject.git
  - PPT: https://drive.google.com/file/d/1uDGNjkepO-dKUQeIpOhPxPQ-29l4lkpr/view?usp=drive_link

- **Troubleshooting (요약)**
  - 이미지/옵션/카테고리 연동 시 FK/트랜잭션 정합성 이슈 → **삭제/수정 순서 정리 + 트랜잭션 처리**로 안정화
  - 공통 헤더 드롭다운/레이어 겹침(z-index) 문제 → **레이어 우선순위/hover 영역 구조 개선**으로 해결

---

### 2) GClip (개인 프로젝트) — 게임 하이라이트 공유 SNS
- **기간**: 2025.11 ~ 2025.12  
- **한 줄 소개**: 게임 스크린샷/하이라이트 업로드 + 피드/검색/랭킹 + 실시간 채팅 기능을 갖춘 SNS
- **Role**
  - 기획/설계/개발/배포까지 1인 End-to-End
  - 인증(JWT), 실시간 채팅(Socket.io), 피드/검색/랭킹/프로필 기능 구현

- **Key Features**
  - 피드/게시글 작성(이미지 업로드), 통합 검색(유저/게임/태그)
  - 게임 랭킹/탐색 탭(외부 데이터 RAWG API 활용)
  - 실시간 채팅(Socket.io), 알림/배지(미구현이면 계획으로 표기)

- **Tech**
  - React(React Router/Context/MUI)
  - Node.js(Express), MySQL, Socket.io, JWT
  - RAWG Games API

- **Links**
  - Repo: https://github.com/Kimseongmin3790/React_Project

- **Troubleshooting (요약)**
  - 게시글 삭제 시 태그(FK)로 삭제 실패 → **연관 테이블 선삭제(post_tags 등) + 트랜잭션 처리**로 해결
  - 소켓 연결 오류(connect_error) → **환경변수/서버 주소 분리(.env) + CORS/프록시 점검**으로 안정화

---

## 📌 What I Value
- 기능 구현뿐 아니라 **데이터 정합성 / 예외처리 / 유지보수성**을 같이 챙기는 개발
- 협업을 위한 **문서화(README/회의록/기능정리/ERD)**와 깔끔한 Git 흐름

---

## 🤝 Contact
- Email: sungmin3790@gmail.com
