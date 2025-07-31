# [프론트엔드 개발자] 노혜련
## ⭐ 공연 OTT 플랫폼 서비스 - OALive
**`[ 소개 ]`**

방구석에서 VIP석 공연을 관람할 수 있도록 하는 OTT 플랫폼 서비스입니다. 개인 프로젝트로 진행했으며 프론트엔드와 백엔드 개발을 했습니다.


**`[ 기간 ]`**

2025.05.27. ~ 2025.07.30.


**`[ 인원 ]`**

1명


**`[ 개발 내용 ]`**

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


**`[ 이슈 ]`**

* 아이콘 폰트 사용하는데 유니코드를 못읽는 문제 => css에 !important로 넣어서 **우선순위 조정**으로 해결
* 메인 데이터 가져오는데 vod와 oaset 각각 있는 데이터를 한꺼번에 같이 보여줘야하는 문제 => **view 가상테이블**로 묶어서 불러오기
* 검색페이지 검색 수가 같아야하는데 카테고리 선택할때마다 달라지는 문제 => 처음 들어오는 값 **저장해서 렌더링 되지 않도록** 저장


**`[ 사용기술 ]`**

* Frontend: `Javascript`, `CSS`, `tailwind CSS`
* Backend:
  * Framework: `Express`
  * Database: `MySQL`
  * AWS: `EC2`, `S3`, `RDS`
  * CI/CD: `GithubAction`, CodeDeploy


**`[ Github 링크 ]`**
* [OALive - 프론트엔드](https://github.com/Zoeryeon/OA-frotend.git)
* [OALive - 백엔드](https://github.com/Zoeryeon/OA-backend.git)
* [OALive - 챗봇](https://github.com/Zoeryeon/OA-chatbot.git)




