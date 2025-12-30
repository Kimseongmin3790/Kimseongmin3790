# 김성민 (Kimseongmin) 👋
**Full-stack Developer**  
사용자 흐름을 기준으로 기능을 설계하고, **DB 설계/연동 → API → 화면 구현**까지 End-to-End로 완성하는 것을 좋아합니다.

[![Email](https://img.shields.io/badge/Email-sungmin3790%40gmail.com-000?logo=gmail)](mailto:sungmin3790@gmail.com)
[![AGRICOLA Repo](https://img.shields.io/badge/Repo-AGRICOLA-000?logo=github)](https://github.com/Kimseongmin3790/Team2_SpringProject.git)
[![GClip Repo](https://img.shields.io/badge/Repo-GClip-000?logo=github)](https://github.com/Kimseongmin3790/React_Project)
[![PPT](https://img.shields.io/badge/PPT-AGRICOLA-000?logo=googledrive)](https://drive.google.com/file/d/1uDGNjkepO-dKUQeIpOhPxPQ-29l4lkpr/view?usp=drive_link)

---

## 🔥 Highlights
- **공통 UI(header/footer) 모듈화**로 페이지 간 UI 일관성 확보 및 유지보수 비용 절감 (외부 CSS/JS 분리)
- **DB 모델링(Oracle/MySQL) + API 설계 + 화면 연동**까지 End-to-End 구현 경험
- 실서비스 핵심 기능 **인증(JWT), 실시간 채팅(Socket.io), 결제(PortOne), 이미지 업로드, 검색/필터링** 구현 경험

---

## 🧰 Tech Stack
**Backend**: Spring Boot · Spring MVC · MyBatis / Node.js(Express) · REST API · JWT  
**Frontend**: React(Router/Context/MUI) · JSP · Vue3 · HTML/CSS/JS · AJAX  
**Database**: Oracle · MySQL  
**Tools & APIs**: AWS · Git/GitHub · Socket.io · PortOne · Kakao Maps API · RAWG Games API

---

# 🚀 Featured Projects

---

## 1) AGRICOLA (팀 프로젝트) — 농수산물 직거래 이커머스 플랫폼
**기간**: 2025.10 ~ 2025.11 | **인원**: 4명  
**Repo**: https://github.com/Kimseongmin3790/Team2_SpringProject.git  
**PPT**: https://drive.google.com/file/d/1uDGNjkepO-dKUQeIpOhPxPQ-29l4lkpr/view?usp=drive_link

> ✅ 스크린샷(예시): 회원가입 / 관리자 화면
![AGRICOLA 회원가입](./assets/agricola_signup.png)
![AGRICOLA 관리자](./assets/agricola_admin.png)

### 🔎 한 줄 소개
판매자/구매자/관리자 흐름을 갖춘 **직거래 커머스 플랫폼** (상품/옵션/이미지/카테고리/결제/관리자)

### 🙋 내가 맡은 핵심 기능 (구체)
- **공통 UI 템플릿 구축**
  - 모든 페이지에 공통 적용되는 `header.jsp / footer.jsp` 분리
  - 외부 `header.css / footer.css`로 스타일 표준화, 네비게이션/아이콘/드롭다운 구조 정리
- **카테고리 UI/동작 구성**
  - 다단(3단) 카테고리 드롭다운 UI 구성 및 hover/레이어(z-index) 이슈 해결
- **DB 연동 기반 CRUD 구현(프로젝트 내 담당 범위)**
  - 화면 입력값 → 컨트롤러/서비스 → MyBatis → Oracle DB까지 연결되는 CRUD 플로우 구현
- **외부 서비스 연동 경험**
  - 결제(PortOne) 연동 플로우 이해 및 검증/처리 로직 구성(프로젝트 내 적용 범위)

### ⭐ Key Features
- 3단 카테고리 트리/드롭다운 UI, 검색/정렬
- 상품 등록(옵션/이미지 다중 업로드), 썸네일/정렬 처리
- 관리자 페이지(회원/상품/카테고리 관리)

### 🧩 Troubleshooting (대표)
- **드롭다운 레이어 겹침/hover 끊김 문제**
  - 원인: 배너/컨텐츠 레이어가 메뉴 위로 올라와 hover 이벤트가 끊김
  - 해결: z-index 우선순위 재정의 + hover 영역 구조 개선 → 메뉴 사용성 안정화
- **연관 데이터(FK) 정합성 이슈**
  - 해결 방향: 삭제/수정 시 “참조 관계 → 선행 삭제 순서”를 명확히 하고 트랜잭션으로 묶어 정합성 유지

---

## 2) GClip (개인 프로젝트) — 게임 하이라이트 공유 SNS
**기간**: 2025.11 ~ 2025.12  
**Repo**: https://github.com/Kimseongmin3790/React_Project

> ✅ 스크린샷(예시): 메인 피드
![GClip 메인 피드](./assets/gclip_feed.png)

### 🔎 한 줄 소개
게임 스크린샷/하이라이트 업로드 + 피드/검색/랭킹 + 실시간 채팅을 갖춘 **게임 SNS**

### 🙋 내가 맡은 핵심 기능 (구체)
- **피드 중심 UI 구성(React + MUI)**
  - 메인 피드 페이지 구성 및 공통 헤더 적용 구조 정리
  - 게시글 작성/이미지 업로드 UI 개선(첨부 미리보기 등)
- **검색/랭킹 데이터 연동**
  - RAWG Games API 호출 파라미터 구성(페이지네이션/정렬/플랫폼 필터 등) 및 화면 출력
  - 검색 결과 페이지 구성 및 라우팅 연계
- **실시간 채팅(Socket.io) 연결 안정화**
  - 소켓 connect_error 이슈 대응: 환경변수(.env) 기반 서버 주소 분리 및 네트워크/CORS 점검
- **데이터 정합성 중심의 삭제 로직 설계**
  - 게시글 삭제 시 FK로 인한 실패 이슈 해결:
  - 연관 테이블(예: post_media, post_tags 등) **선삭제 + 트랜잭션 처리**로 안정적인 삭제 플로우 구성

### ⭐ Key Features
- 피드/게시글 작성(이미지 업로드), 통합 검색(유저/게임/태그)
- 게임 랭킹/탐색(외부 데이터 RAWG API 활용)
- 실시간 채팅(Socket.io), 프로필/마이페이지

### 🧩 Troubleshooting (대표 2건)
- **게시글 삭제 실패(FK)**
  - 원인: 태그/미디어 등 연관 테이블 레코드가 남아 참조 무결성 위반
  - 해결: `연관 테이블 선삭제 → posts 삭제` 순서 적용 + 트랜잭션으로 원자성 보장
- **소켓 연결 오류(connect_error)**
  - 해결: socket 서버 주소를 .env로 분리하고, 실행 환경별 설정/네트워크/CORS를 점검해 연결 안정화

---

## 📌 What I Value
- 기능 구현뿐 아니라 **데이터 정합성 / 예외처리 / 유지보수성**을 같이 챙기는 개발
- 협업을 위한 **문서화(README/기능 정리/ERD)** + 깔끔한 Git 기록(PR/커밋 단위) 지향

---

## 🤝 Contact
- Email: sungmin3790@gmail.com
