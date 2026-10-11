# Jaeseok Lim

> 작은 모듈을 모아 하나의 시스템으로 만드는 서버 개발자

**🎂 Birth**

1999.09.09

**📞 Phone**

010-4071-2296

**✉️ E-Mail**

dlawotjr1999@gmail.com

🐱 **Github**

https://github.com/dlawotjr1999

📘 **Notion(Tech Learning)**

https://swamp-scaffold-bfd.notion.site/b0b4a9ee9750441f8d62cc94afe187e3?source=copy_link

📖 **Portfolio**

https://drive.google.com/drive/folders/1zV1RC6aJ3CuYP9so0h0QUbdiNZ4qzE4y?usp=drive_link

## Education
- 충주대원고등학교 졸업(2015.03 ~ 2018.02)
- 서울시립대학교 컴퓨터과학부 졸업(2018.03 ~ 2025.02)
  
## Info
[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=dlawotjr1999)](https://solved.ac/dlawotjr1999/)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=dlawotjr1999&layout=compact)
[![GitHub stats](https://github-readme-stats.vercel.app/api?username=dlawotjr1999)](https://github.com/anuraghazra/github-readme-stats)

## Language
![c](https://img.shields.io/badge/c-A8B9CC.svg?&style=for-the-badge&logo=c&logoColor=black)
![cplusplus](https://img.shields.io/badge/c%2B%2B-00599C.svg?&style=for-the-badge&logo=c%2B%2B&logoColor=white)
![C#](https://img.shields.io/badge/C-Sharp-239120.svg?&style=for-the-badge&logo=C&logoColor=white)
![java](https://img.shields.io/badge/java-ED8B00.svg?&style=for-the-badge&logo=openjdk&logoColor=white)
![javascript](https://img.shields.io/badge/javascript-F7DF1E.svg?&style=for-the-badge&logo=javascript&logoColor=black)

## Backend
![springboot](https://img.shields.io/badge/spring_boot-6DB33F.svg?&style=for-the-badge&logo=springboot&logoColor=white)
![jpa](https://img.shields.io/badge/jpa-59666C.svg?&style=for-the-badge&logo=hibernate&logoColor=white)
![postgresql](https://img.shields.io/badge/postgresql-4169E1.svg?&style=for-the-badge&logo=postgresql&logoColor=white)
![mysql](https://img.shields.io/badge/mysql-4479A1.svg?&style=for-the-badge&logo=mysql&logoColor=white)
![firebase](https://img.shields.io/badge/firebase_auth-DD2C00.svg?&style=for-the-badge&logo=firebase&logoColor=white)

## System & Network
![linux](https://img.shields.io/badge/linux-FCC624.svg?&style=for-the-badge&logo=linux&logoColor=black)
![posixsocket](https://img.shields.io/badge/posix_socket-333333.svg?&style=for-the-badge)

## Infra & DevOps
![docker](https://img.shields.io/badge/docker-2496ED.svg?&style=for-the-badge&logo=docker&logoColor=white)
![kubernetes](https://img.shields.io/badge/kubernetes-326CE5.svg?&style=for-the-badge&logo=kubernetes&logoColor=white)
![githubactions](https://img.shields.io/badge/github_actions-2088FF.svg?&style=for-the-badge&logo=githubactions&logoColor=white)

## Client & Engine
![reactnative](https://img.shields.io/badge/react_native-20232A.svg?&style=for-the-badge&logo=react&logoColor=61DAFB)
![unity](https://img.shields.io/badge/unity-FFFFFF.svg?&style=for-the-badge&logo=unity&logoColor=black)
![unrealengine](https://img.shields.io/badge/unrealengine-0E1128.svg?&style=for-the-badge&logo=unrealengine&logoColor=white)

## Most Interested
- Server Development
- Cloud · Container Service
- Destributed System

---

## Projects

### Allargando (2026.03 ~ 2026.10)

<img width="541" height="479" alt="Image" src="https://github.com/user-attachments/assets/c3ea30a5-4df9-49d4-8226-c1f351cefee9" />

- [Github](https://github.com/dlawotjr1999/Allargando)
- 악기 취미생들을 위한 연주 모임 플랫폼 (React Native와 Spring Boot 기반의 취미생 앙상블 매칭 서비스)
- 2인 / React Native, Spring Boot, PostgreSQL, Firebase Authentication · FCM, GitHub Actions
- 담당 파트
    - ERD 및 시스템 아키텍처 설계
    - Frontend : 앱 화면 및 navigation 구조 설계
    - Backend : 회원정보 관리 및 지원서 작성 구현
- 주요 내용
    - 동시 가입 시 정상 Firebase 계정까지 삭제할 수 있는 보상 로직 제거, 트랜잭션 경계 분리와 UID 재조회로 멱등 가입 구현
    - AFTER_COMMIT 이벤트와 전용 Executor로 알림을 분리해 롤백된 작업의 FCM 발송 방지
    - 정원 축소·수락 철회 시 인원과 마감 상태의 불일치를 엔티티 규칙·@Version·DB CHECK로 방어
    - HTTP 200으로 오류를 반환하는 KOPIS 응답을 XML 오류 코드로 판별하고 장르·페이지 단위로 실패 격리
    - Firebase·DB 장애를 인증 실패(401)와 구분해 503으로 응답, 일시 장애에 앱이 로그아웃되지 않도록 수정

---

<img width="495" height="291" alt="Image" src="https://github.com/user-attachments/assets/411817b5-bffb-431c-93ce-238eeab84001" />

### Chat Server (2025.12 ~ 2026.08)

- [Github](https://github.com/dlawotjr1999/ServerProject)
- epoll TCP 채팅 서버를 Redis 기반 다중 Pod 구조로 확장한 서버 프로젝트
- 개인 프로젝트 / C, C++17, pthread, POSIX Socket, Redis, Docker, Kubernetes, Prometheus, Grafana, GitHub Actions
- 주요 내용
    - epoll 기반 단일 net thread와 Logic Worker 4개를 Job Queue로 연결하고, 메시지 유형별 큐 포화 정책(CHAT 드롭 / JOIN·LEAVE·DISCONNECT 대기) 적용
    - fd 재사용 문제에 대응해 session_id로 작업 대상을 분리하고 세션 수명 관리 재설계
    - 다중 Pod에서 session_id 충돌로 발생한 메시지 누락을 Redis INCR 기반 global_id로 해결
    - Pod 종료 후 방 인원 누수의 원인을 lease·count 동시 만료로 분석, lease·heartbeat로 회수하도록 키 수명 분리
    - 300개 연결에서 세 버전의 전달 지연 비교 : 세션 재설계 전후 지연은 유사, Redis 도입 후 p99 증가(37.01ms → 101.73ms) 기록
    - TSan으로 경합을 수정하고 CI에 동시성 회귀 검사 추가

---

<img width="308" height="430" alt="Image" src="https://github.com/user-attachments/assets/b5cde1ea-bb24-4015-bb34-23b292a998c8" />

### Capstone Project (2024.09 ~ 2024.12)

- [Github](https://github.com/dlawotjr1999/Capstone) & [Capstone Archive](https://capstone.uos.ac.kr/cdc/index.php/2%EB%B6%84%EB%B0%98-%EC%8B%9C%EA%B7%B8%EB%AA%A8%EC%9D%B4%EB%93%9C)
- STT & SER을 활용한 퍼즐 어드벤처 게임
- 4인 / Unity, C#, ONNX, Sentis
- 담당 파트
    - 게임 시스템 아키텍처 설계 및 전투 시스템 구현
    - 음성 및 감정 인식 결과를 검증·변환해 중앙 Manager에서 스킬 발동과 상태이상 적용으로 통합
    - 방 생성 및 Trigger 기반 전투 시스템 구현, Room 단위 NavMeshSurface·NavMeshLink로 런타임 맵의 이동 경로 구성
    - 전체 Room 활성화와 현재·인접 Room 활성화 방식의 부하를 비교해, 플레이 중 프레임 안정성을 우선한 전체 사전 활성화 채택

---

<img width="308" height="413" alt="Image" src="https://github.com/user-attachments/assets/7dfc5053-6922-45fa-b4f9-57431e1c902d" />

### Project Orpheus(2024.02 ~ 2024.07)

- [영상](https://www.youtube.com/watch?v=auBd6zEksRw)
- 3D 로그라이크 게임
- 2024 GIGDC 공모전 출품작
- 6인 / Unity, C#, CSV
- 담당 파트
    - 몬스터·아이템·스킬·스토리 데이터의 수작업 반영을 줄이기 위해 CSV 기반 Import 파이프라인 설계
    - ID·타입별 ScriptableObject 생성과 Prefab·Resource·Manager 참조를 자동화해 한 번의 Import로 게임 데이터가 일관되게 반영되는 구조 구축
    - NPC 상호작용, 퀘스트 상태 흐름 및 인벤토리·도감·미니맵 UI 구현
    - 카메라(시네마틱) 시스템, 몬스터 및 오브젝트 기능 구현

---

<img width="308" height="430" alt="Image" src="https://github.com/user-attachments/assets/d0fc1ba5-3fbd-4b1d-b3d1-753f17c03d9c" />

### 서울시 공영주차장 입지선정을 위한 분석 (2022.10 ~ 2023.12)

- 앙상블 기법을 통한 서울시 공영주차장 입지선정을 위한 분석
- Sklearn을 활용한 데이터 분석
- 회귀 분석과 클러스터링으로 1차 분석 후 앙상블 기법을 활용하여 2차 분석 진행
- 분석 후 여러 기사들과 자료들을 활용하여 교차검증 진행

---

## Certification
- 정보처리기사 (2025.12.24)
- SQLD (2024.09.20)
- OPIc Intermediate High (2024.11.09 ~ 2026.11.08)
