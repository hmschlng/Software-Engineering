# 9-1 Evolution Processes
---

<br>

### ✅ Evolution processes (소프트웨어 진화 프로세스)

- 소프트웨어 진화 과정은 다음에 따라 달라집니다.
  - 소프트웨어의 유형
  - 사용된 개발 프로세스
  - 관련된 사람들의 기술, 경험 수준
<br>

- 시스템 진화는 변화에 대한 제안, 즉 **수정안을 바탕으로 진행**됩니다.
  - 수정안에는 변경의 영향을 받는 구성요소들에 대한 설명이 있어야 하며, 이로 하여금 변경하는 데 **소요되는 비용과 변화의 영향을 추정**할 수 있어야 합니다.
<br>

- **변경사항을 확인하고, 진화시키는 작업은 시스템 수명주기 동안 계속 진행됩니다.**
<br>

#### 변경사항 식별과 진화 프로세스
![캡처](https://i.imgur.com/oUfwYxy.png)
그림을 통해 소프트웨어의 변경사항을 확인하고 진화시키는 프로세스에 대해 설명하겠습니다. 먼저 새로운 시스템(New System)이 있으면, 그 시스템의 변경 사항을 확인하는 절차(Change Identidication Proc.)를 거치고, 그것을 바탕으로 수정안(Change Proposal)을 제시합니다. 

이러한 작업이 다 끝난 이후에 비로소 소프트웨어 진화 과정(SW Evolution Proc.)에 들어가게 됩니다.
<br>

#### 소프트웨어 진화 과정
![캡처](https://i.imgur.com/vhEZBJu.png)

소프트웨어 진화의 전체 과정을 그림으로 나타낸 것입니다. 먼저 수정 제안이 들어오면(Change Requests) 그를 바탕으로 영향 분석을 거치고(Impact Analysis), 배포 계획을 세웁니다(Release Planning). 

배포 계획을 수립할 땐 오류 복구(Fault Repair), 플랫폼 적응(Platform Adaptation), 시스템 향상(System Enhancement) 작업을 합니다.

배포 계획을 세운 다음엔 소프트웨어의 구현 내용을 본격적으로 바꿉니다. 만약 계획에 변경이 필요할 때는 배포 계획을 다시 짜기도 합니다.

소프트웨어 구현이 변경 완료되면 시스템의 새 버전을 배포합니다. 그러나 새로운 수정안이 생기면 다시 수정 제안 - 영향 분석 - 배포 계획 - 구현 변경 - 배포의 과정을 반복합니다.
<br>

#### 구현 변경

소프트웨어 진화 과정에서, 구현 변경(Change Implementation) 절차는 아래 그림과 같습니다.

![캡처](https://i.imgur.com/0lsHDgr.png)

- 구현 변경은 마치 소프트웨어를 초기 개발할 때처럼, 시스템에 대해 제안된 수정사항이 설계, 구현 및 테스트되는 과정을 반복합니다.
<br>

- 하지만 구현 변경과 소프트웨어 개발에는 차이가 있습니다. 중요한 차이점은 변경 구현의 첫 번째 단계에서는, 특히 시스템을 개발한 원래 개발자가 유지보수/확장에 대한 책임을 지지 않고 다른 사람이 소프트웨어 진화 프로세스를 진행하는 경우, 구현 내용을 변경하기 전에 먼저 전체 프로그램에 대해 이해하는 과정이 있어야 한다는 것입니다.
<br>

- 프로그램 이해 단계에서는 프로그램의 구조와 기능 제공 방법을 차악하고, 제안된 변경 사항이 프로그램에 어떤 영향을 미칠 수 있는지 이해해야만 합니다.
<br>

### ✅ Urgent change requests (긴급 변경 요청)

- 한편, 상황에 따라서는 소프트웨어를 긴급하게 변경햐야하는 상황이 발생할 수 있습니다. 긴급 변경이 필요한 상황은 다음과 같습니다.
  - 정상 작동을 계속하기 위해 심각한 시스템 고장을 수리해야 하는 경우
  - 시스템 환경 변경(예: OS 업그레이드)이 예상치 못한 영향을 미치는 경우
  - 매우 신속한 대응이 필요한 비즈니스 변화가 있는 경우(예: 경쟁 제품 출시)
<br>

- 이때는 소프트웨어 엔지니어링 프로세스의 모든 단계를 거치지 않고 긴급한 변경이 구현되어야 할 수 있습니다.

#### 비상 복구 프로세스
긴급 수정이 필요한 상황에서의 작업 과정은 다음 그림과 같습니다.

![캡처](https://i.imgur.com/dk6kD7m.png)

이러한 경우에는 수정사항이 나오면(Change Requests), 바로 코드 분석을 시작하고(Analyze Source Code), 바로 코드를 수정합니다(Modify Source Code). 그리고 수정된 코드를 바로 시스템에 전달합니다(Deliver Modified System).
<br>

### ✅ Agile methods and evolution (애자일 방법에서의 SW 진화)
- 애자일 개발 방법은 점진적인 개발을 기반으로 하므로 개발에서 진화로의 전환이 원활한 편입니다.
  - 진화는 빈번한 시스템 릴리스를 기반으로 한 개발 프로세스의 연속일 뿐입니다.
<br>

- 자동화된 회귀 테스트는 시스템을 변경할 때 특히 중요합니다.
<br>

- 변경 사항은 추가 사용자 이야기로 표현될 수 있다.
<br>

### ✅ Handover problems (이양 관련 문제)
개발팀과 진화 팀은 종종 다를 수 있습니다. 이럴 땐 소프트웨어 수정에 대한 이양 절차가 진행되는데, 이 때 발생할 수 있는 문제들은 다음과 같습니다.

- 예를 들어 개발 팀은 애자일 기법을 사용했지만, 진화 팀은 애자일 방법에 익숙하지 않고 PDD(계획기반개발) 방식을 선호합니다.
  - 이런 경우, 진화 팀은 진화를 뒷받침할 상세한 문서를 예상할 수 있는데, 이는 애자일 프로세스에서는 만들지 않는 것입니다.
<br>

- 개발팀은 PDD 사용하였지만 진화 팀은 애자일 방법을 사용하는 것을 선호합니다.
  - 진화 팀은 자동화 테스트를 처음부터 개발해야 할 수 있으며, 시스템의 코드가 애자일 개발에서 예상한 대로 리팩터링되거나 단순화되지 않았을 수 있습니다.
<br>