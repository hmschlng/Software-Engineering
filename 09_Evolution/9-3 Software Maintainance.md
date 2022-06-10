# 9-3 Software Maintainance
---

<br>

### ✅ Software maintenance (소프트웨어 유지보수)

소프트웨어 유지보수는 프로그램이 사용되기 시작한 후 프로그램 을 수정하는 것을 의미합니다. 

Maintenance 라는 말은 대부분 사용자 지정 소프트웨어를 변경하는 경우에 주로 사용되는 용어입니다. 일반 소프트웨어 제품의 경우, 새로운 버전을 만들기 위해 진화한다고 한다.

유지보수는 일반적으로 시스템 아키텍처의 큰 변경을 수반하지 않는 변경을 의미합니다. 유지보수 작업을 할 때는 보통 기존 컴포넌트 내용을 수정하고, 시스템에 새 컴포넌트를 추가하는 등의 작업을 합니다.
<br>

#### 유지보수의 종류
- 고장 수리
  - 시스템을 변경하여 버그/장애를 해결하고, 요구사항이 충족되는 방향으로 결점을 보완합니다.
<br>

- 환경 적응
  - 소프트웨어를 다른 작동 환경에 적응시키기 위한 유지보수입니다.
  - 시스템을 초기 구현과 다른 환경(컴퓨터, OS 등)에서 작동하도록 변경합니다.
<br>

- 기능 추가 및 수정
  - 새로운 요구 사항을 충족하도록 시스템을 수정합니다.
<br>

#### 유지보수 작업의 분포
![캡처](https://i.imgur.com/48WlKHn.png)
<br>

### ✅ Maintenance costs (유지보수비용)
<br>

- 유지보수비용은 일반적으로 개발 비용보다 큽니다 (애플리케이션에 따라 2 ~ 100배).
<br>

- 기술적 요인 및 비기술적 요인 모두에 영향을 받습니다.
<br>

- 소프트웨어가 유지 관리될수록 증가합니다.
유지보수는 소프트웨어 구조를 손상시키므로 유지보수는 점점 어려워집니다.
<br>

- 노후화된 소프트웨어는 지원 비용이 높을 수 있습니다(예: 오래된 언어, 컴파일러 등).
<br>

일반적으로 개발 중에 동일한 기능을 추가하는 것보다 유지보수 중에 시스템에 새로운 기능을 추가하는 것이 더 비쌉니다.
- 새로운 팀은 유지 관리 중인 프로그램을 이해해야 합니다.
<br>

- 유지 관리 및 개발을 분리한다는 것은 개발 팀이 유지 관리 가능한 소프트웨어를 작성할 동기가 없음을 의미합니다.
<br>

- 프로그램 유지보수쪽 분야가 인기가 없습니다. 때문에 유지보수 작업자의 경험이 부족하고 도메인 지식이 제한적인 경우가 많습니다.
<br>

- 프로그램이 노후화되면 구조가 저하되고 변경하기 어려워집니다.
<br>

---

### ✅ Maintenance prediction (유지보수 예측)
![캡처](https://i.imgur.com/chwh74i.png)

유지 보수 예측은 시스템의 어느 부분이 문제를 일으킬 수 있고 유지 보수 비용이 높은지 평가하는 것과 관련이 있습니다.
  - 변경 허용 여부는 변경의 영향을 받는 구성 요소의 유지관리 가능성에 따라 달라집니다.
  - 변경을 시행하면 시스템이 저하되고 유지보수성이 저하됩니다.
  - 유지보수 비용은 변경 횟수에 따라 달라지며, 변경 비용은 유지보수 가능성에 따라 달라짐
<br>

### ✅ Change prediction (변화 예측)

- 변경 예측은 시스템과 현재 환경 사이의 관계를 이해하고, 필요한 변경의 수를 예측하는 것입니다.
<br>

- 긴밀하게 연결된 시스템은 환경이 변경될 때마다 변화가 필요합니다.
<br>

- 시스템과 환경 간의 관계에 영향을 미치는 요인은 다음과 같습니다. 
  - 시스템 인터페이스의 수와 그 **복잡도**
  - 본질적으로 불안정한 시스템 요구사항의 수
  - 시스템이 사용되는 비즈니스 **프로세스**의 수
<br>

#### 복잡도 측정 기준

- 유지보수 가능성에 대한 예측은 시스템 컴포넌트의 복잡성을 평가함으로써 이루어질 수 있습니다.
<br>

- 연구에 따르면, 대부분의 유지보수 작업은 비교적 적은 수의 시스템 컴포넌트에 소비됩니다.
<br>

- 복잡성을 결정하는 요소는 다음과 같습니다.
  - 제어 구조(control structures)의 복잡성
  - 데이터 구조(data structures)의 복잡성
  - 객체, 메소드(procedure), 모듈 등의 크기.
<br>

#### 프로세스 측정 기준
<br>

- 유지보수성 평가의 근거로 프로세스 측정을 사용할 수 있습니다. 프로세스 측정의 기준은 다음과 같습니다.
  - 수리, 복구 등 시정 관련 유지보수 요청의 건수
  - 충격 분석에 필요한 평균 시간
  - 변경 요청 구현에 소요되는 평균 시간
  - 아직 해결되지 않은 변경 요청의 수
<br>

- 이 중 하나라도 증가하고 있는 경우 유지관리성이 저하될 수 있다는 뜻입니다.
<br>

### ✅ Software reengineering (소프트웨어 재설계)
소프트웨어 재설계는 기능을 변경하지 않고 레거시 시스템의 일부 또는 전부를 재구성하거나 다시 쓴다는 뜻입니다.

재설계는 보통 대형 시스템의 일부 하위 시스템에 빈번한 유지보수가 필요한 경우에 진행됩니다.

리엔지니어링은 유지보수를 더 쉽게 하기 위한 노동력을 추가하는 것입니다. 시스템을 재구성하고 다시 문서화할 것입니다.
<br>

#### 리엔지니어링의 이점

- **리스크 감소**
  - 아예 새로운 소프트웨어를 개발하는 것은 리스크가 큰 작업입니다. 개발 문제, 인력 문제 및 사양 문제가 있을 수 있습니다.
  - 재설계는 이런 관점에서 리스크가 덜합니다.
<br>

- **비용 절감**
  - 리엔지니어링은 대개 새로운 소프트웨어 개발보다 비용적으로 훨씬 저렴합니다.
<br>

#### 리엔지니어링 과정
![캡처](https://i.imgur.com/QpErUAC.png)
<br>

- **소스 코드 변환** (Source code translation)
  - 코드를 새로운 언어로 변환합니다.
<br>

- **리버스 엔지니어링** (Reverse engineering)
  - 프로그램을 분석하여 이해합니다.
<br>

- **프로그램 구조 개선** (Program structure improvement)
  - 이해가능성을 위해 자동으로 재구성합니다.
<br>

- **프로그램 모듈화** (Program modularisation)
  - 프로그램 구조를 개편합니다.
<br>

- **데이터 리엔지니어링** (Data reengineering)
  - 시스템 데이터를 정리하고 재구성합니다.
<br>

#### 리엔지니어링 접근 방식
![캡처](https://i.imgur.com/GHcrXk4.png)
<br>

#### 리엔지니어링 비용 요인

- 재설계할 소프트웨어의 품질
<br>

- 리엔지니어링에 사용 가능한 도구 지원 수준
<br>

- 필요한 데이터 변환의 범위
<br>

- 리엔지니어링을 위한 전문 인력 확보
  - 이는 더 이상 널리 사용되지 않는 기술 기반의 오래된 시스템에서 문제가 될 수 있습니다.
<br>

### ✅ Refactoring (리팩터링)
- 리팩터링(refactoring)은 프로그램을 개선하여, 변경을 통한 성능 저하를 늦추는 과정입니다.
<br>

- 리팩터링은 미래 변화의 문제점을 줄여주는 '예방적 정비'라고 볼 수 있습니다.
<br>

- 리팩터링은 프로그램의 구조를 개선하거나, 복잡성을 줄이거나, 이해하기 쉽게 하기 위해 프로그램을 수정하는 것을 포함합니다.
<br>

- 프로그램을 리팩터링할 때는 기능을 추가하지 말고 프로그램 개선에 집중해야 합니다.
<br>

#### 리팩터링과 리엔지니어링의 비교
- **재설계는 시스템이 이미 몇번 유지된 상태이고, 유지보수 비용이 점점 증가하고 있을 때 진행합니다.** 
  자동화 툴을 사용하여 기존 시스템을 처리하거나 재설계하여 보다 유지 관리가 용이한 새 시스템을 만들 수 있습니다.
<br>

- **리팩토링은 개발 및 진화 과정 전반에 걸쳐 지속적으로 진행합니다.** 
  시스템의 유지보수 비용과 유지보수 난이도를 증가시키는 시스템 구조와 코드 저하 등을 예방하기 위한 작업입니다.
<br>

#### 리팩토링 대상 - 프로그램 코드의 '악취'
<br>

- 중복된 코드 (Duplicated code)
  - 동일하거나 매우 유사한 코드가 프로그램의 다른 위치에 포함되는 경우입니다. 이런 중복코드는 하나의 메서드로 구현하여 필요에 따라 호출되는 형태로 리팩터링할 수 있습니다.
<br>

- 너무 긴 메소드
  - 너무 긴 메소드는 다수의 짧은 방법으로 재설계하는 것이 좋습니다.
<br>

- Switch - Case 문
  - switch-case 문이 값의 유형에 따라 달라지는 경우, 중복이 포함되는 경우가 많습니다. 객체 지향 언어를 사용한다면, 프로그램 곳곳에 뿌려진 switch-case문들을 다형성 구조로 리팩터링해서 관리할 수 있습니다.
<br>

- 데이터 군집
  - 데이터 덩어리는 프로그램의 여러 위치에서 동일한 데이터 항목 그룹(클래스의 필드, 메서드의 매개 변수)이 다시 발생할 때 발생합니다. 이러한 개체는 종종 모든 데이터를 캡슐화하는 오브젝트로 대체할 수 있습니다.
<br>

- 추측에 근거한 일반성
  - 미래에 필요할 경우를 대비해 개발자가 프로그램에 일반성을 포함시킬 때 발생한다. 이것은 종종 간단히 제거할 수 있다.
<br>