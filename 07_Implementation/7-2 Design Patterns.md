# 7-2 Design Patterns
---
<br>

### ✅ Design patterns (디자인 패턴)

- 디자인 패턴은 문제와 그 해결책에 대한 추상적인 지식을 재사용하는 방법이다.
<br>

- 패턴은 문제와 그 해결책의 본질에 대한 설명입니다.
<br>

- 다른 설정에서 재사용할 수 있을 만큼 충분히 추상적이어야 한다.
<br>

- 패턴 설명은 일반적으로 상속이나 다형성과 같은 객체 지향 특성을 이용한다.
<br>

### ✅ Patterns (패턴)

- 패턴 및 패턴 언어는 모범 사례, 좋은 설계 및 캡처 경험을 다른 사용자가 재사용할 수 있는 방식으로 설명하는 방법입니다.
<br>

### ✅ Pattern elements (패턴 요소)

- 이름
  - 의미 있는 패턴 식별자입니다.
<br>

- 문제 설명.
<br>

- 솔루션 설명.
  - 구체적인 설계가 아니라 다양한 방법으로 인스턴스화할 수 있는 설계 솔루션의 템플릿입니다.
<br>

- 결과
  - 패턴을 적용한 결과와 트레이드오프.
<br>

### ✅ The Observer pattern (옵저버 패턴)
<table>
  <tr>
    <td><b>패턴</td>
    <td><b>관찰자 패턴 (Observer Pattern)</td>
  </tr>
  <tr>
    <td>설명</td>
    <td>개체 상태 표시를 개체 자체에서 분리하고 대체 디스플레이를 제공할 수 있습니다. 개체 상태가 변경되면 모든 디스플레이가 자동으로 통지되고 변경 내용을 반영하도록 업데이트됩니다.</td>
  </tr>
  <tr>
    <td rowspan=2>문제 설명</td>
    <td><p>[다중 디스플레이 사용 상황]<br></p><img src = "https://i.imgur.com/94uL87r.png"></td>
  </tr>
  <tr>
    <td><p>대부분의 경우 그래픽 디스플레이 및 표 형식 디스플레이와 같은 상태 정보의 디스플레이를 여러 개 제공해야 합니다. 정보가 지정될 때 이 모든 것을 알 수 있는 것은 아닙니다. 모든 대체 프레젠테이션은 상호 작용을 지원해야 하며, 상태가 변경되면 모든 디스플레이를 업데이트해야 한다.</p>
    <p>이 패턴은 상태 정보에 대해 둘 이상의 표시 형식이 필요하고 상태 정보를 유지하는 개체가 사용하는 특정 표시 형식에 대해 알 필요가 없는 모든 상황에서 사용할 수 있다.</p></td>
  </tr>
  <tr>
    <td rowspan=2>솔루션 설명</td>
    <td><p>아래 UML에는 두 개의 추상 개체인 Subject와 Observer와 두 개의 구체적인 개체인 ConcreteSubject와 ConcreteObject가 포함되며, 이는 관련된 추상 개체의 속성을 상속합니다. 추상 개체에는 모든 상황에 적용할 수 있는 일반 작업이 포함됩니다. 표시할 상태는 콘크리트 제목에서 유지되며, 이 항목은 관찰자를 추가 및 제거하고(각 관찰자는 디스플레이에 해당), 상태가 변경되었을 때 알림을 발행할 수 있도록 제목에서 연산을 상속합니다. </p>
    <p>ConcreteObserver는 ConcreteSubject의 상태 복사본을 유지하고 이러한 복사본을 보조에 맞게 유지할 수 있는 Observer 업데이트() 인터페이스를 구현합니다. ConcreteObserver는 상태를 자동으로 표시하고 상태가 업데이트될 때마다 변경사항을 반영합니다.</p></td>
  </tr>
  <tr>
    <td><p>[옵저버 패턴을 적용한 UML 모델]</p><img src="https://i.imgur.com/13CdB2K.png"></td>
  </tr>
  <tr>
    <td>결과</td>
    <td>피험자는 추상적인 관찰자만 알고 구체적인 클래스의 세부 사항은 알지 못한다. 따라서 이들 개체 사이에는 최소한의 결합이 존재한다.
이러한 지식 부족으로 인해 디스플레이 성능을 향상시키는 최적화는 비현실적이다. 주제를 변경하면 관찰자에 대한 링크된 업데이트 집합이 생성될 수 있으며, 그 중 일부는 필요하지 않을 수 있습니다.</td>
  </tr>
</table>
<br>

### ✅ Design problems (디자인 문제)

- 설계에 패턴을 사용하려면 현재 직면하고 있는 설계 문제에 적용할 수 있는 관련 패턴이 있을 수 있다는 점을 인식해야 합니다.
  - 다른 오브젝트의 상태가 변경되었음을 여러 오브젝트에 알립니다(Obsever pattern).
  - 인터페이스를 점진적으로 개발되는 여러 관련 개체로 정리합니다(Façade pattern).
  - 컬렉션이 구현되는 방식에 관계없이 컬렉션의 요소에 액세스하는 표준 방법을 제공합니다(Iterator pattern).
  - 실행 시 기존 클래스의 기능을 확장할 수 있습니다(Decorator pattern).
<br>