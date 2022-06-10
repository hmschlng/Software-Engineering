# 8-1 Development Testing
---

<br>

### ✅ Development testing (개발 테스트)
<br>

- 개발시험은 시스템 개발팀이 수행하는 모든 시험활동을 포함한다.
  - 단위 테스트, 개별 프로그램 단위 또는 객체 클래스를 테스트합니다. 장치 시험은 물체나 방법의 기능성 시험에 중점을 두어야 한다.
  - 구성 요소 테스트. 여러 개별 장치가 통합되어 복합 구성 요소를 생성합니다. 구성요소 시험은 구성요소 인터페이스 시험에 중점을 두어야 한다.
  - 시스템 테스트. 시스템의 일부 또는 모든 구성 요소를 통합하고 시스템을 전체적으로 테스트합니다.
시스템 시험은 구성요소 상호작용 시험에 중점을 두어야 한다.
<br>

### ✅ Unit testing (유닛 테스트)
<br>

- 유닛 테스트는 개별 구성 요소를 격리하여 테스트하는 프로세스입니다.
<br>

- 이것은 결함 테스트 과정입니다.
<br>

- 단위는 다음과 같습니다.
  - 객체 내 개별 기능 또는 방법
  - 여러 속성 및 메서드가 있는 객체 클래스
  - 기능에 액세스하는 데 사용되는 인터페이스가 정의된 복합 구성 요소.
<br>

### ✅ Object class testing (객체 클래스 테스트)
<br>

- 강의의 전체 시험 범위는 다음을 포함한다.
  - 물체와 관련된 모든 작업 테스트
  - 모든 객체 속성 설정 및 조회
  - 가능한 모든 상태에서 물체를 연습한다.
<br>

- 상속은 테스트할 정보가 현지화되지 않기 때문에 객체 클래스 테스트를 설계하는 것을 더 어렵게 만듭니다.
<br>

#### 예시 : 기상 관측소 객체 인터페이스
![캡처](https://i.imgur.com/CrZ9iyE.png)
<br>

#### 예시 : 기상 관측소 테스트
<br>

- 날씨 보고, 보정, 테스트, 시작 및 종료에 대한 테스트 사례를 정의해야 합니다.
<br>

- 상태 모델을 사용하여 테스트할 상태 전환 순서와 이러한 전환을 유발하는 이벤트 순서를 식별합니다.
<br>

- 예를 들어:
  - 종료 -> 실행 -> 종료
  - 구성-> 실행-> 테스트 -> 전송 -> 실행
  - 실행-> 수집-> 실행-> 요약 -> 전송 -> 실행
<br>

### ✅ Automated testing (자동 테스트)
<br>

- 가능한 경우 수동 개입 없이 테스트를 실행하고 점검할 수 있도록 장치 테스트를 자동화해야 합니다.
<br>

- 자동 장치 테스트에서는 테스트 자동화 프레임워크(예: JUnit)를 사용하여 프로그램 테스트를 작성하고 실행합니다.
<br>

- 단위 테스트 프레임워크는 특정 테스트 사례를 생성하기 위해 확장하는 일반 테스트 클래스를 제공합니다. 그런 다음 사용자가 구현한 모든 테스트를 실행하고 다른 테스트의 성공 여부를 일부 GUI를 통해 보고할 수 있습니다.
<br>

#### 자동화된 테스트 구성 요소
<br>

- 테스트 케이스, 즉 입력 및 예상 출력으로 시스템을 초기화하는 설정 파트입니다.
<br>

- 테스트할 개체 또는 메서드를 호출하는 호출 파트입니다.
<br>

- 통화 결과를 예상 결과와 비교하는 어설션 파트입니다. 주장이 참으로 평가되면 테스트가 거짓이면 성공한 것이고 실패한 것입니다.
<br>

### ✅ Choosing unit test cases (유닛 테스트 케이스 선택)
<br>

- 테스트 사례는 예상대로 사용할 때 테스트 중인 구성요소가 수행해야 할 작업을 수행한다는 것을 보여 주어야 합니다.
<br>

- 부품에 결함이 있는 경우 테스트 사례를 통해 이를 밝혀야 합니다.
<br>

- 따라서 다음과 같은 두 가지 유형의 장치 테스트 사례가 발생합니다.
  - 이 중 첫 번째 항목은 프로그램의 정상 작동을 반영해야 하며 구성 요소가 예상대로 작동함을 보여야 한다.
  - 다른 종류의 시험사례는 일반적인 문제가 발생하는 부분에 대한 시험경험을 바탕으로 한다. 비정상적인 입력을 사용하여 올바르게 처리되었는지 확인하고 구성 요소를 손상시키지 않아야 합니다.
<br>

### ✅ Testing strategies (테스트 전략)
<br>

- 파티션 테스트 - 공통 특성을 가지며 동일한 방식으로 처리되어야 하는 입력 그룹을 식별합니다.
  - 각 그룹 내에서 검정을 선택해야 합니다.
<br>

- 테스트 지침을 사용하여 테스트 사례를 선택하는 지침 기반 테스트입니다.
  - 이러한 지침은 프로그래머가 구성 요소를 개발할 때 자주 저지르는 오류에 대한 이전의 경험을 반영합니다.
<br>

### ✅ Partition testing (파티션 테스트)
<br>

- 입력 데이터와 출력 결과는 종종 클래스의 모든 구성원이 관련된 다른 클래스로 분류됩니다.
<br>

- 각 클래스는 프로그램이 각 클래스 멤버에 대해 동등한 방식으로 동작하는 동등성 파티션 또는 도메인입니다.
<br>

- 테스트 사례는 각 파티션에서 선택해야 합니다.
<br>

#### 등가 분할
![캡처](https://i.imgur.com/ohTirjV.png)
<br>

#### 동치 파티션
![캡처](https://i.imgur.com/9z2pNaa.png)
<br>

### ✅ Testing guidelines (sequences) (테스트 순서 가이드)
<br>

- 단일 값만 있는 시퀀스로 소프트웨어를 테스트합니다.
<br>

- 크기가 다른 시퀀스를 다른 테스트에 사용합니다.
<br>

- 시퀀스의 첫 번째, 중간 및 마지막 요소에 액세스할 수 있도록 테스트를 도출합니다.
<br>

- 길이가 0인 시퀀스로 테스트합니다.
<br>

### ✅ General testing guidelines (일반 테스트 지침)
<br>

- 시스템이 모든 오류 메시지를 생성하도록 강제하는 입력 선택
<br>

- 입력 버퍼를 오버플로시키는 입력 설계
<br>

- 동일한 입력 또는 일련의 입력을 여러 번 반복합니다.
<br>

- 잘못된 출력이 강제로 생성되도록 함
<br>

- 계산 결과가 너무 크거나 너무 작도록 합니다.
<br>
---

### ✅ Component testing (구성 요소 테스트)
<br>

- 소프트웨어 구성 요소는 종종 여러 상호 작용하는 개체로 구성된 복합 구성 요소입니다.
  - 예를 들어, 기상 관측소 시스템에서 재구성 구성요소는 재구성의 각 측면을 다루는 객체를 포함한다.
<br>

- 정의된 구성 요소 인터페이스를 통해 이러한 개체의 기능에 액세스할 수 있습니다.
<br>

- 따라서 복합 구성품 시험은 구성품 인터페이스가 사양에 따라 작동함을 보여주는 데 중점을 두어야 한다.
  - 부품 내 개별 물체에 대한 단위 시험이 완료되었다고 가정할 수 있습니다.
<br>

### ✅ Interface testing (인터페이스 테스트)
<br>

- 인터페이스 오류 또는 인터페이스에 대한 잘못된 가정으로 인한 결함을 탐지하는 것이 목표입니다.
<br>

- 인터페이스 유형
  - 매개 변수 인터페이스 한 방법 또는 절차에서 다른 방법으로 전달된 데이터입니다.
  - 공유 메모리 인터페이스 메모리의 블록은 절차 또는 기능 간에 공유됩니다.
  - 절차 인터페이스 하위 시스템은 다른 하위 시스템에서 호출할 절차 집합을 캡슐화합니다.
  - 메시지 전달 인터페이스 하위 시스템이 다른 하위 시스템에서 서비스를 요청합니다.
<br>

#### 인터페이스 테스트 일반 모델
![캡처](https://i.imgur.com/kFY1Tdq.png)
<br>

### ✅ Interface errors (인터페이스 오류)
<br>

- 인터페이스 오용
  - 호출하는 구성 요소가 다른 구성 요소를 호출하고 인터페이스를 사용할 때 잘못된 순서로 매개 변수 등의 오류를 발생시킵니다.
<br>

- 인터페이스 오해
  - 호출 구성 요소에는 호출된 구성 요소의 동작에 대한 잘못된 가정이 포함되어 있습니다.
<br>

- 타이밍 오류
  - 호출된 구성 요소와 호출된 구성 요소는 서로 다른 속도로 작동하며 오래된 정보에 액세스합니다.
<br>

### ✅ Interface testing guidelines (인터페이스 테스트 지침)
<br>

- 호출된 절차의 모수가 해당 범위의 끝단에 있도록 설계 검정을 수행합니다.
<br>

- 항상 null 포인터로 포인터 매개 변수를 테스트합니다.
<br>

- 구성 요소의 고장을 일으키는 설계 테스트입니다.
<br>

- 메시지 전달 시스템에서 스트레스 테스트를 사용합니다.
<br>

- 공유 메모리 시스템에서 구성 요소가 활성화되는 순서를 변경합니다.
<br>

### ✅ System testing (시스템 테스트)
<br>

- 개발 중 시스템 테스트는 시스템 버전을 만들기 위해 구성 요소를 통합한 다음 통합 시스템을 테스트하는 것을 포함한다.
<br>

- 시스템 테스트의 초점은 구성 요소 간의 상호 작용을 테스트하는 것입니다.
<br>

- 시스템 테스트에서는 구성 요소가 호환되고 올바르게 상호 작용하며 적절한 시간에 인터페이스를 통해 올바른 데이터를 전송하는지 확인합니다.
<br>

- 시스템 테스트는 시스템의 출현 동작을 테스트합니다.
<br>

### ✅ System and component testing (시스템 및 구성 요소 테스트)
<br>

- 시스템 테스트 중에 별도로 개발된 재사용 가능한 구성 요소와 기성 시스템이 새로 개발된 구성 요소를 통합할 수 있습니다.
그런 다음 전체 시스템을 테스트합니다.
<br>

- 다른 팀 구성원 또는 하위 팀이 개발한 구성 요소는 이 단계에서 통합될 수 있습니다. 시스템 테스트는 개별 프로세스가 아닌 집합적인 프로세스입니다.
  - 일부 회사에서는 설계자 및 프로그래머의 개입 없이 별도의 테스트 팀이 시스템 테스트에 참여할 수 있습니다.
<br>

### ✅ Use-case testing (사용 사례 테스트)
<br>

- 시스템 상호작용을 식별하기 위해 개발된 사용 사례는 시스템 테스트의 기준으로 사용될 수 있다.
<br>

- 각 사용 사례에는 일반적으로 여러 시스템 구성 요소가 포함되므로 사용 사례를 테스트하면 이러한 상호 작용이 발생합니다.
<br>

- 사용 사례와 관련된 시퀀스 다이어그램은 테스트 중인 구성 요소와 상호작용을 문서화합니다.
<br>

#### 예시 : 날씨 데이터 수집 Use-case에 대한 시퀀스 차트
![캡처](https://i.imgur.com/CEdQODo.png)
<br>

### ✅ Test cases derived from sequence diagram (시퀀스 다이어그램에서 파생된 테스트 사례)
<br>

- 보고서에 대한 요청의 입력에는 관련 승인이 있어야 한다. 보고서는 궁극적으로 요청에서 반환되어야 한다.
  - 보고서가 올바르게 구성되었는지 확인하는 데 사용할 수 있는 요약 데이터를 생성해야 합니다.
<br>

- WeatherStation에 대한 보고서를 입력 요청하면 요약 보고서가 생성됩니다.
  - SatComm 테스트를 위해 준비한 요약에 해당하는 원시 데이터를 생성하고 WeatherStation 개체가 이 요약을 올바르게 생성하는지 확인하여 테스트할 수 있습니다. 이 원시 데이터는 WeatherData 객체를 테스트하는 데도 사용됩니다.
<br>

### ✅ Testing policies (테스트 정책)
<br>

- 철저한 시스템 테스트는 불가능하므로 필요한 시스템 테스트 범위를 정의하는 테스트 정책이 개발될 수 있습니다.
<br>

- 테스트 정책의 예:
  - 메뉴를 통해 액세스하는 모든 시스템 기능을 테스트해야 합니다.
  - 동일한 메뉴를 통해 액세스하는 기능(예: 텍스트 형식 지정)의 조합을 테스트해야 합니다.
  - 사용자 입력이 제공되는 경우 모든 기능을 올바른 입력과 잘못된 입력으로 테스트해야 합니다.
<br>
