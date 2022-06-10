# 8-3 Release Testing
---
<br>

### ✅ Release testing (릴리스 테스트)
<br>

- 릴리스 테스트는 개발 팀 외부에서 사용하도록 설계된 시스템의 특정 릴리스를 테스트하는 프로세스입니다.
<br>

- 릴리스 테스트 프로세스의 주요 목표는 시스템이 사용하기에 충분하다는 것을 공급자에게 납득시키는 것입니다.
  - 따라서 릴리스 테스트는 시스템이 지정된 기능, 성능 및 신뢰성을 제공하며 정상적인 사용 중에 고장이 발생하지 않음을 보여주어야 합니다.
<br>

- 릴리스 테스트는 일반적으로 블랙박스 테스트 프로세스로, 테스트는 시스템 사양에서만 파생됩니다.
<br>

### ✅ Release testing and system testing (배포 테스트와 시스템 테스트)
<br>

- 릴리스 테스트는 시스템 테스트의 한 형태입니다.
<br>

- 중요한 차이점:
  - 시스템 개발에 관여하지 않은 별도의 팀이 릴리스 테스트를 담당한다.
  - 개발팀의 시스템 테스트는 시스템 내 버그(bug)를 발견하는 데 중점을 두어야 한다. 릴리스 테스트의 목적은 시스템이 요구 사항을 충족하고 외부 사용에 충분한지 확인하는 것입니다(검증 테스트).
<br>

### ✅ Requirements based testing (요구사항 기반 테스트)
<br>

- 요구사항 기반 테스트는 각 요구사항을 검사하고 그에 대한 테스트 또는 테스트를 개발하는 것을 포함한다.
<br>

- 예시 : 멘트케어 시스템 요구사항:
  - 환자가 특정 의약품에 알레르기가 있는 것으로 알려진 경우 해당 의약품의 처방을 통해 시스템 사용자에게 경고 메시지가 전달되어야 합니다.
  - 처방자가 알레르기 경고를 무시하기로 선택한 경우, 이를 무시한 이유를 제시해야 한다.
<br>

### ✅ Requirements tests (요구사항 테스트)
<br>

- 알려진 알레르기가 없는 환자 기록을 설정합니다. 존재하는 것으로 알려진 알레르기에 대한 약을 처방한다. 시스템에 의해 경고 메시지가 발행되지 않는지 점검하십시오.
<br>

- 알려진 알레르기가 있는 환자 기록을 설정합니다. 환자가 알레르기가 있는 약물을 처방하고 시스템에서 경고가 발생하는지 확인합니다.
<br>

- 두 개 이상의 약물에 대한 알레르기가 기록된 환자 기록을 설정합니다.
이 두 가지 약을 각각 처방하고 각 약물에 대한 올바른 경고가 발행되었는지 확인하십시오.
<br>

- 환자가 알레르기가 있는 두 가지 약을 처방한다. 두 개의 경고가 올바르게 발행되었는지 점검하십시오.
<br>

- 경고를 발하는 약을 처방하고 경고를 무시합니다. 시스템에서 사용자에게 경고가 무시된 이유를 설명하는 정보를 제공해야 하는지 점검하십시오.
<br>

#### 예시 : Mentcare 시스템의 사용 시나리오
조지는 정신 건강 관리를 전문으로 하는 간호사이다. 그의 책임 중 하나는 집에 있는 환자들을 방문하여 그들의 치료가 효과적이고 그들이 약물 부작용으로 고통 받고 있지 않은지 확인하는 것이다.
가정 방문을 위한 날에 조지는 Mentcare 시스템에 로그인하여 방문하려는 환자에 대한 요약 정보와 함께 그날의 가정 방문 일정을 인쇄하는 데 사용합니다. 그는 이 환자들의 기록을 그의 노트북에 다운로드 할 것을 요청한다. 그는 노트북의 기록을 암호화하기 위한 핵심 문구를 입력하라는 메시지를 받는다.
그가 방문하는 환자 중 한 명은 우울증 치료제로 치료를 받고 있는 짐이다. 짐은 그 약이 자신을 돕고 있다고 느끼지만, 그것이 밤에 잠을 자지 못하게 하는 부작용이 있다고 믿는다. 조지는 짐의 기록을 찾아보고 그 기록을 해독하기 위한 핵심 문구를 입력하라는 메시지를 받는다. 그는 처방된 약을 확인하고 부작용에 대해 의문을 제기한다. 잠 못 이루는 것은 알려진 부작용이기 때문에 그는 짐의 기록에 문제를 기록하고 약을 바꾸기 위해 병원을 방문하라고 제안한다. 짐도 동의해서 조지가 진료소로 돌아가 의사와 약속을 잡으면 그에게 전화를 걸라는 프롬프트를 표시합니다. 조지는 상담을 끝내고 시스템은 짐의 기록을 다시 암호화한다.
상담이 끝난 후 조지는 진료소로 돌아와 방문했던 환자들의 기록을 데이터베이스에 올린다. 시스템은 George가 후속 정보를 얻고 진료 예약을 위해 연락해야 하는 환자들의 통화 목록을 생성합니다.
<br>

#### 시나리오별로 테스트된 기능
<br>

- 시스템에 로그온하여 인증합니다.
<br>

- 지정된 환자 기록을 랩톱에 다운로드 및 업로드합니다.
<br>

- 홈 방문 일정 설정.
<br>

- 모바일 장치의 환자 기록 암호화 및 암호 해독
<br>

- 검색 및 수정을 기록합니다.
<br>

- 부작용 정보를 유지하는 약물 데이터베이스와 연결합니다.
<br>

- 통화 프롬프트용 시스템입니다.
<br>

### ✅ Performance testing (성능 테스트)
<br>

- 릴리스 테스트의 일부는 성능 및 신뢰성과 같은 시스템의 새로운 특성 테스트를 포함할 수 있다.
<br>

- 테스트는 시스템 사용 프로파일을 반영해야 한다.
<br>

- 성능 시험은 일반적으로 시스템 성능을 허용할 수 없을 때까지 부하가 지속적으로 증가하는 일련의 시험을 계획하는 것을 포함한다.
<br>

- 스트레스 테스트는 시스템이 고장 동작을 테스트하기 위해 의도적으로 오버로드되는 성능 테스트의 한 형태입니다.
<br>
