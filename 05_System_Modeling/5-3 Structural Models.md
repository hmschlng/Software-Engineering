# 🍎 5-3 Structural Models
---
<br>

### ✅ Structural models
- 소프트웨어의 구조 모델은 시스템을 구성하는 컴포넌트와 그 관계를 기준으로 시스템의 구성을 표시합니다.
<br>

- 구조 모델은 시스템 설계의 구조를 보여주는 정적 모델 또는 시스템이 실행될 때 시스템의 구성을 보여주는 동적 모델일 수 있습니다.
<br>

- 시스템 아키텍처를 논의하고 설계할 때 시스템의 구조 모델을 만듭니다.
<br>


### ✅ Class diagrams
- 클래스 다이어그램은 객체 지향 시스템 모델을 개발할 때 시스템의 클래스와 이러한 클래스 간의 연결을 보여주는 데 사용됩니다.
<br>

- 객체 클래스는 하나의 시스템 객체의 일반적인 정의로 생각할 수 있다.
<br>

- 연결은 클래스 사이에 관계가 있음을 나타내는 클래스 간의 링크입니다.
<br>

- 소프트웨어 엔지니어링 프로세스의 초기 단계에서 모델을 개발할 때의 객체는 환자, 처방전, 의사 등과 같은 실제 세계에서 무언가를 나타냅니다.
<br>

#### Mentcare 예시 : UML 클래스와 그 연결 (1:1 관계)
![1](https://i.imgur.com/mJdcLU7.png)
<br>

#### Mentcare 예시 : MHC-PMS에서의 UML 클래스와 그 연결
![1](https://i.imgur.com/HCz34kH.png)
<br>

#### Mentcare 예시 : The Consultation class
![1](https://i.imgur.com/DvfJenF.png)

필드 -> Properties
메소드 -> Operations
<br>

### ✅ Generalization (일반화)
- 일반화는 우리가 복잡성을 관리하기 위해 사용하는 일상적인 기술입니다.
<br>

- 우리가 경험하는 모든 실체의 자세한 특성을 배우기보다는 이러한 실체를 보다 일반적인 클래스(동물, 자동차, 집 등)에 배치하고 이러한 클래스의 특성을 학습합니다.
<br>

- 이를 통해 다람쥐와 쥐가 설치류인 것과 같은 이 분류의 다른 구성원들이 몇 가지 공통적인 특징을 가지고 있다는 것을 추론할 수 있습니다. (클래스 상속)
<br>

- 모델링 시스템에서 일반화를 위한 범위가 있는지 확인하기 위해 시스템의 클래스를 검사하는 것이 종종 유용합니다. 변경사항이 제안되면 시스템의 모든 클래스를 확인하여 변경사항이 영향을 받는지 확인할 필요가 없습니다.
<br>

- 자바와 같은 객체 지향 언어에서 일반화는 언어에 내장된 클래스 상속 메커니즘을 사용하여 구현됩니다.
<br>

- 일반화에서, 상위 레벨 클래스와 관련된 특성과 동작은 하위 레벨 클래스와도 연관됩니다.
<br>

- 하위 레벨 클래스는 슈퍼 클래스에서 특성과 동작을 상속하는 서브클래스입니다. 하위 레벨 클래스는 이러한 슈퍼 클래스의 특성과 동작을 상속한 다음, 더 구체적인 특성과 동작을 추가합니다.
<br>

#### A generalization hierarchy
![1](https://i.imgur.com/FMvJ8BA.png)
<br>

#### A generalization hierarchy with added detail
![1](https://i.imgur.com/5WUX7I8.png)
<br>

#### Object class aggregation models
- 집계 모델은 집합인 클래스가 다른 클래스로 구성되는 방식을 보여줍니다.
<br>

- 집계 모델은 의미 데이터 모델의 부분 관계와 유사합니다.
<br>

### ✅ The aggregation association
![1](https://i.imgur.com/K6J0OkT.png)
<br>

### ✅ Object aggregation
![1](https://i.imgur.com/Xq7xgDe.png)
<br>

