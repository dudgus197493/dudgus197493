# 김영현

Backend & Generative AI Platform Engineer

Java·Spring Boot와 Python·FastAPI를 중심으로 생성형 AI 플랫폼을 개발합니다.

웹 클라이언트, 도메인 API, LLM 오케스트레이션과 데이터 계층을 연결하고 비용 통제, 접근 제어, 감사 로그와 회귀 검증을 통해 운영 가능한 서비스로 만드는 일을 해왔습니다.

## Core Competencies

- Spring Boot와 FastAPI를 활용한 백엔드 및 AI API 개발
- React와 TypeScript를 포함한 생성형 AI 서비스 통합
- LLM, RAG, 평가, 가드레일 및 서비스 모니터링
- PostgreSQL과 Oracle 기반 데이터 모델링 및 연동
- Docker와 AWS 기반 개발·운영 환경 구성

## Selected Professional Work

### DinAI

다이닝브랜즈그룹의 생성형 AI 플랫폼 프로젝트입니다. React, Spring Boot, FastAPI와 PostgreSQL 전 계층에서 기능을 개발했습니다.

- 부서별 사용 한도와 실시간 비용 집계, 요청별 RAG 제어 및 가드레일 처리
- SSE 스트리밍, 대화·첨부파일 수명주기와 관리자 감사·조회 기능
- 문서 파싱 엣지 케이스와 URL 중복 제거 회귀 테스트
- 조회 인덱스와 성능 검증 데이터, 컨테이너 의존성 최적화

### 대상그룹 AI 플랫폼

React·TypeScript, Spring Boot와 Python LLM API로 구성된 기업용 AI 플랫폼을 개발했습니다.

- 사용자 역할과 회사 범위에 따른 관리자 데이터 접근 제어
- 도메인 감사 로그와 E2E 테스트, 민감 정보 처리 경계 구현
- 시스템 프롬프트 노출 방어와 토큰 한도 기반 대화 컨텍스트 처리

### 생성형 AI 챗봇

React 클라이언트, Spring Boot 코어 API, Python AI API와 PostgreSQL로 구성된 생성형 AI 챗봇 V1·V2를 개발했습니다.

- SSE 프록시 실행기와 오류 처리, 사용자·클라이언트 추적 정보 전달
- 파일 업로드 상태와 대화 상태의 책임 분리, 첨부파일 수명주기 보강
- 세션 소유권 검사와 요청별 RAG 제어

## Featured Projects

### [AI Quality Lab](https://github.com/dudgus197493/ai-quality-lab)

LLM 애플리케이션의 출력과 실행 추적을 외부 모델 없이 검사하는 결정형 회귀 품질 게이트입니다.

- 프롬프트 노출, 도구 호출 순서와 RAG 근거 포함 여부 평가
- JSONL 데이터셋과 케이스별 판정 이유를 포함한 JSON 리포트
- 기준 리포트에서 성공했던 항목의 실패를 별도 회귀로 탐지
- 최소 통과율 또는 회귀 발생 시 CI 실패 처리

### [Document Ops Lab](https://github.com/dudgus197493/document-ops-lab)

문서 정규화부터 중복 제거, 실패 재처리와 운영 리포트까지 연결한 로컬 처리 파이프라인입니다.

- 여러 페이지에서 반복되는 머리글·바닥글 제거와 텍스트 정규화
- SHA-256 콘텐츠 해시로 소스 경로가 다른 중복 문서 식별
- SQLite에 소스별 상태·시도 횟수·오류와 고유 산출물 분리 저장
- 실패 작업 선택적 재실행과 처리 현황 Markdown 리포트 생성

### [TravelCompass](https://github.com/travel-compass/TravelCompass)

한국관광공사와 KakaoMap API를 활용한 여행 정보 및 일정 관리 서비스입니다.

- 좌표 기반 관광정보 조회와 외부 API·Oracle 데이터 연동
- 로그인, 이메일 인증, 비밀번호 암호화 및 비동기 유효성 검사
- 여행 일정 CRUD와 지도·로드뷰 기능
- 공통 유틸리티 구현과 Git 협업 관리

### [Cubespace](https://github.com/Team-Cubespace/Cubespace)

팀 기반 웹 애플리케이션 프로젝트로, 저장소 기준 217개 커밋에 참여했습니다.

## Technology

- Backend: Java, Spring Boot, Python, FastAPI
- AI: LLM, RAG, LangChain, LangGraph, AWS Bedrock
- Frontend: React, TypeScript, JavaScript
- Data: PostgreSQL, Oracle, MySQL
- Infrastructure: Docker, AWS, GitHub Actions

## Contact

- Email: [kyh991023@gmail.com](mailto:kyh991023@gmail.com)
- GitHub: [github.com/dudgus197493](https://github.com/dudgus197493)
