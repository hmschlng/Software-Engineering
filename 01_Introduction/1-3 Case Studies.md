# 🍎 Case Studies
---
<br>

### ✅ Case Studies (사례 연구)
#### 사례 1 : 개인용 인슐린 펌프
- 혈당 조절을 유지하기 위해 당뇨병 환자가 사용하는 인슐린 펌프에 내장된 시스템.
<br>

#### 사례 2 : 정신 건강 환자 관리 시스템 (Mentcare)
- 정신 건강 문제에 대한 치료를 받는 사람들의 기록을 유지하는 데 사용되는 시스템.
<br>

#### 사례 3 : 황야 기상 관측소
- 오지의 기상 정보를 수집하는 데이터 수집 시스템.
<br>

#### 사례 4 : 디지털 학습 환경 (iLearn)
 - 학교에서 학습을 지원하는 시스템
<br>


### ✅ Case 1 - Insulin Pump Control System (hereinafter, IPCS)
> <br>
> 
> - 혈당 센서에서 데이터를 수집하고 주입해야 하는 인슐린 양을 계산합니다.
> 
> <br>
> 
> - 혈당 수치의 변화율을 기준으로 계산합니다.
> 
> <br>
> 
> - 마이크로 펌프에 신호를 보내 정확한 인슐린 용량을 전달합니다.
> 
> <br>
> 
> - 저혈당이 뇌 기능 장애, 혼수 상태 및 사망으로 이어질 수 있으므로 안전이 중요한 시스템입니다. 또한 고혈당 수치는 눈과 신장 손상과 같은 장기적인 결과를 초래합니다..
> 
> <br>

<br>

#### Hardware Architecture of IPCS (IPCS의 하드웨어 구조)
![1](https://i.imgur.com/ziG7DRl.png)
출처 : 『Software Engineering 9th Edition』 by	Ian Sommerville (published by Addison-Wesley)
<br>

#### Activity Model of the IPCS (IPCS의 동작모델)
![1](https://i.imgur.com/0SGC25z.png)
출처 : 『Software Engineering 9th Edition』 by	Ian Sommerville (published by Addison-Wesley)
<br>

#### Essential High - Level Requirements (필수 상위 수준 요구 사항)
- 시스템은 필요할 때 인슐린을 전달할 수 있어야 합니다.
<br>

- 시스템이 안정적으로 작동하고 현재 혈당 수준에 대응하기 위해 정확한 양의 인슐린을 전달해야 합니다.
<br>

- 따라서 시스템이 항상 이러한 요구 사항을 충족할 수 있도록 시스템을 설계하고 구현해야 합니다.
<br>


### ✅ Case 2 - A Patient Information System for Mental Health Care 
> <br>
> 
> **정신건강관리 지원 환자정보시스템, Mentcare**는 정신건강문제로 고통받는 환자와 그들이 받은 치료에 대한 정보를 보존하는 의료정보시스템입니다.
>
> <br>
> 
> 대부분의 정신 건강 환자는 전담 병원 치료가 필요하지 않지만 문제에 대해 자세히 알고 있는 의사를 만날 수 있는 전문 클리닉을 정기적으로 방문해야 합니다.
> 
> <br>
> 
> 이러한 클리닉은 환자가 쉽게 방문할 수 있도록 병원에서만 운영되는 것이 아닙니다. 또한 지역 의료 관행이나 커뮤니티 센터에서 진행될 수도 있습니다.
> 
> <br>

<br>

#### Mentcare
> <br>
> 
> - Mentcare는 진료소에서 사용하기 위한 정보 시스템입니다.
>
> <br>
> 
> - 중앙 집중화된 환자 정보 데이터베이스를 사용하지만 PC에서도 실행되도록 설계되어 네트워크 연결이 안정적이지 않은 상황에서도 사이트에 액세스하여 사용할 수 있습니다.
> 
> <br>
> 
> - 로컬 시스템에 보안 네트워크 액세스가 있는 경우 데이터베이스의 환자 정보를 사용하지만, 만약 연결이 끊긴 경우엔 환자 기록의 로컬 복사본을 다운로드하여 사용할 수 있습니다.
> 
> <br>

<br>

#### Goals of Mentcare (Mentcare의 목표)
- 의료 서비스 관리자가 지방 및 정부 목표에 대한 성과를 평가할 수 있도록 하는 관리 정보를 생성합니다.
<br>

- 환자의 치료를 지원하기 위해 의료진에게 시기적절한 정보를 제공합니다.
<br>

#### The Organization of the Mentcare System (Mentcare 시스템 구조)
![1](https://i.imgur.com/WznFONL.png)
출처 : 『Software Engineering 9th Edition』 by	Ian Sommerville (published by Addison-Wesley)
<br>

#### Key Features of the Mentcare System (Mentcare 시스템의 핵심 기능)
- **개별 케어 관리**
  - 임상의는 환자에 대한 기록을 작성하고, 시스템의 정보를 편집하고, 환자 이력을 보는 등을 할 수 있습니다. 시스템은 데이터 요약을 지원하므로 의사는 처방된 주요 문제 및 치료에 대해 빠르게 배울 수 있습니다.
<br>

- **환자 모니터링**
  - 시스템은 치료에 관련된 환자의 기록을 모니터링하고 가능한 문제가 감지되면 경고를 발행합니다.
<br>

- **행정보고**
  - 시스템은 각 클리닉에서 치료한 환자 수, 요양 시스템에 입/퇴원한 환자 수, 분할된 환자 수, 처방된 약물 및 비용 등을 보여주는 월간 관리 보고서를 생성합니다.

<br>

#### Mencare System Concerns.. (Mentcare 시스템의 고려사항)
- **개인정보 보호**
  - 환자 정보는 기밀로 유지되어야 하며 승인된 의료진과 환자 자신 외에는 절대 공개되지 않습니다.
<br>

- **안전**
  - 일부 정신 질환은 환자로 하여금 자살 충동을 일으키거나 다른 사람들에게 위험을 초래합니다. 가능한 한 시스템은 잠재적으로 자살하거나 위험한 환자에 대해 의료진에게 경고해야 합니다.
  - 시스템은 필요할 때 사용할 수 있어야 합니다. 그렇지 않으면 안전이 손상될 수 있고 환자에게 올바른 약을 처방하는 것이 불가능할 수 있습니다.
<br>


### ✅ Case 3 - Wilderness Weather Station

> <br>
> 
> 광야 지역이 넓은 국가의 정부는 외딴 지역에 수백 개의 기상 관측소를 배치하기로 결정합니다.
>
> <br>
> 
> 기상 관측소는 온도와 기압, 일조량, 강우량, 풍속 및 풍향을 측정하는 일련의 장비에서 데이터를 수집합니다.
> - 기상 관측소에는 풍속 및 풍향, 지면 및 대기 온도, 기압 및 24시간 동안의 강우량과 같은 기상 매개변수를 측정하는 여러 도구가 포함되어 있습니다. 이러한 각 기기는 주기적으로 매개변수를 읽고 기기에서 수집된 데이터를 관리하는 소프트웨어 시스템에 의해 제어됩니다.
> 
> <br>

<br>

#### The Environment of Weather Station (기상 관측소 환경)
<img src="https://i.imgur.com/noYt1S7.png" width=450 height=300>

출처 : 『Software Engineering 9th Edition』 by	Ian Sommerville (published by Addison-Wesley)

- **기상 관측소 시스템**
  - 이것은 날씨 데이터를 수집하고 일부 초기 데이터 처리를 수행하고 데이터 관리 시스템으로 전송하는 일을 담당합니다.
<br>

- **관측소 유지 보수 시스템**
  - 이 시스템은 위성을 통해 모든 야생 기상 관측소와 통신하여 이러한 시스템의 상태를 모니터링하고 문제 보고서를 제공할 수 있습니다.
<br>

- **데이터 관리 및 보관 시스템**
  - 이 시스템은 모든 황야 기상 관측소에서 데이터를 수집하고 데이터 처리 및 분석을 수행하고 데이터를 보관합니다.
<br>


#### Additional Software Functionality (추가 소프트웨어 기능)
- 기기, 전원 및 통신 하드웨어를 모니터링하고 관리 시스템에 오류를 보고합니다.
<br>

- 시스템 전원을 관리하여 환경 조건이 허용할 때마다 배터리를 충전하고 강풍과 같이 잠재적으로 피해를 줄 수 있는 기상 조건에서 발전기를 차단합니다.
<br>

- 소프트웨어의 일부가 새 버전으로 교체되고 시스템 장애 발생 시 백업 기기가 시스템으로 전환되는 동적 재구성을 지원합니다.
<br>

### ✅ Case 4 - A Digital Learning Environment (iLearn)
> <br>
> 
> **디지털 학습 환경**은 학습을 위해 범용 및 특수 목적으로 설계된 도구들의 집합이 내장된 **프레임워크**와, 시스템을 사용하는 학습자의 요구에 맞게 조정된 또는 **응용 프로그램 세트가 합쳐진 형태**입니다.
니다.
>
> <br>
> 
> 디지털 학습 환경의 각 버전에 포함된 도구는 교사와 학습자가 특정 요구 사항에 맞게 선택합니다.
> - 도구는 스프레드시트와 같은 일반 응용 프로그램, 가상 학습 환경(VLE)과 같은 학습 관리 응용 프로그램, 숙제 제출 및 평가 관리, 게임 및 시뮬레이션이 될 수 있습니다.
> 
> <br>

<br>

#### Service-oriented System (서비스 지향 시스템)
- 이 시스템은 교체 가능한 서비스로 간주되는 모든 시스템 구성 요소가 있는 **서비스 지향 시스템**입니다.
<br>

- 이를 통해 새로운 서비스를 사용할 수 있게 되면 시스템을 점진적으로 업데이트할 수 있습니다.
<br>

- 또한 글을 읽지 못하는 아주 어린 아이, 고등학생 등과 같은 다양한 그룹을 위한 환경 버전을 생성하도록 시스템을 신속하게 구성할 수 있습니다.

<br>

#### iLearn Services (iLearn의 서비스)
- **유틸리티 서비스**
  - 기본 응용 프로그램 독립 기능을 제공하며 시스템의 다른 서비스에서 사용할 수 있습니다.
<br>

- **종합 지원 서비스**
  - 이메일, 회의, 사진 공유 등과 같은 특정 응용 프로그램을 제공하고 과학 영화 또는 역사적 자원과 같은 특정 교육 콘텐츠에 대한 액세스를 제공합니다.
<br>

- **구성 서비스**
  - 이 서비스는 특정 응용 프로그램 서비스 세트로 환경을 조정하고 학생, 교사 및 학부모 간에 서비스를 공유하는 방법을 정의하는 데 사용됩니다.
<br>

#### Architecture of iLearn
![1](https://i.imgur.com/P8szVZo.png)
출처 : 『Software Engineering 9th Edition』 by	Ian Sommerville (published by Addison-Wesley)
<br>

#### iLearn Service Integration (iLearn 서비스 통합)
- 통합 서비스는 API(응용 프로그래밍 인터페이스)를 제공하고 해당 API를 통해 다른 서비스에서 액세스할 수 있는 서비스입니다. 따라서 직접적인 서비스 간 통신이 가능합니다.
<br>

- 독립 서비스는 단순히 브라우저 인터페이스를 통해 액세스하고 다른 서비스와 독립적으로 작동하는 서비스입니다. 정보는 복사 및 붙여넣기와 같은 명시적인 사용자 작업을 통해서만 다른 서비스와 공유할 수 있습니다. 각 독립 서비스에 대해 재인증이 필요할 수 있습니다.
<br>
