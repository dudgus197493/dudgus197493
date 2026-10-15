# 김영현

Backend & Generative AI Platform Engineer

[Email](mailto:kyh991023@gmail.com) · [GitHub](https://github.com/dudgus197493)

Java·Spring Boot와 Python·FastAPI를 중심으로 기업용 생성형 AI 플랫폼을 개발해 왔습니다. React 클라이언트부터 도메인 API, LLM 오케스트레이션, PostgreSQL 데이터 계층까지 연결하며 기능 설계·구현·검증과 운영 문제 해결을 수행했습니다.

문제를 한 계층의 오류로 단정하지 않고 사용자 경로, 애플리케이션 코드, DB와 외부 API를 함께 대조합니다. 재현 조건과 지표의 분모를 먼저 정의하고, 변경 범위와 롤백 가능성을 확인한 뒤 E2E 검증으로 마무리합니다.

## Core Competencies

- Spring Boot와 FastAPI 기반 백엔드·AI API 설계 및 개발
- React·TypeScript 클라이언트와 SSE 스트리밍 API 통합
- LLM, RAG, 에이전트, 프롬프트 보안, 가드레일과 컨텍스트 관리
- 사용자·조직·테넌트 접근 제어와 감사 이벤트 설계
- PostgreSQL 데이터 모델링, 쿼리 최적화와 운영 지표 검증
- Docker·AWS Bedrock 기반 실행 환경과 테스트·CI 자동화

## Experience

### 하이아스 | SI 개발 · 대리

2023.03 – 2026.10

기업용 생성형 AI 플랫폼의 웹 클라이언트, 도메인 API, AI API와 데이터 계층 전반을 담당했습니다. 요구사항과 검증 기준을 구체화하고, 기능 개발부터 장애 분석, 배포 전 회귀 검증까지 전체 흐름을 다뤘습니다.

#### 다이닝브랜즈그룹 DinAI AI 플랫폼

React, Spring Boot, FastAPI와 PostgreSQL로 분리된 플랫폼에서 채팅, RAG, 지식베이스, 뉴스 클리핑, 특화 에이전트와 관리자 기능을 설계·구현하고 운영 이슈를 해결했습니다.

- 부서별 일일 비용 한도 검증과 실시간 사용량 UPSERT를 설계하고 단위 테스트를 추가해 테넌트별 예산 통제 기반 구축
- 요청 단위 RAG 활성화와 도메인 지식 도구 필터링, 실행 중 가드레일 전환을 구현해 사용자·요청 조건에 따라 AI 동작을 제어
- 뉴스 수집 API의 검색 문법 오류와 100건 제한을 분리 분석하고 날짜 경계 페이지네이션과 호출 간격을 적용해 동일 조건 단일 수집의 정제 기사 수를 545건에서 645건으로 확대
- Bedrock 요청 제한과 SDK 재시도 중첩을 라이브러리 소스와 실호출로 규명하고, 재시도 정책과 오류 분류를 정비해 실패 시간의 상한을 명확화
- 계정 전환 후 남은 URL과 세션 소유권 검사 비대칭을 서버·클라이언트 양쪽에서 수정하고 교차 계정 쓰기 차단을 브라우저 E2E로 검증
- 비동기 감사 로그의 공유 상태 오염을 이벤트 경계의 상태 복사로 해결하고 자원별 고유 ID 기록을 DB와 E2E로 확인
- 관리자 대화 조회용 부분·함수 인덱스와 성능 시드를 구성하고, 파일 업로드 훅의 검증·상태 책임을 분리해 데이터와 프런트엔드 구조 개선
- 불필요한 런타임 의존성을 제거해 AI API 컨테이너 이미지 약 2–3GB 절감

기술: Java, Spring Boot, Python, FastAPI, React, TypeScript, PostgreSQL, AWS Bedrock, RAG, Docker

#### 대상그룹 AI 플랫폼

React·TypeScript, Spring Boot, Python LLM API와 배치 계층으로 구성된 기업용 AI 플랫폼에서 접근 제어, 감사 추적, 프롬프트 보안과 대화 처리 기능을 개발했습니다.

- 사용자 역할과 회사 범위를 반영한 관리자 리소스 접근 제어를 구현하고 감사 이벤트와 E2E 테스트로 권한 경계 검증
- 대화 생성과 첨부파일 업로드를 포함한 주요 행위의 감사 로그를 설계해 행위자·자원 단위 추적성 확보
- 시스템 지시문 노출 요청을 방어하는 규칙과 검증 시나리오를 추가하고, XML 기반 프롬프트 구조화와 ReAct 루프로 에이전트 처리 흐름 정비
- 모델 입력 한도 초과 시 최신 대화가 누락되는 원인을 분석하고 토큰 예산 안에서 최근 대화를 우선 선택하도록 컨텍스트 구성 로직 개선
- 클라이언트, 도메인 API, LLM API 사이의 인증·세션·오류 전파 문제를 전체 요청 경로에서 재현하고 계층별 수정 범위 검증

기술: Java, Spring Boot, Python, FastAPI, React, TypeScript, PostgreSQL, LLM, RAG, Docker

> 회사 프로젝트는 보안과 계약 범위를 고려해 소스 코드를 공개하지 않으며, 공개 가능한 역할과 기술적 의사결정만 정리했습니다.

## Public Projects

### [TravelCompass](https://github.com/travel-compass/TravelCompass) | 팀 프로젝트

한국관광공사 TourAPI와 KakaoMap API를 활용한 여행 정보·일정 관리 서비스입니다.

- 프로젝트 Git 관리와 공통 유틸리티 구현
- 좌표 기반 관광정보 조회와 외부 API·Oracle 데이터 연동
- 로그인, 이메일 인증, BCrypt 비밀번호 암호화와 비동기 유효성 검사
- 여행 일정 비동기 CRUD, 지도 마커와 로드뷰 기능 개발

기술: Java, Spring, JavaScript, Oracle, TourAPI, KakaoMap API

### [Cubespace](https://github.com/Team-Cubespace/Cubespace) | 팀 프로젝트

웹 애플리케이션 팀 프로젝트로, 저장소 기준 217개 커밋에 기여했습니다.

## Engineering Principles

- 증상과 원인을 분리하고 코드·DB·로그·사용자 경로로 가설을 검증합니다.
- 수치가 무엇을 세는지, 제외 조건과 분모가 무엇인지 먼저 정의합니다.
- 단위 테스트만으로 끝내지 않고 실제 사용자 흐름과 계층 간 계약을 확인합니다.
- 타인의 변경을 보존하고 되돌릴 수 있는 작은 범위로 배포·롤백을 설계합니다.

## Technology

- Backend: Java, Spring Boot, Python, FastAPI
- AI: LLM, RAG, LangChain, LangGraph, AWS Bedrock
- Frontend: React, TypeScript, JavaScript
- Data: PostgreSQL, Oracle, MySQL
- Infrastructure: Docker, AWS, GitHub Actions

## Education

서일대학교 사회복지학과 졸업
