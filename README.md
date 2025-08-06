# [프론트엔드 개발자] 노혜련
-----------------
## 📑 목록
* [OALive 사이트]
* [창비 사이트]
* [폴인 사이트]
* [한국관광공사 사이트]
-----------------
## ⭐ 공연 OTT 플랫폼 서비스 - OALive
[OALive](https://zoejoyaws.com/)

### 🗨️ 소개

방구석에서 VIP석 시야로 공연을 관람할 수 있도록 하는 OTT 플랫폼 서비스입니다. 개인 프로젝트로 진행했으며 프론트엔드와 백엔드 개발을 했습니다.


### 🗓️ 기간

2025.05.27. ~ 2025.07.30.


### 👥 인원

1명


### 💡 개발 내용

프론트엔드

* **Next.js 프레임워크**를 기반으로 페이지를 **클라이언트 사이드 렌더링(CSR)** 방식으로 구현
* **React Query**를 사용하여 쿼리 캐싱 및 상태 관리
* 전역 상태 관리는 **Zustand** 사용, 일부 UI 영역은 **Context API Provider**를 통해 분리 관리
* `Swiper slider` 라이브러리를 활용하여 배너 및 이미지 전환 효과 구현
* **아이콘 폰트**를 활용해 인터페이스의 시각적 완성도 향상
* **페이지네이션**을 구현하여 각 카테고리마다 totalPage를 다시 계산할 수 있도록 구현
* 모든 화면 **다크모드** 설정 구현


백엔드

* **Express 프레임워크**
* 환경변수를 별도로 관리하는 **dotenv 모듈** 사용
* 개발 단계에서는 **nodemon**을 적용하여 코드 수정 시 자동으로 서버 재시작되도록 구성하여 생산성 향상
* HTTP 요청에 대한 상세 로그를 **morgan**으로 출력하여 디버깅과 모니터링 효율화
* **CORS** 설정을 통해 프론트엔드와 백엔드 간의 도메인 간 요청을 안전하게 허용
*  Node.js의 **mysql 모듈**을 사용해서 직접 **SQL 쿼리**를 실행해 검색/정렬 기능 구현


DB

* **MySQL**과 **Workbench**를 활용하여 정규화로 데이터 중복을 최소화하고 무결성 확보
* **CRUD** 기능을 구현하여 모듈화된 컴포넌트로 구성하여 유지보수성과 확장성 확보


Open AI 챗봇

* **Python** 기반 **FastAPI 프레임워크**를 활용하여 비동기 처리가 빠른 경량 웹 서버를 구성
* **OpenAI의 대화형 API**를 이용해 사용자 요청에 대해 자연어로 응답하는 챗봇 기능 개발
* AI 모델로는 **gpt4-mini**를 선택하여 경량화된 모델로 빠른 응답 처리 및 클라우드 환경에서의 리소스 부담 최소화


CI/CD 및 배포 환경 구성

* 프로젝트별 **GitHub 레포지토리**를 통합 관리
* 프론트엔드는 **Vercel 클라우드** 플랫폼에 자동 배포되도록 구성하여 개발 및 배포 프로세스를 간소화
* Express 기반 백엔드는 **Docker 환경**에서 애플리케이션을 컨테이너화하고 **GitHub Actions를 통해 AWS EC2 인스턴스**에 자동 빌드 및 배포 파이프라인 구성
* 데이터베이스는 **AWS RDS**를 사용하여 클라우드 기반의 저장소를 구성하고 **MySQL Workbench SSH 터널링**을 통해 보안적으로 접근 및 운영
* Python 기반 FastAPI 서버 또한 **Docker** 기반으로 컨테이너화하고 **GitHub Actions**를 활용하여 기존 **EC2 서버**에 서비스 모듈을 추가하는 방식으로 CI/CD 파이프라인 자동화


### 🌀 이슈

* 아이콘 폰트 사용하는데 유니코드를 못읽는 문제 => css에 !important로 넣어서 **우선순위 조정**으로 해결
* 메인 데이터 가져오는데 vod와 oaset 각각 있는 데이터를 한꺼번에 같이 보여줘야하는 문제 => **view 가상테이블**로 묶어서 불러오기
* 검색페이지 검색 수가 같아야하는데 카테고리 선택할때마다 달라지는 문제 => 처음 들어오는 값 **저장해서 렌더링 되지 않도록** 저장


### ⚙️ 사용기술

* Frontend: `Javascript`, `CSS`, `tailwind CSS`
* Backend:
  * Framework: `Express`
  * Database: `MySQL`
  * AWS: `EC2`, `S3`, `RDS`
  * CI/CD: `GithubAction`, CodeDeploy


### 🔗 Github 링크
* [OALive - 프론트엔드](https://github.com/Zoeryeon/OA-frotend.git)
* [OALive - 백엔드](https://github.com/Zoeryeon/OA-backend.git)
* [OALive - 챗봇](https://github.com/Zoeryeon/OA-chatbot.git)


-----------------
## ⭐ 도서구매 및 참고자료 제공 서비스 - 창비

### 🗨️ 소개

문학 출판사로 책 구매와 관련 자료를 제공하는 서비스입니다. 개인 프로젝트로 진행했으며 프론트엔드와 데이터는 mock서버를 활용하여 개발을 했습니다.


### 🗓️ 기간

2025.05.02. ~ 2025.05.26.


### 👥 인원

1명


### 💡 개발 내용

프론트엔드
* 메인페이지 중심으로 13개 서브페이지 구성
* 반응형 웹앱으로 UI/UX 최적화 대응

데이터
* mock 데이터를 활용한 가짜 서버 연동 및 데이터 흐름(ID 기반) 구축
* 데이터별 필터 로직 처리 서버 구현이 핵심

### 🌀 이슈

* 이미지가 기본적으로 위로 맞춤이 되어있는데 align-items를 넣어도 아래맞춤이 안되는 문제 => img에 vertical-align:baseline 속성 추가
* 서브 메뉴를 누르는데 전체가 밑으로 내려가고 옆 공간이 너무 많이 나오는 문제 => 옆으로 이동하는걸 이중으로 넣어놨었음, 풀어주고 header이 아니라 gnb에서 늘리는걸로 바꿔서 해결
* category 주소가 제대로 바뀌지 않는 문제 => setCate가 조건 밖에 있었는데 안으로 넣어줘서 해결
* 검색버튼 누르면 페이지 이동해야하는데 하지 않는 문제 => form 이랑 onClick 이벤트를 이중으로 걸어놨음, button에 onClick을 form에 onSubmit으로 옮겨주며 해결


### ⚙️ 사용기술

* Frontend: `TypeScript`, `Tailwind CSS`, `Swiper`
* Backend:
  * Framework: `Express`, `CORS`, `Node.js`, `Next.js 15`, `React 19`, `Vite`
  * CI/CD: `GithubAction`, `Vercel`
  * Data: `TanStack React Query`, `RESTful 구조 기반 외부 데이터 연동`


### 🔗 Github 링크
* [창비](https://github.com/Zoeryeon/Changbi.git)


-----------------
## ⭐ 전문가들의 경험 공유 서비스스 - 폴인 fol:in

### 🗨️ 소개

변화의 앞단에서 빠르게 성장하는 이들의 경험을 공유하는 콘텐츠 서비스입니다. 개인 프로젝트로 진행했으며 프론트엔드와 데이터는 mock서버를 활용하여 개발을 했습니다.


### 🗓️ 기간

2025.04.04. ~ 2025.04.24.


### 👥 인원

3명


### 💡 개발 내용

프론트엔드
* 세미나 메인/상세 페이지 포함 총 5개 서브 UI 화면 구현
* 필터 상태 기반 조건부 렌더링 및 버튼 텍스트/스타일 동적 전환 로직 구현
* 로그인 페이지 UI 구현 및 비밀번호 보기/숨기기 상태 핸들링 기능 적용
* 다양한 해상도 테스트를 통해 반응형 디자인 최적화 및 시각적 정돈성 반영

데이터
* 세미나 데이터 흐름 설계 및 filterState, onClickHandler 중심 상태 제어 기능 구현
* 팀원 간 병렬 작업을 고려한 일정 조율 및 비동기 데이터 대응 로직 구축


### 🌀 이슈

* handler에서는 데이터가 나오는데 article에서는 나오지 않는 문제 => 연결이 잘못 되어서 다시 연결해서 해결
* linker가 두명일때 데이터를 못가져오는 문제 => 그냥 적지 않고 배열로 바꿔서 해결


### ⚙️ 사용기술

* Frontend: `TypeScript`, `Tailwind CSS`, `Swiper`
* Backend:
  * Framework: `Express`, `CORS`, `Node.js`, `React Router`, `React 19`, `Vite`, `Ubuntu(Local)`
  * CI/CD: `GithubAction`, `Vercel`
  * Data: `TanStack React Query`, `RESTful 구조 기반 외부 데이터 연동`


### 🔗 Github 링크
* [폴인 fol:in](https://github.com/Zoeryeon/folin.git)

