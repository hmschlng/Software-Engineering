# 21-2 Architectural Patterns for Real-time Software
---

<br>

### ✅ Architectural patterns for embedded systems (임베디드 시스템의 아키텍처 패턴)
<br>

- 임베디드 시스템의 특성 시스템 아키텍처
  - 관찰 및 대응 이 패턴은 일련의 센서를 정기적으로 모니터링하고 표시할 때 사용됩니다.
  - 환경 제어 이 패턴은 환경에 대한 정보를 제공하는 센서와 환경을 변화시킬 수 있는 액추에이터를 포함하는 시스템에 사용되는 패턴입니다.
  - 프로세스 파이프라인 이 패턴은 데이터를 처리하기 전에 한 표현에서 다른 표현으로 변환해야 할 때 사용됩니다.
<br>

### ✅ The Observe and React pattern (관찰 및 반응 패턴)
![캡처](https://i.imgur.com/nFiaoZB.png)
<br>

#### 관찰 및 반응 패턴 프로세스의 구조
![캡처](https://i.imgur.com/ezxLyGB.png)
<br>

#### 경보 시스템 설명
소프트웨어 시스템은 상업용 건물에 대한 도난 경보 시스템의 일부로 구현될 것이다. 여기에는 여러 가지 다른 유형의 센서가 사용됩니다. 여기에는 개별 룸의 이동 감지기, 복도 문이 열리는 것을 감지하는 도어 센서, 창문이 열린 때를 감지하는 1층 창의 윈도우 센서가 포함됩니다.
센서가 침입자의 존재를 감지하면 시스템은 자동으로 지역 경찰을 부르고 음성 합성기를 사용하여 경보의 위치를 보고합니다. 활성 센서 주변의 실내 조명을 켜고 가청 알람을 울립니다. 센서 시스템은 일반적으로 주 전원으로 작동하지만 배터리 백업이 장착되어 있습니다. 전원 손실은 주 전압을 모니터링하는 별도의 전원 회로 모니터를 사용하여 감지됩니다. 전압 강하가 감지되면 시스템은 침입자가 전원 공급을 중단했다고 가정하여 경보가 발생합니다.
<br>

#### 도난경보시스템 프로세스 구조
![캡처](https://i.imgur.com/HUlhEAB.png)
<br>

### ✅ The Environmental Control pattern (환경 제어 패턴)
![캡처](https://i.imgur.com/PtT5rDa.png)
<br>

#### 환경 제어 프로세스 구조
![캡처](https://i.imgur.com/6fXyaIh.png)
<br>

#### 미끄럼 방지 제동 시스템의 제어 시스템 아키텍처
![캡처](https://i.imgur.com/kMlgLbQ.png)
<br>

### ✅ The Process Pipeline pattern (프로세스 파이프라인 패턴)
![캡처](https://i.imgur.com/ioQD536.png)
<br>

#### 프로세스 파이프라인 프로세스 구조
![캡처](https://i.imgur.com/cXLBj9a.png)
<br>

#### 중성자속 데이터 수집
![캡처](https://i.imgur.com/vawbX83.png)
<br>


