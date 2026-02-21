# Maechuri
## 개요
매추리 게임은 "매일 추리 게임"이라는 이름으로 AI로 매일 색 다른 추리 게임을 하는 것을 목표로 합니다.

## 기술 스택
- Frontend: React
- Backend: FastAPI, Kotlin + Webflux + Spring Boot 
- Al Tools: Gemini Cli, Github Copilot

## 주간 진행 상황
### Week 9 (26.02.16 - 26.02.22)
- **작업 내역**: 마인드 펠리스 ui 구현, fact, clue 참조 정상화
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**:마인드 펠리스 UI, 하드 코딩된 Today scenario 수정, DB 마이그레이션 적용, 세션 ID 관리
- **PR 로그**:
    - [마인드 펠리스 UI](https://github.com/Apptive-Game-Team/MaechuriClient/pull/25)
    - [하드 코딩된 Today scenario 수정](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/27)
    - [DB 마이그레이션 적용](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/25)
    - [세션 ID 관리](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/23)
    - [enum 리펙터링](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/56)

### Week 8 (26.02.09 - 26.02.15)
- **작업 내역**: solve api 연결, solve ui 구현, ai server SBERT model 로드 문제 해결
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: solve api 연결, solve ui 구현, ai server SBERT model 로드 문제 해결
- **PR 로그**: Solve UI, Solve API, 관련된 Fact Id 반환, 모델 로드 문제 해결
    - [관련된 Fact Id 반환, 모델 로드 문제 해결](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/54)
    - [Solve UI](https://github.com/Apptive-Game-Team/MaechuriClient/pull/23)
    - [Solve API](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/21)

### Week 7 (26.02.02 - 26.02.08)
- **작업 내역**: AI <-> Main <-> client 연결, 대화에서 fact 뽑아주기
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: AI <-> Main <-> client 연결
- **PR 로그**:
    - [redis](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/49)
    - [data2prompt mapper 모으기 & 버그 고침](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/51)
    - [main <-> ai 대화 연결](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/19)
    - [지난주 수정된 데이터 구조 반영](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/17)

### Week 6 (26.01.26 - 26.02.01)
- **작업 내역**: 발표 준비, 시나리오 데이터 구조 수정 (단순화), map 구체화 로직 구현
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: 발표 준비, 시나리오 데이터 구조 단순화, map 로직 구현
- **PR 로그**:
    - [fact 통합](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/42)
    - [데이터 구조 가지치기](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/47)

### Week 5 (26.01.19 - 26.01.25)
- **작업 내역**: main-server <-> ai-server 소통 기능 구현, 시나리오 생성 상호작용 방식 수정 (비동기 방식으로), 엔딩 판단 로직 고도화
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: game_session 방식 구현, 시나리오 생성 상호작용 방식 수정, 엔딩 판단 로직 고도화
- **PR 로그**:
    - [ai-main 연결](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/15)
    - [rag, game session](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/32)
    - [리펙터링 (일관성1)](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/35)
    - [리펙터링 (일관성2)](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/37)
    - [엔딩 판단](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/38)

### Week 4 (26.01.12 - 26.01.18)
- **작업 내역**: 증거 인벤토리 및 참조(Reference) 시스템 구축, AI 대화 로직 고도화(SBERT 도입), API 호출 제한(Rate Limit) 및 지문(Fingerprint) 인식 구현, 인프라 배포 자동화
- **AI 활용**: SBERT 기반 임베딩 구현을 통한 대화 고도화, 환경변수 중앙 관리 및 CI 파이프라인 최적화
- **완료 기능**: yh.yunseong.dev 서버 환경(Docker) 구축, 2단계 맵 생성 파이프라인, 용의자 단서 생성 로직, 클라이언트 카메라/채팅 UX 개선, 참조 시스템 UI/UX
- **PR 로그**: 
    - [하루 API 양 제한 구현](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/13)
    - [Map 생성 파이프라인 및 고도화](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/18)
    - [용의자 대화 시스템 구현](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/16)
    - [SBERT Embedding 구현](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/22)
    - [레퍼런스 기능 구현 (Client)](https://github.com/Apptive-Game-Team/MaechuriClient/pull/17)
    - [카메라 시스템 및 채팅 UX 개선](https://github.com/Apptive-Game-Team/MaechuriClient/pull/15)
    - [API 호출 커스텀 (Fingerprint/Cache)](https://github.com/Apptive-Game-Team/MaechuriClient/pull/19)
- **다음 주 계획**: 증거 인벤토리 시스템 연동 완료, '시스템 과부화' 및 '자백 모드' 로직 구체화, SBERT를 활용한 RAG 성능 최적화

### Week 3 (26.01.05 - 25.01.11)
- **작업 내역**: 대화 기능 초안, api 구현 (map, interaction), main ci 구현, 전장의 안개 기능 (raycasting), map 데이터 구조 수정, client api 연결
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: map interaction api (server, client), main server ci 구현, 전장의 안개 기능, map 데이터 구조 수정
- **PR 로그**: [대화 기능 초안](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/2), [api 구현](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/8), [docker ci](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/10), [전장의 안개](https://github.com/Apptive-Game-Team/MaechuriClient/pull/8), [맵 데이터 구조 변경](https://github.com/Apptive-Game-Team/MaechuriClient/pull/10), [client api 연결](https://github.com/Apptive-Game-Team/MaechuriClient/pull/12)
- **다음 주 계획**: RAG 구현, suspect 대화 기능 고도화, 게임 엔딩 체크 Tool 구현, Client ref 기능 구현

### Week 2 (25.12.29 - 26.01.04)
- **작업 내역**: jwt 기능 구현, history 디지털 서명 설계, asset 저장 기능 구현, asset 관리 admin 페이지 구현, 시나리오 증거 제작 기능 구현
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, gemini cli를 통한 자료 조사, 코드 생성
- **완료 기능**: jwt 기능, history 서명 기능, asset 저장 기능, asset 관리 페이지, 시나리오 제작 기능, 증거 제작 기능
- **PR 로그**: [jwt 기능, 히스토리 서명](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/4), [asset 저장, 관리](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/6), [시나리오 제작](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/7), [증거 제작](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/9)
- **다음 주 계획**: 상호작용 시스템 통합, AI 대화 엔진 안정화, 시나리오 생성 자동화, 개인화 기능 구체화

### Week 1 (25.12.22 - 12.28)
- **작업 내역**: minio 서버 구축, interface 구현, fast api 초기화, 용의자 생성 기능 구현, react 프로젝트 초기화, 게임 화면 구현, 플레이어 이동 구현, client CICD 배포 구현, asset loading system 구현
- **AI 활용**: Github Copilot을 사용한 issue to pr 생성으로 코드 구현, 이미지 생성으로 asset 생성 
- **완료 기능**: asset loading, client cicd, client player moving, 용의자 생성 기능
- **PR 로그**: [minio 기능 구현](https://github.com/Apptive-Game-Team/MaechuriMainServer/pull/2), [init fast api](https://github.com/Apptive-Game-Team/MaechuriAIServer/pull/2), [client 기능 구현](https://github.com/Apptive-Game-Team/MaechuriClient/pull/2), [CICD](https://github.com/Apptive-Game-Team/MaechuriClient/pull/6), [asset loading](https://github.com/Apptive-Game-Team/MaechuriClient/pull/4)
- **링크**: [게임 링크](https://apptive-game-team.github.io/MaechuriClient/)
- **다음 주 계획**: 인증 및 생태 유지 시스템 구축, 데이터 영속성 및 에셋 관리, 시나리오 생성 엔진 고도화
