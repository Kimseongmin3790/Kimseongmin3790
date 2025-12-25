# 김성민 (Kimseongmin) 👋
**Full-stack Developer**  
사용자 흐름 중심의 기능 구현부터 DB 설계/연동까지 End-to-End로 만드는 것을 지향합니다.

[![Email](https://img.shields.io/badge/Email-sungmin3790%40gmail.com-000?logo=gmail)](mailto:sungmin3790@gmail.com)
[![AGRICOLA Repo](https://img.shields.io/badge/Repo-AGRICOLA-000?logo=github)](https://github.com/Kimseongmin3790/Team2_SpringProject.git)
[![GClip Repo](https://img.shields.io/badge/Repo-GClip-000?logo=github)](https://github.com/Kimseongmin3790/React_Project)
[![PPT](https://img.shields.io/badge/PPT-AGRICOLA-000?logo=googledrive)](https://drive.google.com/file/d/1uDGNjkepO-dKUQeIpOhPxPQ-29l4lkpr/view?usp=drive_link)

---

## 🔥 Highlights (Impact)
- 공통 UI(header/footer) 템플릿 분리로 **페이지 유지보수 비용 감소** 및 UI 일관성 확보 (외부 CSS/JS 구조화)
- Oracle/MySQL 기반 **DB 모델링 + REST API 설계 + 화면 연동**까지 End-to-End 개발 경험
- 인증(JWT), 실시간 채팅(Socket.io), 결제(PortOne), 이미지 업로드, 검색/필터링 등 **서비스 핵심 기능 구현 경험**

---

## 🧰 Tech Stack
**Core**: Spring Boot · MyBatis · React · Node.js(Express) · Oracle/MySQL · AWS  
**Also used**: JSP · Vue3 · Socket.io · PortOne · Kakao Maps API · RAWG Games API · Git/GitHub

---

## 🚀 Featured Projects

| Project | Summary | My Role | Links |
|---|---|---|---|
| **AGRICOLA** (팀, 2025.10~2025.11) | 농수산물 직거래 이커머스 (상품/옵션/이미지/카테고리/결제/관리자) | 공통 UI 템플릿 구조화 · DB 설계/연동 및 CRUD API · 외부 API 연동(결제/지도) | [Repo](https://github.com/Kimseongmin3790/Team2_SpringProject.git) · [PPT](https://drive.google.com/file/d/1uDGNjkepO-dKUQeIpOhPxPQ-29l4lkpr/view?usp=drive_link) |
| **GClip** (개인, 2025.11~2025.12) | 게임 하이라이트 공유 SNS (피드/검색/랭킹/실시간 채팅) | 1인 기획~개발 · JWT 인증 · Socket.io 채팅 · RAWG API 연동 | [Repo](https://github.com/Kimseongmin3790/React_Project) |

---

## 🧩 Troubleshooting (대표 2건)
### 1) FK로 인해 게시글 삭제 실패 (GClip)
- **문제:** 게시글 삭제 시 tags/post_tags FK로 인해 삭제 실패  
- **원인:** 연관 테이블 레코드가 남아 있어 참조 무결성 위반  
- **해결:** `post_tags → post_media → posts` 순서로 **선삭제 + 트랜잭션** 적용해 정합성 보장  
- **배운점:** “삭제/수정”은 항상 **참조 방향과 트랜잭션 경계**를 먼저 설계해야 안정적

### 2) 공통 헤더 드롭다운 레이어 겹침 (AGRICOLA)
- **문제:** 배너/버튼 요소가 dropdown 위로 올라와 hover가 끊김  
- **해결:** z-index 우선순위 재정의 + hover 영역 구조 개선으로 UI 안정화  
- **배운점:** 복잡한 UI는 **레이어/이벤트 영역 설계**가 기능만큼 중요

---

## 📌 What I Value
- 데이터 정합성 / 예외처리 / 유지보수성을 함께 고려하는 개발
- 협업을 위한 문서화(README/기능정리/ERD)와 깔끔한 Git 흐름

---

## 🤝 Contact
- Email: sungmin3790@gmail.com
