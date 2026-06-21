# 🚀 AI Vibe Coding Studio (AI 바이브코딩 스튜디오)

"미래 기술을 교실의 책상 위로 옮기는 에듀테크 기업, 바운더리엑스"
코딩, AI, 로봇의 완벽한 융합을 위한 피지컬 AI(Physical AI) 코딩 어시스턴트

## 📖 소개 (About the Project)

AI 바이브코딩 스튜디오는 생성형 AI(Google Gemini API)를 활용하여 BBC Micro:bit V2 기반의 로봇 하드웨어 코드를 자동으로 생성, 개선, 디버깅해 주는 웹 애플리케이션입니다. 

단순히 화면 속 결과를 내는 것을 넘어, 로봇의 물리적인 움직임과 센서 제어를 이해하는 학습 여정(AXperience)을 제공합니다. 프론트엔드 환경에서만 단독으로 동작하도록 설계되어, 교실 현장에서 별도의 회원가입이나 복잡한 환경 세팅 없이 접속 링크만으로 즉시 활용 가능한 '가입 없는 SaaS' 환경을 구현했습니다.

### 🎯 타겟 디바이스
* AI Ponybot (AI 포니봇): 메카넘 휠, 초음파, 라인 트레이싱 등을 활용한 모빌리티 로봇
* Vibe Lamp (바이브램프): 네오픽셀과 디스플레이를 활용한 감성 인터랙티브 조명

---

## ✨ 주요 특징 (Key Features)

* 가입 없는 관리 시스템 (No Registration): 학생 개인정보 보호와 교사의 행정 부담 제로화를 위해 회원가입 없이 브라우저 단에서 API 키만 입력하여 즉시 사용 가능합니다.
* 강력한 AI 가드레일 (Zero Hallucination Policy): 
  - MakeCode PXT 엔진의 특성을 반영한 변수 선언 최적화(Type Inference 강제).
  - 하드웨어 핀 충돌(Pin Conflict) 방지 및 무한 루프 과부하 방어 설계.
  - 메카넘 휠의 수평/대각선 이동과 일반 회전을 완벽히 구분하는 물리적 모터 제어.
* 바운더리엑스 AI 통신 최적화: 실시간 AI 모드 전환 및 UART 데이터 파싱 시 통신 안정성을 보장하는 방어 로직이 적용되어 있습니다.
* 교육적 피드백: 코드를 생성할 때마다 단순한 코드 나열이 아닌, 로봇 하드웨어와 코딩 로직이 어떻게 연결되는지 학생의 눈높이에 맞춘 친절한 설명을 함께 제공합니다.

---

## 🛠️ 기술 스택 (Tech Stack)

* Frontend: React 18, Tailwind CSS
* Compiler/Transformer: Babel Standalone (v7.24.4)
* AI Integration: Google Gemini API (gemini-1.5-flash / gemini-2.5-flash)
* Typography: Pretendard (UI), JetBrains Mono (Code)

---

## 🚀 시작하기 (Getting Started)

본 프로젝트는 별도의 Node.js 서버나 빌드 과정 없이 단일 HTML 파일로 실행 가능한 구조입니다.

### 사용 방법
1. 바이브코딩 스튜디오에 접속합니다.
2. 우측 상단의 ⚙️ 설정 버튼을 클릭하여 발급받은 Google Gemini API Key를 입력합니다.
3. 상단의 탭에서 'AI 포니봇' 또는 '바이브램프'를 선택합니다.
4. 채팅창에 구현하고 싶은 동작을 한국어로 자연스럽게 입력합니다.
   * 예: "포니봇이 전진하다가 초음파 센서 거리가 10cm 이하가 되면 멈추게 해줘"
5. 생성된 코드를 복사하여 MakeCode for micro:bit의 JavaScript 탭에 붙여넣고 실행합니다.

---

## 💡 프롬프트 모드 (Work Modes)

작업의 효율을 높이기 위해 세 가지 프롬프트 모드를 지원합니다:
1. 새로 코드 작성하기: 기존 코드를 무시하고 백지상태에서 새로운 로직을 구성합니다.
2. 오른쪽 코드 개선하기: 현재 에디터에 있는 코드의 뼈대를 유지하며 새로운 기능을 추가합니다.
3. 오른쪽 코드 에러 해결하기: 논리적 오류나 동작 불량의 원인을 파악하고 코드를 수정합니다.

---

## 🛡️ 안전 및 보안 (Security & Privacy)

* 개인정보 무수집: 본 서비스는 사용자의 데이터를 서버로 전송하거나 저장하지 않습니다.
* 프롬프트 필터링: 시스템 프롬프트 내에 개인정보 입력 방지 및 수업과 무관한 잡담(Off-topic)을 차단하는 강력한 가드레일이 적용되어 있습니다.

---

## 📄 라이선스 및 저작권 (License & Copyright)

본 프로젝트의 소스 코드, 프롬프트 엔지니어링 구조(AI 하네스 및 시스템 프롬프트), 교육 커리큘럼 및 관련 문서에 대한 모든 지식재산권 및 저작권은 바운더리엑스(Boundary X)에 있습니다.

* 무단 복제 및 사용 금지: 사전 승인 없는 코드의 무단 복제, 배포, 상업적 사용을 엄격히 금지합니다.
* 출처 표기 의무: 교육적 목적의 제한적 참고 시에도 반드시 명확한 출처(Boundary X)를 밝혀야 하며, 출처를 은폐한 무단 도용 및 2차 가공은 허용되지 않습니다.

---

## 🏢 Contact & Support

바운더리엑스 (Boundary X)
* Lead Developer / Representative: 권현중 (Hyeon-joong Kwon)
* Website: https://boundaryx.io
* Product Info: https://boundaryx.io/shop

Copyright 2026 Boundary X Co. All rights reserved.
