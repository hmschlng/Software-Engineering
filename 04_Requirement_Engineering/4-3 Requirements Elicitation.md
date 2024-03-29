# 🍎 4-3 Requirements Elicitation
---
<br>

### ✅ Requirements elicitation and analysis (요구사항 도출 및 분석)
> <br>
>
> - 요구 사항 도출 또는 요구 사항 발견이라고도 합니다.
> <br>
> 
> - 기술 직원이 고객과 협력하여 애플리케이션 도메인, 시스템이 제공해야 하는 서비스 및 시스템의 운영 제약에 대해 알아냅니다.
> <br>
> 
> - **최종 사용자, 관리자, 유지 관리에 관련된 엔지니어, 도메인 전문가, 노동 조합 등이 포함될 수 있습니다.** 이들을 이해 관계자라고 합니다.
> 
> <br>

<br>

### ✅ Requirements Elicitation (요구사항 도출)
> <br>
>
> 소프트웨어 엔지니어는 다양한 시스템 이해 관계자와 협력하여 애플리케이션 **도메인**, 시스템이 제공해야 하는 **서비스**, 필요한 **시스템 성능**, 하드웨어 **제약 조건**, 기타 시스템 등에 대해 알아봅니다.
> 
> <br>

#### 요구사항 엔지니어링 단계
- **요구 사항 발견** (Discovery),
<br>

- **요구사항 분류 및 구성** (Classification / Organization),
<br>

- **요구 사항 우선 순위 지정 및 협상** (Prioritization and Negotiation),
<br>

- **요구 사항 명세화** (Specification).
<br>

#### 👎🏼 요구사항 도출의 문제점 
- 이해관계자는 자신이 진정으로 원하는 것이 무엇인지 모릅니다.
<br>

- 이해 관계자는 요구 사항을 자신의 용어로 표현합니다.
<br>

- 이해 관계자마다 요구 사항이 상충할 수 있습니다.
<br>

- 조직적 및 정치적 요인이 시스템 요구 사항에 영향을 미칠 수 있습니다.
<br>

- 분석 과정에서 요구 사항이 변경됩니다.
<br>

- 새로운 이해관계자가 등장하고 비즈니스 환경이 바뀔 수 있습니다.
<br>


### ✅ 요구사항 도출·분석 프로세스
![1](https://i.imgur.com/jsdQkfE.png)
<br>

#### 프로세스 활동 
- **요구사항 발견** (Requirements discovery)
  - 이해 관계자와 상호 작용하여 요구 사항을 발견합니다. 도메인 요구 사항도 이 단계에서 발견됩니다.
<br>

- **요구사항 분류 및 구성** (Requirements classification and organization)
  - 관련 요구 사항을 그룹화하고 일관된 클러스터로 구성합니다.
<br>

- **우선순위 및 협상** (Prioritisation and negotiation)
  - 요구 사항의 우선 순위를 지정하고 요구 사항 충돌을 해결합니다.
<br>

- **요구사양** (Requirements specification)
  - 요구 사항은 문서화되고 나선형의 다음 라운드에 입력됩니다.
<br>


### ✅ Requirements discovery (요구사항 발견)❌
- 필수 및 기존 시스템에 대한 정보를 수집하고 이 정보에서 사용자 및 시스템 요구사항을 추출하는 프로세스.
<br>

- 상호 작용은 관리자에서 외부 규제 기관에 이르기까지 시스템 이해 관계자와 이루어집니다.
<br>

- 시스템에는 일반적으로 다양한 이해 관계자가 있습니다.
<br>


### ✅ Interviewing (인터뷰) 

> <br>
>
> 이해 관계자와의 공식 또는 비공식 인터뷰는 대부분의 RE 프로세스에서 진행됩니다.
> 
> <br>

#### 면접유형
  - **비공개 인터뷰** (Closed Interview)
    - 미리 정해진 질문 목록을 기반으로 진행됩니다.
  <br>

  - **공개 인터뷰** (Open Interview)
    - 다양한 이슈를 이해관계자와 함께 탐구합니다.
<br>

#### 효과적인 면접❌
  - 열린 마음을 갖고 요구 사항에 대한 선입견을 피하고 이해 관계자의 말을 기꺼이 경청합니다.
<br>

  - 면접 대상자에게 스프링보드 질문, 요구 사항 제안을 사용하거나 프로토타입 시스템에서 함께 작업하여 토론을 진행하도록 요청합니다.
<br>

#### 실무에서의 인터뷰❌
- 일반적으로 **비공개 인터뷰와 개방형 인터뷰가 혼합**되어 있습니다.
<br>

- 인터뷰는 이해 관계자가 무엇을 하고 시스템과 상호 작용할 수 있는지에 대한 **전반적인 이해를 얻는 데 유용**합니다.
<br>

- 면접관은 시스템이 무엇을 해야 하는지에 대한 선입견 없이 열린 마음이 필요합니다.
<br>

- 사용자에게 단순히 원하는 것을 묻기보다 요구 사항을 제안하여 시스템에 대해 이야기하도록 유도해야 합니다.
<br>

#### 👎🏼 인터뷰에서의 문제 
- 애플리케이션 전문가는 요구 사항 엔지니어가 이해하기 쉽지 않은 언어를 사용하여 작업을 설명할 수 있습니다.
<br>

- 인터뷰는 도메인 요구 사항을 이해하는 데 적합하지 않습니다.
  - 요구 사항 엔지니어는 특정 도메인 용어를 이해할 수 없습니다.
  - 일부 영역 지식은 너무 친숙하여 ​​사람들이 설명하기 어렵거나 설명할 가치가 없다고 생각합니다.
<br>

### ✅ Ethnography (민족지학)❌
- 사회 과학자는 사람들이 실제로 어떻게 일하는지를 관찰하고 분석하는 데 상당한 시간을 할애합니다.
- 사람들은 자신의 작업을 설명하거나 명료화할 필요가 없습니다.
- 중요한 사회적, 조직적 요인이 관찰될 수 있습니다.
- 민족지학적 연구에 따르면 작업은 일반적으로 단순한 시스템 모델에서 제안하는 것보다 더 풍부하고 복잡합니다.
<br>

#### 민족지학의 범위❌
- 프로세스 정의가 작업해야 한다고 제안하는 방식보다 사람들이 실제로 작업하는 방식에서 파생된 요구 사항.
- 다른 사람의 활동에 대한 협력과 인식에서 파생되는 요구 사항.
  - 다른 사람들이 하는 일에 대한 인식은 우리가 일을 하는 방식의 변화로 이어집니다.
- 민족지학은 기존 프로세스를 이해하는 데 효과적이지만 시스템에 추가해야 하는 새로운 기능을 식별할 수 없습니다.
<br>

#### 집중된 민족지학❌
- 항공 교통 관제 과정을 연구하는 프로젝트에서 개발
- 민족지와 프로토타이핑 결합
- 프로토타입 개발은 민족지학적 분석에 초점을 맞춘 답이 없는 질문을 초래합니다.
- 민족지학의 문제는 더 이상 관련이 없는 역사적 근거가 있을 수 있는 기존 관행을 연구한다는 것입니다.
<br>

#### 요구 사항 분석을 위한 민족와 프로토타이핑❌
![1](https://i.imgur.com/e51znqa.png)
<br>

### ✅ 스토리와 시나리오
> <br>
>
> 시나리오와 유저 스토리는 **시스템의 실제 사용 예시**이며, 시스템이 특정 작업에 어떻게 사용될 수 있는지 설명합니다.
> 실제 상황을 기반으로 하기 때문에 이해관계자는 스토리에 공감하고 상황에 대해 논평할 수 있습니다.
> 
> <br>

<br>

#### iLearn 예시 : 교실에서 사진공유

> <br>
>
> Jack은 Ullapool(스코틀랜드 북부의 한 마을)의 초등학교 교사입니다. 그는 클래스 프로젝트가 어업의 역사, 개발 및 경제적 영향을 살펴보고 지역의 어업을 중심으로 집중되어야 한다고 결정했습니다. 그 일환으로 학생들은 친척들로부터 추억을 수집 및 공유하고, 신문 기록 보관소를 이용하고, 지역의 어업 및 어촌과 관련된 오래된 사진을 수집하도록 요청받습니다. 학생들은 iLearn Wiki를 사용하여 낚시 이야기를 수집하고 SCRAN(역사 자료 사이트)을 사용하여 신문 아카이브와 사진에 액세스합니다. 그러나 Jack은 학생들이 서로의 사진을 찍고 댓글을 달고 가족에 있을 수 있는 오래된 사진의 스캔본을 업로드하기를 원하기 때문에 사진 공유 사이트도 필요합니다.
>
> <br>
> 
> Jack은 자신이 속한 초등학교 교사 그룹에 이메일을 보내 적절한 시스템을 추천할 수 있는 사람이 있는지 확인합니다. 두 명의 교사가 답장을 보내고 둘 다 교사가 콘텐츠를 확인하고 조정할 수 있는 사진 공유 사이트인 KidsTakePics를 사용한다고 제안합니다. KidsTakePics는 iLearn 인증 서비스와 통합되어 있지 않으므로 교사와 수업 계정을 설정합니다. 그는 iLearn 설정 서비스를 사용하여 학급의 학생들이 볼 수 있는 서비스에 KidsTakePics를 추가하여 로그인하는 즉시 시스템을 사용하여 모바일 장치와 학급 컴퓨터에서 사진을 업로드할 수 있습니다.
> 
> <br>

<br>

#### 시나리오 
- 사용자 스토리의 구조화된 형태
<br>

- 시나리오의 형태
  - **시작 상황**에 대한 설명
  - **정상적인 이벤트 흐름**에 대한 설명
  - 무엇이 **잘못**될 수 있는지에 대한 설명
  - 기타 동시 활동에 대한 정보
  - **시나리오 완료 시 상태**에 대한 설명
<br>

#### iLearn 예시 : 사진 업로드 
> <br>
>
> - **초기 가정**
>   - 사용자 또는 사용자 그룹은 사진 공유 사이트에 업로드할 하나 이상의 디지털 사진을 가지고 있습니다. 이들은 태블릿이나 노트북 컴퓨터에 저장됩니다. KidsTakePics에 성공적으로 로그온했습니다.
>
> <br>
> 
> - **일반적인 동작**
>   - 사용자가 사진 업로드를 선택하면 컴퓨터에 업로드할 사진을 선택하고 사진을 저장할 프로젝트 이름을 선택하라는 메시지가 표시됩니다. 또한 업로드된 각 사진과 연결되어야 하는 키워드를 입력할 수 있는 옵션이 제공되어야 합니다. 업로드된 사진의 이름은 사용자 이름과 로컬 컴퓨터의 사진 파일 이름을 결합하여 지정됩니다.
>   - 업로드가 완료되면 시스템은 자동으로 프로젝트 중재자에게 새 콘텐츠를 확인하도록 요청하는 이메일을 보내고 완료되었다는 화면 메시지를 사용자에게 생성합니다.
>
> <br>
>
> - **무엇이 잘못될 수 있습니까?**
>   - 선택한 프로젝트와 연결된 중재자가 없습니다. 프로젝트 중재자를 지명하도록 요청하는 이메일이 학교 관리자에게 자동으로 생성됩니다. 사진을 표시하는 데 지연이 있을 수 있음을 사용자에게 알려야 합니다.
>   - 동일한 사용자가 이미 동일한 이름의 사진을 업로드했습니다. 동일한 이름으로 사진을 다시 업로드할 것인지, 사진 이름을 바꿀 것인지 또는 업로드를 취소할 것인지 사용자에게 물어봐야 합니다. 사진을 다시 업로드하도록 선택하면 원본을 덮어씁니다. 사진 이름을 바꾸도록 선택한 경우 기존 파일 이름에 숫자를 추가하여 새 이름이 자동으로 생성됩니다.
>
> <br>
> 
> - **기타 활동** 
>   - 중재자는 시스템에 로그온할 수 있으며 업로드되는 사진을 승인할 수 있습니다.
>
> <br>
> 
> - **완료 시 시스템 상태** 
>   - 사용자가 로그온되어 있습니다. 선택한 사진이 업로드되었으며 '검토 대기 중' 상태가 지정되었습니다. 사진은 중재자와 사진을 업로드한 사용자에게 표시됩니다.
> 
> <br>

<br>