# 🏭  무게/등급에 따른 제품 분류 컨베이어벨트 프로젝트
![PLC](https://img.shields.io/badge/PLC-XG5000-blue)
![HMI](https://img.shields.io/badge/HMI-XP--Builder-lightgrey)
![Ladder Logic](https://img.shields.io/badge/Ladder%20Logic-%E2%9C%94-green)
![Industrial Automation](https://img.shields.io/badge/Industrial%20Automation-%E2%9C%94-orange)

---
## 📃 프로젝트 개요
1. **배경 및 필요성**
    - 최근 스마트 팩토리 도입이 활발해지면서 제조 공정에서의 **자동화 요구**가 급증하고 있음. 제조 산업에서는 생산 속도 및 품질 관리의 효율성을 극대화하기 위해 **자동화된 시스템 구축**이 필수적으로 요구됨. 특히, **생산 공정의 자동화**를 구현하기 위해서는 각 공정에서 발생할 수 있는 다양한 변수와 상황에 대해 즉각적인 대응이 가능한 PLC의 역할이 중요해지고 있음
    - **디지털 트윈** 기술: 현실의 사물과 환경을 **가상 공간에 그대로 구현**해 실시간 모니터링과 시뮬레이션을 가능하게 하는 기술. 국내 외 주요기업들이 디지털 트윈 기술을 제조 산업에 적용해 디지털 혁신에 기여하고 있음. 실제 공장을 시범 가동하지 않고도 최적화된 공장 가동률 등을 시험해 볼 수 있고, **원격으로 라인 가동 관리** 가능함.
    이에 따라 hmi 작화로 공장 라인을 그대로 구현하고 이를 plc와 연결해 실제 공장 가동 상황을 모니터링하고자 함.
2. **목표 및 방향 설정**
    
    이에 따라 제조 공정의 효율성을 높이기 위해 **PLC 알고리즘의 구조와 동작 원리**에 대한 심층적인 이해가 필요하다는 점을 인식하였음. 이를 위해 다음과 같은 구체적인 목표를 설정하였음.
    
    - 제품 생산 시 요구되는 **PLC의 기본 구조** 및 프로그래밍 방식 학습
    - 제조 공정에서 발생하는 **분류 및 처리 로직**에 대한 알고리즘 설계
    - 실제 자동화 프로세스에서 발생할 수 있는 상황을 반영한 **시뮬레이션 및 최적화**
---
## 💻 주요 기능

### <span style="background-color:grey">**📍 컨베이어 벨트 기반 제품 분류 시스템**</span>

**✔️ 기능1. 랜덤한 무게의 제품 생성**

- 1~100 범위의 난수를 입력 받아 각 제품 생산 시 할당

**✔️ 기능2. 품질 로봇에 의해 각 제품의 품질을 랜덤하게 할당** 

- 1~3 범위의 난수를 입력받아 품질 로봇 작동 시 각 제품의 품질을 할당
- 각 품질에 적합한 제품 이미지로 변화

**✔️ 기능3. 무게와 품질에 따라 각 소터의 동작 상태가 결정** 

**✔️ 기능4. 각 제품 분류 후 재고량 카운트** 
<br>

### <span style="background-color:grey">**📍 시스템 모니터링 시스템**</span>

**✔️ 기능1. 제품 데이터 모니터링**

- 100개의 재고가 쌓이면 자동 출고(재고량 0 RESET)
- 모니터링 데이터
    - 무게/등급별 재고량
    - 현재 생산 중인 제품의 등급 및 무게 데이터

**✔️ 기능2. 컨베이어 벨트 데이터 모니터링**

- 컨베이어 벨트
    - 속도 데이터 만큼 줄어듦
    - 0이 되었을 때 제품 생산 강제 종료
- 모니터링 데이터
    - 컨베이어 벨트 수명
    - 컨베이어 벨트 속도
<br>

### <span style="background-color:grey">📍 **속도 조절 시스템**</span>

- 제품 무게*0.1 만큼으로 자동 조정
---
## 🔧 활용 스택
- PLC: XG5000 (LS 산전/XGI)
- HMI: XP-Builder (LS산전/XGI CPU Eternet)
- 프로그래밍 언어: Ladder Logic, FBD
---
## 🔨 협업 툴

![GITHUB](https://img.shields.io/badge/GITHUB-lightgrey) - 결과물 시각화

![NOTION](https://img.shields.io/badge/NOTION-black) - 문서 공유 및 일정 관리

![ZOOM](https://img.shields.io/badge/ZOOM-blue) - 주기적인 회의

---
## 📆 프로젝트 수행 절차 - 마일스톤
![image (5)](https://github.com/user-attachments/assets/48045360-78c3-45fb-afe3-525fc8524a52)

---
## 👪 역할 분담

| 구성원 | 역할 | 주요업무 | 주요 활용 스택 | GITHUB |
|------|------|---------|-----|-----|
|이동건|팀장| 프로젝트 PM<br>전반적인 PLC 설계<br>프로젝트 문서화|![PLC](https://img.shields.io/badge/PLC-XG5000-blue) ![HMI](https://img.shields.io/badge/HMI-XP--Builder-lightgrey)|[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github)](https://github.com/a08160)|
|조경록|팀원| [제품 분류 시스템] 기능3/기능4 PLC 구현<br>[모니터링 시스템/속도 자동 조절 시스템] HMI 작화<br>발표|![PLC](https://img.shields.io/badge/PLC-XG5000-blue) ![HMI](https://img.shields.io/badge/HMI-XP--Builder-lightgrey)|[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github)](https://github.com/josh980510)|
|김혜은|팀원| [제품 분류 시스템] HMI 작화<br>전체적인 세부 디자인 완성<br>PPT 제작|![PLC](https://img.shields.io/badge/PLC-XG5000-blue) ![HMI](https://img.shields.io/badge/HMI-XP--Builder-lightgrey)|[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github)](https://github.com/hyeeun619)|
