# 7-2 Design Patterns
---
<br>

### ✅ Design patterns (디자인 패턴)

- 디자인 패턴은 문제와 그 해결책에 대한 추상적인 지식을 재사용하는 방법이라고 볼 수 있습니다.
<br>

- 패턴은 문제와 그 해결책에 대한 본질에 대한 설명입니다.
<br>

- 디자인 패턴은 다른 설정에서 재사용할 수 있을 만큼 충분히 추상적이어야 합니다.
<br>

- 패턴 설명은 보통 상속이나 다형성과 같은 객체 지향 개념이나 특징을 이용합니다.
<br>

### ✅ Patterns (패턴)

- 패턴과 패턴 언어는 모범 사례, 좋은 설계 및 **캡처 경험?** 을 다른 사용자가 재사용할 수 있는 방식으로 설명하는 방법입니다.
<br>

### ✅ Pattern elements (패턴의 구성 요소)

- 패턴 이름
<br>

- 문제 설명.
<br>

- 솔루션 설명.
  - 디자인 패턴의 솔루션은 설계에 대해 다양한 방법으로 적용(instantiate)할 수 있도록, 구체적인 설계가 아니라 **템플릿의 형태**를 가집니다.
<br>

- 결과
  - 패턴을 적용한 결과와 트레이드오프.
<br>

#### 예시 : 관찰자 패턴
<table>
  <tr>
    <td><b>패턴</td>
    <td><b>관찰자 패턴 (Observer Pattern)</td>
  </tr>
  <tr>
    <td>설명</td>
    <td>객체의 상태를 객체 자체에서 표시하지 않고 분리합니다. 그리고 대체 디스플레이를 통해 표시합니다. 객체 상태가 변경되면 모든 디스플레이가 자동으로 통지되고 변경 내용을 반영하도록 업데이트됩니다.</td>
  </tr>
  <tr>
    <td rowspan=2>문제 설명</td>
    <td><p>[다중 디스플레이 사용 상황]<br></p><img src = "https://i.imgur.com/94uL87r.png"></td>
  </tr>
  <tr>
    <td><p>서비스 제공 시, 우리는 그래픽이나 표 등 상태 정보 디스플레이를 여러 개 제공해야 하는 상황이 많습니다. 그러나 정보가 지정될 때 이 모든 것을 알기는 힘듭니다. 모든 대체 프레젠테이션은 상호 작용을 지원해야 하며, 상태가 변경되면 모든 디스플레이를 업데이트해야 합니다.</p>
    <p>옵저버 패턴은 이렇게 상태 정보에 대해 둘 이상의 표시 형식이 필요하고, 상태 정보를 유지하는 개체가 사용하는 특정 표시 형식에 대해 알 필요가 없는 모든 상황에서 사용할 수 있습니다.</p></td>
  </tr>
  <tr>
    <td rowspan=2>솔루션 설명</td>
    <td>
    <p>아래 UML는 두 개의 Abstract Object인 [Subject]와 [Observer], 그리고 Abstract Class를 상속하고 있는 두 개의 Concrete Object인 [ConcreteSubject]와 [ConcreteObject] 가 있습니다. 
    </p>
    <p> Abstract Class들에는 모든 상황에 적용할 수 있는 일반 작업들이 추상적으로 정의되어 있습니다. <br>
    디스플레이에 표시할 상태 정보는 [Concrete Subject]에서 관리합니다. <br>
    [Concrete Subject]는 [Subject]의 기능들을 상속하고 있기 때문에, [ConcreteObserver](디스플레이)들을 추가하거나 삭제할 수 있고, 디스플레이 상태가 변경될 때 알림을 발행할 수 있습니다.
    </p>
    <p>[ConcreteObserver]는 [ConcreteSubject]가 보내는 상태정보의 복사본을 가지고 있고, [Observer]의 Update() 인터페이스를 구현하여 이 복사본을 보조에 맞추어 유지할 수 있도록 합니다. <br>
    [ConcreteObserver]는 상태정보를 자동으로 디스플레이에 표시하고 상태가 업데이트될 때마다 변경사항을 반영합니다.</p></td>
  </tr>
  <tr>
    <td><p>[옵저버 패턴을 적용한 UML 모델]</p><img src="https://i.imgur.com/13CdB2K.png"></td>
  </tr>
  <tr>
    <td>결과</td>
    <td>옵저버 패턴에서, [Subject]는 Abstract한 [Observer]만 알고, Concrete Class들의 세부 사항은 알지 못합니다. 따라서 이 Object들 사이에는 최소한의 결합만이 존재합니다. <br>
    그러나 Concrete Object들에 대한 지식이 부족하기 때문에, 디스플레이 성능을 향상시키는 최적화는 비현실적입니다. <br>
    또한, [Subject]를 수정하면 [Observer] 또한 수정해야 할 수 있으며, 그 중 일부는 해당 [Observer]에게 필요하지 않은 업데이트일 수 있기 때문에 좋지 않습니다.</td>
  </tr>
</table>
<br>

### ✅ Design problems (디자인 문제) ❌

- 설계에 패턴을 사용하려면 현재 직면하고 있는 설계 문제에 적용할 수 있는 관련 패턴이 있을 수 있다는 점을 인식해야 합니다.
  - 다른 오브젝트의 상태가 변경되었음을 여러 오브젝트에 알립니다(Obsever pattern).
  - 인터페이스를 점진적으로 개발되는 여러 관련 개체로 정리합니다(Façade pattern).
  - 컬렉션이 구현되는 방식에 관계없이 컬렉션의 요소에 액세스하는 표준 방법을 제공합니다(Iterator pattern).
  - 실행 시 기존 클래스의 기능을 확장할 수 있습니다(Decorator pattern).
<br>
