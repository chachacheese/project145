# 📚 Project145 – 5인 팀 최종 프로젝트 (2021 · 아카이브용)

본 프로젝트는 2021년 진행된 5인 팀 최종 프로젝트로,
Java 기반 Spring MVC 구조를 활용하여 

로그인, 게시판, 결제, 수강신청,
금융 오픈 API를 활용한 적립금 충전/인출 기능 등 다양한 서비스 기능을 구현하는 데 목적이 있었습니다.

2026년 현재 기준으로 코드를 다시 보관(Archive)하고자 GitHub에 업로드한 프로젝트이며,  
당시 구현 수준 그대로 보존되어 있습니다.

---
## 🛠 Tech Stack

### Backend
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![Servlet](https://img.shields.io/badge/Servlet-6DB33F?style=for-the-badge)
![JSP](https://img.shields.io/badge/JSP-007396?style=for-the-badge&logo=java&logoColor=white)
![MVC](https://img.shields.io/badge/MVC-000000?style=for-the-badge)

### Database
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)

### Tools & Build
![Eclipse](https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipse&logoColor=white)
![Tomcat](https://img.shields.io/badge/Apache_Tomcat-F8DC75?style=for-the-badge&logo=apachetomcat&logoColor=black)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

### Frontend
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JS-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)

---

## 🙋‍♀️ My Contributions (내가 직접 구현한 기능)

문서와 코드 기반으로 확인된 제가 구현한 기능은 아래와 같습니다.

### 🔹 1. 메인 화면 전체 UI 구성
- 서비스 초기 진입 페이지 전체 구현
- 주요 메뉴, 배너, 레이아웃 구성
- 사용자 경험 중심 메뉴 동선 설계

### 🔹 2. 로그인 기능
- ID/비밀번호 기반 기본 로그인 처리
- 세션 기반 로그인 유지 및 권한 체크
- 로그인/로그아웃 흐름 구현

### 🔹 3. 네이버 간편 로그인(OAuth)
- 네이버 OAuth 2.0 인증 연동
- Authorization Code → Access Token 발급 로직 구현
- 사용자 프로필 정보 수신 및 자동 회원 처리
- 콜백 URL 및 리다이렉트 흐름 구현

### 🔹 4. 네이버 검색 API 연동
- 네이버 검색 API 호출 기능 구현
- 검색 키워드 기반 데이터 조회 처리
- JSON 파싱 및 화면 표출

### 🔹 5. 레시피 목록 페이지 구성
- 레시피 데이터 목록 조회 UI 구현
- 페이징 처리 일부 포함
- 검색/필터링 흐름 기반 페이지 구성

### 🔹 6. 레시피 CRUD 기능
- 레시피 작성(Create)
- 레시피 조회(Read)
- 레시피 수정(Update)
- 레시피 삭제(Delete)
- DAO–Service–Controller 계층 구조로 구현

### 🔹 7. 댓글(Comment) 기능
- 댓글 작성/삭제 기능 구현
- 비동기 댓글 반영(AJAX 활용)
- 게시글 상세 페이지와 연동

---

## 📝 Summary
위 기능들은 사용자 인증, 외부 API 호출, CRUD, 비동기 UI 등  
웹 서비스 개발의 핵심 요소로 구성되어 있으며,  
당시 전체 기능 흐름 설계와 실제 구현을 직접 담당했습니다.

---

## 🛠 사용 기술

- **Java 8**
- **JSP / Servlet**
- **MVC 아키텍처 (Controller / Service / DAO / DTO)**
- **ORACLE**
- **Eclipse**
- **Tomcat 8**
- **jQuery / AJAX**
- **Naver OAuth API**

---

## 📁 프로젝트 구조 (요약)
```
Project145/
├── pom.xml
├── src/
│   ├── main/java/
│   │    ├── connect/           # DB 연결
│   │    ├── controller/        # 각 기능별 컨트롤러
│   │    ├── dao/               # DB 접근
│   │    ├── dto/               # 데이터 전달용 VO/DTO
│   │    ├── service/           # 비즈니스 로직
│   │    └── view/              # 콘솔 기반 출력 (일부)
│   ├── main/resources/         # (비어 있음)
│   └── test/                   # (비어 있음)
└── README.md
```
---

## 🔍 기능 요약

- 회원 가입/로그인/로그아웃
- 네이버 간편 로그인(OAuth)
- 게시판 CRUD (작성/조회/수정/삭제)
- 좋아요(Like) 기능
- 게시글 목록 페이징 처리
- 수강 정보 / 결제 / 정산 기능(일부)
- 레시피 데이터 웹 크롤링 및 저장
- 핀테크(계좌/적립금) 기반 적립·충전·인출 기능
- 스케줄러 기반 챌린지 페이백 기능
---

## ⚙️ 실행 방법 (과거 Eclipse 기준)

1. Eclipse에서 프로젝트 Import → Existing Maven Project 선택  
2. Tomcat 8 서버 추가  
3. ORACLE 연결 정보 수정 (`dbConnection.java`)  
4. 실행 (Run on Server)

※ 현재는 환경 차이로 실행이 어려울 수 있으며,  
본 프로젝트는 **아카이브(기록) 보관 목적**으로 업로드되었습니다.

---

## 📝 프로젝트 상태 (2026 기준) 
- 참고/기록용으로만 보관  
- 5년 전 개발 당시의 코드 스타일과 구조 그대로 보존

---

## 💬 회고 (현재 시점에서)
- 백엔드 기본 구조(MVC) 이해에 큰 도움이 되었던 프로젝트  
- OAuth, 페이징, CRUD 등 실제 개발 흐름을 경험한 팀프로젝트  
- 지금 FastAPI + Tortoise ORM 학습에 큰 밑바탕이 되었음

---

## 📬 Contact

- GitHub: https://github.com/chachacheese  
- Velog: https://velog.io/@jiiiin0  
- Email: oz.data.88@gmail.com
