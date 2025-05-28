<!-- 헤더 이미지 -->

![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=300&section=header&text=Welcome%20to%20dbp-jack%27s%20GitHub!%20%F0%9F%91%8B%F0%9F%8F%BB&fontSize=52&animation=fadeIn&fontAlignY=36&textColor=ffffff)

<!-- 소개 문구 -->

# 안녕하세요.  
**실전에서 부딪히고, 그 경험을 가공하는 개발자 dbp-jack입니다.**  
_Developer forged by real-world challenges and refined by experience._

📫 **Email**: dbp100402@gmail.com  
📘 **Blog**: [https://dev99-tale.tistory.com](https://dev99-tale.tistory.com)

---

## 🔧 Skills

<!-- 백엔드 -->
![Java](https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat)
![QueryDSL](https://img.shields.io/badge/QueryDSL-009688?style=flat)
![MSA](https://img.shields.io/badge/MSA-FF7043?style=flat)

<!-- 데이터 / 인프라 -->
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![AWS ECS](https://img.shields.io/badge/AWS_ECS-FF9900?style=flat&logo=amazonaws&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat&logo=amazonec2&logoColor=white)

<!-- 협업 -->
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=flat&logo=jira&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=flat&logo=slack&logoColor=white)

---

## 📊 GitHub Stats

<img src="https://github-readme-stats.vercel.app/api?username=dbp-jack&show_icons=true&theme=default" alt="dbp-jack's GitHub stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=dbp-jack&layout=compact&theme=default" alt="Top Languages" />

> ⚠️ 상단 언어 통계는 개인 소유 레포지토리 기준이며, Organizations 활동은 포함되지 않습니다.

---

## 📁 Projects

### 🧢 [Teepick](https://github.com/FINAL-SPARTA/SPARTA-FINAL-PROJECT)  
**2025.04 – 2025.05**  
야구 팬을 위한 티켓 예매·이벤트·채팅 통합 플랫폼
대규모 트래픽 대응과 결제 시스템이 반영된 MSA기반 시스템 구현
팀 구성: 4명 / 역할: 팀장  
담당 도메인: 주문, 결제, 인프라 (AWS ECS)  
- 구현/성과:  
  - 주문 생성 및 결제 결과에 따른 상태 전이 API 구현, Kafka 기반 비동기 이벤트 흐름 설계
  - TICKET_RESERVED 수신 시 주문 생성 및 ORDER_CREATED 발행, 결제 결과에 따른 상태 전이 및 보상 트랜잭션 처리
  - Toss Payments API 연동을 통한 실결제 처리 및 결제 취소 API 구현
  - Kafka 이벤트 기반 구조로 결합도 감소 및 처리 흐름 안정화
  - Feign → Kafka 전환으로 응답 시간 83% 개선 (128ms → 21ms)
  - Kafka 병렬 처리 구조로 TPS 3배 향상 (83.3 → 250), 응답 시간 60% 단축 (6379ms → 2515ms)

FIX - [👉 프로젝트 팀 노션 바로가기](https://slime-face-7c4.notion.site/9-FIX-1f0eeaa2f0af801c9cfffc280207a3be?pvs=4)

---

### 🚛 [B2B 물류 시스템](https://github.com/sparta-i4u/sparta-msa)  
**2025.03 – 2025.04**
물류 관리 및 배송 시스템을 위한 MSA 기반 플랫폼
- 팀 구성: 4명 / 역할: 팀장  
- 담당 도메인: 유저, 인증, 게이트웨이, 인프라(Docker)  
- 구현/성과:  
  - 유저 서비스 및 인증 처리, API Gateway 설계
  - JWT 기반 토큰 인증 구조 설계, Auth 서비스에서 토큰 생성·검증, Gateway에서 인증 필터 적용
  - Redis 기반 유저 조회 캐싱 적용으로 DB 부하 분산 및 응답 속도 개선
  - Spring Cloud Gateway + Eureka 기반 API 라우팅 및 서비스 디스커버리 구성
  - 인증과 사용자 도메인 분리 및 단일 책임 원칙에 따른 서비스 구조 개선
  - WebClient 기반 내부 비동기 통신 구성 → 프론트 없는 구조에서 도메인 간 데이터 전달 문제 해결
  - 인증/조회 기능 분리와 캐시 적용으로 응답 속도 및 구조 안정성 향상
 
I4U - [👉 프로젝트 팀 노션 바로가기](https://slime-face-7c4.notion.site/16-I-4-U-1f0eeaa2f0af80bd9f00d0a062903703?pvs=4)
---

### 🍱 [B2C 음식 주문 플랫폼](https://github.com/sparta-onetoone/sparta-onetoone)  
**2025.02 – 2025.03** 
  음식점들의 배달 및 포장 주문 관리, 결제, 그리고 주문 내역 관리 기능을 제공하는 플랫폼
  모놀리식 아키텍처 및 4계층 레이어드 아키텍처로 구성
  추후 MSA 적용을 위해, 각 도메인 간의 의존성과 연관관계를 최소화하여 독립적인 관계를 맺도록 시스템 아키텍처를 설계
- 팀 구성: 4명 / 역할: 팀장  
- 담당 도메인: 가게, 리뷰, 카테고리  
- 구현/성과:  
  - 가게 등록/수정/삭제, 카테고리 기반 검색, 리뷰 작성 및 수정 등 도메인 기능 구현
  - 각 도메인 간 의존성을 최소화한 독립 구조 설계
  - Swagger 기반 API 문서화로 프론트 협업 및 확장성 고려한 인터페이스 구축
  - WebClient 도입으로 내부 도메인 간 데이터 전송 문제 해결
  - 모놀리식 구조 내 도메인 분리 및 단일 책임 원칙 적용으로 유지보수성과 확장성 확보
 
OneToOne - [👉 프로젝트 팀 노션 바로가기](https://slime-face-7c4.notion.site/11-OneToOne-1f0eeaa2f0af80199d6bc47ac641e384?pvs=4)
---

### 🧠 [AI 홍보물 제작 서비스](https://github.com/flyai-Ambition7)  
**2023.12 – 2024.02** 
  자영업자들이 홍보물 제작 과정에서 겪는 시간과 비용을 절감시켜 주는 서비스 플랫폼  
  사용자가 텍스트와 이미지를 입력하면, 현수막·전단지·SNS 이미지를 자동으로 생성하는 생성형 AI 기능 제공
- 팀 구성: 5명 / 역할: 팀원  
- 담당: 백엔드 API 서버 구축, DB 설계
- 구현/성과:
- DRF 기반 API 설계 및 모바일 연동 경험 확보
  - 모바일 앱(Android)과 연동 가능한 RESTful API 백엔드 서버 구축
  - DRF 기반 API 설계 및 모바일 연동 경험 확보
  - ngrok을 활용한 임시 배포 및 테스트 환경 구성 
  - 소상공인 40명 대상 설문을 통해 수요 기반 기능 도출 및 기획 반영  
  - 발표회에서 기술 흐름과 구현 성과를 설명하며 커뮤니케이션 역량 강화

---

### ❤️ [ECG 기반 건강 모니터링](https://github.com/dbp-jack/Development-of-daily-life-physical-monitoring-web-service-using-electrocardiogram-sensor.git)  
**2023.09 – 2024.01**  
  심전도(ECG) 센서를 활용한 실시간 부정맥 감지 및 건강 관리 웹 서비스 플랫폼  
  코로나19 이후 증가한 심장질환 문제에 대응하기 위해, 일상 속에서 부정맥을 실시간으로 측정할 수 있는 시스템 개발을 목표로 프로젝트를 수행함
- 팀 구성: 3명 / 역할: 팀장  
- 담당 : 백엔드 개발, 시스템 설계 및 구축, 논문 작성 및 교류회 발표
- 구현/성과:  
  - 초기에는 setInterval 기반 AJAX 방식으로 실시간 ECG 데이터를 처리했으나, 서버 부하 증가와 데이터 지연·누락 문제가 발생  
  - 이를 AJAX 롱 폴링 방식으로 개선하여 중복 요청과 불필요한 부하를 제거하고, 데이터 손실 없는 안정적인 흐름 유지  
  - 그 결과 평균 응답 지연 시간이 320ms에서 90ms로 약 72% 감소, 0.1초 이내의 실시간 반응성 확보
  - [2023 한국실천공학교육학회 추계종합학술대회 - 학술 논문 발표](https://slime-face-7c4.notion.site/2023-1f0eeaa2f0af802ebe9ece38cc503e4d?pvs=4)
  - [대전대학교 - 호치민시 베트남국립대학교, 글로벌 캡스톤디자인 성과 교류](https://www.dailycc.net/news/articleView.html?idxno=751998#google_vignette)
---

### 🏗️ [ICT 인턴십] – 건설현장 대시보드(개인 프로젝트 6개월)
**2023.03 – 2023.08** 
  건설현장 근로자의 안전장비 착용 상태 실시간 수집 및 시각화하는 웹 기반 안전관리 대시보드 프로토타입 구현
- 기술 스택: Django, Python, JS(AJAX), Bootstrap, MySQL, HTML, CSS
- 담당:
  - 기획 및 보고서 작성, UI/UX 설계
  - 로그인·회원가입, 작업기록 게시판 3종, 직원 조 편성, 실시간 데이터 시각화 기능 구현

- 구현/성과:  
  - Django 기반 웹 대시보드 전체 기능 기획 및 개발  
  - AJAX(0.1초 주기)를 통한 실시간 센서 데이터 처리  
  - SW 요구사항 정의, Flowchart 및 권한 구성 문서화  
  - 기술적 제약 속 실시간 구현 성공 → 문제 해결력 및 협업 역량 향상

