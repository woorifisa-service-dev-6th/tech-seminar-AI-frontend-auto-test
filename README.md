# Frontend Test Automation using AI (Gemini CLI)
github URL: https://github.com/Nan-Navi-60/Clova-ChatBot/tree/main
## 결과 예시 
### Playwright
![6  시연영상](https://github.com/user-attachments/assets/651a8302-4eb8-4bd7-b6ce-beba876b73da)

### Slack
![AI를 활용한 프론트엔드 테스트 자동화](https://github.com/user-attachments/assets/3631068c-5514-461a-9781-85f96b4cf874)


## 실행 가이드
- 서버 실행 경로:
``` bash
node server.js
```
- 클라이언트 실행 경로: 
``` bash
npm run dev
```
- 테스팅 자동화 명령어 실행 경로:
``` bash
npm run test-and-report
npm run propose-improvements
```

### 환경 세팅

- .env 파일
``` bash
CLOVACHAT={APIGW_Invoke_URL} // CHATBOT 프로젝트를 이용할 경우 설정
CLIENT_SECRET={SECRET_KEY} // CHATBOT 프로젝트를 이용할 경우 설정

SLACK_WEBHOOK_URL={your_slack_webhook_url} // SLACK BOT 연동을 이용할 경우 설정
```

## 프로젝트 구조
![5](https://github.com/user-attachments/assets/e6080961-221b-4611-8679-f302a9ef4a51)
![6](https://github.com/user-attachments/assets/b515f7bb-0b87-45a9-bd6f-ff7a0a85598f)


## 폴더 설명 

# Chatbot 기능 소개
![AI를 활용한 프론트엔드 테스트 자동화](https://github.com/user-attachments/assets/90c508c2-3975-4f8f-805e-bfef9c698274)

![AI를 활용한 프론트엔드 테스트 자동화 (1)](https://github.com/user-attachments/assets/9b80fcbc-4be3-46df-9684-a03ca406894b)




#  Agentic Frontend Test Automation
> **AI 에이전트를 활용한 프론트엔드 테스트 자동화 및 Closed-loop 유지보수 시스템**

AI를 단순한 도구가 아닌 독립적인 **'에이전트(Agent)'** 단위로 설계하여, 테스트 시나리오 설계부터 결과 분석, 코드 수정 제안까지 수행하는 지능형 자동화 솔루션입니다.

---

##  1. Project Overview

### 배경 및 필요성
* **테스트 번거로움**: 프로젝트 규모에 따라 복잡해지는 테스트 시나리오와 테스트 코드 작성에 많은 시간이 소요됨.
* **AI를 활용한 테스트 효율화**: AI가 프로젝트의 흐름을 파악하고 주어진 시나리오를 통해 테스트 코드를 작성하고 테스트를 진행.

### 목표
* AI를 활용하여 테스트 코드 작성 및 진행
* 테스트 실패 시 원인 분석 및 해결책 제안.

---

##  2. System Architecture & Tech Stack

### 기술 스택
| 분류 | 기술 |
| :--- | :--- |
| **Framework** | `React` |
| **Testing Tool** | `Playwright` |
| **AI Model** | `Gemini 2.5 Flash` (Gemini-CLI) |

### AI 에이전트 역할 분담
* **SDET Agent**: 테스트 설계 및 Playwright 기반 아키텍처 구축.
* **Documentation Specialist**: 테스트 시나리오 구조화 및 개선 사항 자동 생성.
  
---
##  3. Key Features

### 1) 금융 챗봇(Woori-CLOVA) E2E 테스트
* **입력 폼 검증**: 사용자 데이터 유효성 검증 로직 테스트.
* **비동기 통신**: API 호출 및 데이터 렌더링(Async/Sync) 흐름 체크.

### 2) 지능형 자동화 워크플로우
1. **분석**: `Gemini-CLI`가 프로젝트 전체 흐름과 코드 구조를 파악.
2. **생성**: 기능별 데이터 라벨링(`data-cy`)을 감지하여 최적의 테스트 코드 작성.
3. **실행**: 생성된 코드를 기반으로 자동 테스트 수행 및 결과(`json`) 반환.
4. **개선**: 테스트 결과 분석 후, 실제 파일의 코드 수정 및 리팩토링 방안 제안.

---

##  4. Expected Effects
* **QA 사이클 단축**: 자동화를 통한 즉각적인 피드백 및 테스트 비용 절감.
* **코드 안정성 확보**: 리팩토링 시 기존 기능의 정상 작동을 보장하는 안전망 구축.
* **생산성 극대화**: 사람이 찾기 어려운 논리적 오류를 탐지하고 수정 대안 제시.

---

