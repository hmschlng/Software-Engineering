# 🍎 4-1 Functional and Non-functional Requirements
---
<br>

### ✅ Functional and Non-functional Requirements (기능 및 비기능 요구 사항)
- 기능 요구 사항
  - 시스템이 제공해야 하는 서비스, 시스템이 특정 입력에 어떻게 반응해야 하는지, 특정 상황에서 시스템이 어떻게 작동해야 하는지에 대한 설명.
  - 시스템이 하지 말아야 할 일을 명시할 수 있습니다.
- 기능 외 요구 사항
  - 타이밍 제약, 개발 프로세스에 대한 제약, 표준 등과 같이 시스템이 제공하는 서비스 또는 기능에 대한 제약.
  - 개별 기능이나 서비스가 아닌 시스템 전체에 적용되는 경우가 많습니다.
- 도메인 요구 사항
  - 운영 영역에서 시스템에 대한 제약 조건
<br>

### ✅ Functional requirements (기능적인 요구 사항)
- 기능 또는 시스템 서비스를 설명합니다.
- 소프트웨어 유형, 예상 사용자 및 소프트웨어가 사용되는 시스템 유형에 따라 다릅니다.
- 기능적 사용자 요구 사항은 시스템이 수행해야 하는 작업에 대한 상위 수준 설명일 수 있습니다.
- 기능 시스템 요구 사항은 시스템 서비스를 자세히 설명해야 합니다.
<br>

#### Mentcare 시스템의 기능적 요구 사항
1. 사용자는 모든 진료소에 대한 예약 목록을 검색할 수 있어야 합니다.
2. 시스템은 각 진료소에 대해 그날 예약에 참석할 것으로 예상되는 환자 목록을 매일 생성해야 합니다.
3. 시스템을 사용하는 각 직원은 8자리 직원 번호로 고유하게 식별됩니다.
<br>

#### 요구사항의 부정확성
- 기능적 요구사항이 정확하게 명시되지 않은 경우 문제가 발생합니다.
- 모호한 요구사항은 개발자와 사용자가 다르게 해석할 수 있습니다.
- Mentcare 요구사항 1에서 '검색'이라는 용어를 고려
  - 사용자 의도 – 모든 진료소의 모든 예약에서 환자 이름을 검색합니다.
  - 개발자 해석 – 개별 클리닉에서 환자 이름을 검색합니다. 사용자는 진료소를 선택한 다음 검색합니다.
<br>

#### 요구 사항의 완전성과 일관성
- 원칙적으로 요구사항은 완전하고 일관성이 있어야 합니다.
- 완료
  - 여기에는 필요한 모든 시설에 대한 설명이 포함되어야 합니다.
- 일관성
  - 시스템 설비의 설명에 충돌이나 모순이 없어야 한다.
- 실제로는 시스템 및 환경의 복잡성으로 인해 완전하고 일관된 요구 사항 문서를 생성하는 것이 불가능합니다.
<br>


### ✅ Non-functional requirements (비기능적 요구사항)
- 이들은 시스템 속성과 제약 조건을 정의합니다. 안정성, 응답 시간 및 저장 요구 사항. 제약 조건은 I/O 장치 기능, 시스템 표현 등입니다.
- 특정 IDE, 프로그래밍 언어 또는 개발 방법을 요구하는 프로세스 요구 사항을 지정할 수도 있습니다.
- 기능적 요구사항보다 비기능적 요구사항이 더 중요할 수 있습니다. 이러한 사항이 충족되지 않으면 시스템이 무용지물이 될 수 있습니다.
<br>

#### 비기능적 요구사항의 유형
![1](https://i.imgur.com/osPoC1w.png)
<br>

#### 비기능적 요구사항의 구현
- 기능 외 요구 사항은 개별 구성 요소보다 시스템의 전체 아키텍처에 영향을 줄 수 있습니다.
  - 예를 들어, 성능 요구 사항이 충족되도록 하기 위해 구성 요소 간의 통신을 최소화하도록 시스템을 구성해야 할 수 있습니다.
- 보안 요구사항과 같은 단일 비기능 요구사항은 필요한 시스템 서비스를 정의하는 여러 관련 기능 요구사항을 생성할 수 있습니다.
  - 기존 요구 사항을 제한하는 요구 사항을 생성할 수도 있습니다.
<br>

#### 비기능적 분류
- 제품 요구 사항
  - 배송된 제품이 특정 방식으로 작동해야 함을 지정하는 요구 사항. 실행 속도, 신뢰성 등
- 조직적 요구사항
  - 조직 정책 및 절차의 결과인 요구 사항. 사용된 프로세스 표준, 구현 요구 사항 등
- 외부 요구 사항
  - 시스템 및 개발 프로세스의 외부 요인에서 발생하는 요구 사항. 상호 운용성 요구 사항, 입법 요구 사항 등
<br>

#### Mentcare 시스템의 비기능적 요구 사항의 예
![1](https://i.imgur.com/n9XdaHy.png)
<br>

#### 목표와 요구 사항
- 비기능적 요구사항은 정확하게 기술하기가 매우 어려울 수 있으며 부정확한 요구사항은 검증하기 어려울 수 있습니다.
- 목표
  - 사용의 용이성과 같은 사용자의 일반적인 의도.
- 검증 가능한 비기능 요구사항
  - 객관적으로 테스트할 수 있는 몇 가지 척도를 사용한 진술.
- 목표는 시스템 사용자의 의도를 전달하므로 개발자에게 도움이 됩니다.
<br>

#### 사용성 요구사항
- 시스템은 의료진이 쉽게 사용할 수 있어야 하며 사용자의 실수를 최소화할 수 있도록 구성되어야 합니다. (목표)
- 의료진은 4시간 교육 후 모든 시스템 기능을 사용할 수 있어야 합니다. 이 교육 후 숙련된 사용자의 평균 오류 수는 시스템 사용 시간당 2개를 초과하지 않아야 합니다. (테스트 가능한 비 기능 요구 사항)
<br>

#### 비기능 요구 사항을 지정하기 위한 척도
<table>
  <tr>
    <td><b>속성</td>
    <td><b>측정</td>
  </tr>
  <tr>
    <td>속도</td>
    <td>
      - 처리된 트랜잭션 (초당)<br>
      - 사용자 / 이벤트 응답 시간<br>
      - 화면 새로 고침 시간</td>
  </tr>
  <tr>
    <td>크기</td>
    <td>
      - MB<br>
      - ROM 칩의 개수</td>
  </tr>
  <tr>
    <td>사용의 용이성</td>
    <td>
      - 훈련 시간<br>
      - 도움말 프레임 수</td>
  </tr>
  <tr>
    <td>신뢰성</td>
    <td>
      - 평균 실패 시간<br>
      - 이용 불가 확률<br>
      - 고장 발생률<br>
      - 유효성</td>
  </tr>
  <tr>
    <td>견고성</td>
    <td>
      - 실패 후 재시작 시간<br>
      - 실패를 유발하는 이벤트 비율<br>
      - 장애 시 데이터 손상 가능성</td>
  </tr>
  <tr>
    <td>휴대성</td>
    <td>
      - 대상 종속 명령문의 백분율<br>
      - 대상 시스템 수</td>
  </tr>
</table>
<br>

#### 
<br>

#### 
<br>