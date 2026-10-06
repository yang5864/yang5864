<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg?v=20261007">
  <img src="./assets/banner-light.svg?v=20261007" alt="yang5864 — 사용자의 문제를 서비스와 AI 자동화로 해결하는 백엔드 개발자" width="100%">
</picture>

<p align="center">
  <a href="#about-me">About Me</a> ·
  <a href="#tech-stack">Tech Stack</a> ·
  <a href="#selected-projects">Projects</a> ·
  <a href="#activities--writing">Activities</a> ·
  <a href="#awards--recognition">Awards</a>
</p>

<div align="center">

## About Me

**사용자의 문제를 서비스와 AI 자동화로 해결하는 백엔드 개발자 양승환입니다.**

<p>Java·Spring 기반 로직부터 AI 연동, 성능 개선, 배포까지 구현합니다.<br>직접 운영하는 블로그와 알고리즘 스터디에서 문제를 발견하고,<br>사용자가 실제로 쓸 수 있는 서비스로 만드는 과정을 좋아합니다.</p>

<a href="https://blog.naver.com/shy_fr00"><img src="https://img.shields.io/badge/Blog-시나브로_기록하기-03C75A?style=flat-square&amp;logo=naver&amp;logoColor=white" alt="시나브로 기록하기 블로그"></a> <a href="https://github.com/yang5864?tab=repositories"><img src="https://img.shields.io/badge/GitHub-Projects-24292F?style=flat-square&amp;logo=github&amp;logoColor=white" alt="GitHub 프로젝트"></a>

</div>

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&amp;logo=openjdk&amp;logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&amp;logo=spring&amp;logoColor=white" alt="Spring">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&amp;logo=python&amp;logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&amp;logo=fastapi&amp;logoColor=white" alt="FastAPI">
  <br>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&amp;logo=mysql&amp;logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&amp;logo=postgresql&amp;logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&amp;logo=redis&amp;logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&amp;logo=supabase&amp;logoColor=102A23" alt="Supabase">
  <br>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&amp;logo=docker&amp;logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&amp;logo=amazonwebservices&amp;logoColor=white" alt="AWS">
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&amp;logo=githubactions&amp;logoColor=white" alt="GitHub Actions">
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&amp;logo=tensorflow&amp;logoColor=white" alt="TensorFlow">
  <br>
  <img src="https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&amp;logo=vuedotjs&amp;logoColor=white" alt="Vue 3">
  <img src="https://img.shields.io/badge/Next.js-24292F?style=flat-square&amp;logo=nextdotjs&amp;logoColor=white" alt="Next.js">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&amp;logo=typescript&amp;logoColor=white" alt="TypeScript">
</p>

| Area | Experience |
| :--- | :--- |
| Backend & Data | Spring MVC·Spring Boot, MyBatis·JPA, SQL, 트랜잭션, Redis Streams·Outbox |
| AI & Automation | LLM API 연동, TensorFlow·GRU, 시계열 전처리, Selenium·CDP, Slack API |
| Deployment & Quality | AWS EC2·ECR·SSM, Docker Compose, GitHub Actions·OIDC, k6, Prometheus·Grafana, pytest |
| Frontend | Vue 3·Pinia, Next.js·TypeScript, 모바일 입력 흐름과 코드 제출 화면 |

## Selected Projects

### 01 / Jaedaero

**제대로 — 군 장병의 전역 자산을 예측하는 AI 자산관리 서비스**<br>2026.07–2026.08 · 6인 팀 · 백엔드·AI·성능 개선·배포

확정 소득과 금융 데이터를 바탕으로 자산 시뮬레이션과 AI 코칭을 제공합니다.

- 금융 계산은 Spring 로직이 책임지고, LLM은 계산 결과를 설명하도록 역할을 분리했습니다.
- MySQL Outbox → Redis Streams → FCM으로 업무 트랜잭션과 외부 알림 실패를 분리했습니다.
- k6로 랭킹 조회 병목을 재현해 캐시와 변경 시 무효화를 적용하고, OIDC·ECR·SSM으로 AWS 배포를 자동화했습니다.

> 챌린지 랭킹 조회 p95 **12.77초 → 22.87ms**. 외부 CODEF 연동을 제외한 **로컬 Docker 환경·k6 100 VU** 측정 결과입니다.

[프로젝트 소개](https://github.com/BellongBellong) · [백엔드 코드](https://github.com/BellongBellong/Jaedaero_backend) · [부하 테스트 구성](https://github.com/BellongBellong/Jaedaero_backend/tree/dev/k6)

### 02 / Pacto

**Pacto — 크리에이터 협업 이력과 조건부 정산을 연결하는 플랫폼**<br>2026.04 시작 · 4인 팀 · 팀장·백엔드

중소 마케팅 대행사가 캠페인·증빙·정산 이력을 축적하고, 검증된 크리에이터와 다시 협업할 수 있도록 만드는 서비스입니다.

- 캠페인 신청 수락·에스크로 생성·미션 생성을 하나의 트랜잭션으로 묶고, 실패 시 전체를 롤백하도록 구현했습니다.
- 에스크로 캠페인 MVP를 구현·배포한 뒤, 반복 협업 이력이 쌓이는 Creator Operations CRM으로 제품 범위를 구체화했습니다.

[프로젝트 소개](https://github.com/Pacto-Developers) · [백엔드 코드](https://github.com/Pacto-Developers/Pacto-backend)

### 03 / BlogLife

**BlogLife — 블로그 운영의 반복 작업을 줄이는 데스크톱 앱**<br>2025.12 시작 · 개인 기획·개발·실사용자 운영

블로그를 직접 운영하며 발견한 반복 작업을 Python·Selenium·Gemini로 자동화했습니다.

- Supabase Auth 기반 요금제·구독 만료일 관리와 기기 라이선싱을 구현했습니다.
- AI 생성 누락 건을 추적해 재생성하고, 제출 결과를 상태로 판정하도록 구성했습니다.
- 백그라운드 워커로 UI 멈춤을 개선하고, pytest로 상태 판정과 외부 API 의존성을 검증했습니다.

### 04 / YOJ

**YOJ — 스터디의 문제 풀이·코드 제출·채점을 한곳에 모은 온라인 저지**<br>2026.04 시작 · 개인 기획·개발·스터디 실사용

Next.js·Supabase와 AWS EC2의 Judge0을 연결해 풀이부터 제출 이력까지 이어지는 학습 환경을 만들었습니다.

- 공개된 문제 조건을 바탕으로 자체 테스트 케이스를 작성하고, 배치 채점과 진행 상태 전달을 구현했습니다.
- 사용자 승인·사용량 제한을 적용하고, 채점 서버의 디스크 부족 장애를 복구했습니다.
- 서버 장애와 사용자 코드 오류를 구분해 결과를 안내하도록 개선했습니다.

## More Projects

| Project | My Contribution | Links |
| :--- | :--- | :--- |
| BitOracle | GRU 시계열 모델 실험, 전처리와 FastAPI 추론 서버 개발 | [AI 서버](https://github.com/BitOracle-bitoracle/bitoracle-ai-server) |
| Ya-Geum | 5인 팀장, 거래 화면·API·챌린지 데이터 설계, Railway Volume으로 재배포 후 데이터 유지 | [프론트엔드](https://github.com/yang5864/Ya-Geum) · [백엔드](https://github.com/yang5864/yageum-backend) |
| Tetz Bot | 스터디 운영 자동화. 1기에는 AI 난이도 평가·외부 API 교차검증, 현재 2기에는 인증·제출 확인과 중복 갱신 방지 | [코드](https://github.com/yang5864/Slack-msg) |
| Eobuba | 5인 팀으로 시니어 은행 방문 준비·금융사기 예방 서비스 기획과 프로토타입 제작에 참여 | 아래 해커톤 수상내역 |

## Activities & Writing

**KB IT's Your Life 7기 기자단 · 2026.03–2026.08**

24주간 주 1회 금융·IT 교육과 프로젝트 과정을 기록했습니다. 공식 문서와 실행 결과를 대조하고, 팀원의 담당 범위를 확인해 학습자가 참고할 수 있는 콘텐츠로 정리했습니다. 활동을 마치며 **최우수 기자상**을 수상했습니다.

[시나브로 기록하기 — 기자단·개발 기록 블로그](https://blog.naver.com/shy_fr00)<br>블로그 이웃 **4,428명 · 2026.09.07 기준**

| Period | Activity | Experience |
| :--- | :--- | :--- |
| 2026.03–2026.08 | KB IT's Your Life 7기 수료 | Java·Spring·DB·클라우드 학습과 팀 프로젝트 |
| 2026.05 | 모두의 창업 프로젝트 1기 도전 | Pacto의 문제 정의와 창업 아이디어 구체화 |
| 2026.09 | KB IT's Your Life 해커톤 본선 | 팀 효도과자·어부바 서비스 기획·프로토타입 |
| 2023.01–2023.02 | KG IT Bank C·Java 과정 수료 | 128시간의 프로그래밍·객체지향 실습 |

## Awards & Recognition

| Date | Recognition | Detail |
| :--- | :--- | :--- |
| 2026.09 | 금융권 공동채용박람회 **IBK기업은행 우수면접자 선정** | 면접 선발 실적 |
| 2026.09.10 | KB IT's Your Life 해커톤 **장려상** | 팀 효도과자·시니어 금융지원 서비스 어부바 |
| 2026.08.27 | KB IT's Your Life 7기 **최우수 기자상** | 금융·IT 교육 및 프로젝트 기록 |
| 2026.04.07 | KB IT's Your Life 1단위기간 **우수훈련생** | 교육·실습 참여 |
| 2022.06.12 | **제23경비여단장 표창** | 이상 징후 식별과 신속 보고 공로 |

## Certifications

- **AWS Certified Cloud Practitioner** · 2025.12 취득
- **SQLD** · 2025.09 취득

## How I Build

- **사용자 흐름에서 출발합니다.** 블로그 운영과 스터디에서 반복되는 불편을 직접 발견하고 서비스를 만들었습니다.
- **계산과 AI의 역할을 나눕니다.** 정확해야 하는 값은 코드가 계산하고, AI는 설명과 보완을 담당하게 합니다.
- **실패와 운영까지 확인합니다.** 재시도·중복 실행·트랜잭션·배포·관측을 기능과 함께 고민합니다.
- **기록을 다음 사람에게 연결합니다.** 구현 과정과 기술 선택을 문서와 블로그로 공유합니다.

---

<p align="center"><sub>프로젝트의 구현과 실행 방법은 연결된 저장소에서 확인할 수 있습니다.</sub></p>
