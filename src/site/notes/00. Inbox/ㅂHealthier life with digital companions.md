---
{"dg-publish":true,"permalink":"/00-inbox/healthier-life-with-digital-companions/","dgHomeLink":true,"dgPassFrontmatter":false}
---


# Abstract
- Quantified-self tools의 장점 : real time으로 감정적, 신체적인 개인 데이터를 track할 수 있음
- 문제 : 그러나 스마트폰이나 피트니스 트래커 등의 장치로 데이터를 수집했을 때 큰 이득이 없음
- 본 연구의 지향점 : 사용자 인식이나 사용자 행동에 영향을 주기 위해  Quantified-self tools이 어떻게 디자인되어야 하는지
	- 특히 MRF(Message Representation Format) -> QS tool을 companion으로 인식하게
	- 왜? 대화형 상호작용에서 사용자와 QS tool이 상호작용 하는 것이 중요하기 때문
	- Samantha라는 메시지 표현 알고리즘을 제작 - 4가지 메시지 표현 방식
	- 

# Introduction

> 데이터가 아니라 "지식"이라고 한 것을 보면 단순 데이터 수집 도구가 아니라 인사이트까지 제공해줘야 하는 컴퓨터라고 생각
> 아이폰 건강 앱에 어떤 과정이나 계산을 거쳐 이런 지표가 측정되는지 나와있음. -> 데이터의 측정 방식을 사용자에게 인식시켜서 건강한 행동을 채택하게 만들기 위한 설계였음
> 사회학의 soci 자체가 동료라는 뜻을 지닌 compaion을 의미
> 일기예보를 제안해주는 것은 촉각적인 인터렉션을 줘서가 아니라, 다른 사회 구성원이 나에게 정보 혹은 도움을 주었기 때문에 호혜성 차원에서 companionship을 느끼는 것이라고 생각이 들었음.
> 마이데이터에 관련된 전망을 어떻게 볼지.. 최근에 있던 LG인지 SK인지 사례와 전망
## quantified-self tool
- 정의 : 자가 추적 기술로 스스로에 대한 지식을 얻을 수 있는 도구
- 수집 사례 : number of steps, amount and quality of sleep, heart rate, and even emotional and psychological statuses in real time...
- 장점 : **technologies of memory**
	- 데이터를 추적, 수집 및 기억하기 위한 적극적인 노력 없이도 데이터 측면에서 스스로 이해 가능하도록 도와줌
		- what they did (e.g., exercising)
		- when they did it (e.g., in the morning)
		- where they did it (e.g., in a park)
		- how they did it
	- 장치 또는 응용 프로그램 사용의 초기 단계에서 자신의 행동에 대한 더 깊은 이해 가능
	- 개인 건강 관련 행동과 관련하여 사용자와 장치 간의 더 깊고 의미 있는 상호 작용을 시작하는 데 사용될 가능성 농후
		- 데이터의 의미와 측정 방식을 이해하면 건강한 행동 채택 -> 의미있는 결정 내림
- 문제 제기 : 추적된 데이터를 단순 제공하는 것은 사용자들에게 그다지 유익하지 않다. -> 사용 중단으로 이어짐
	- 1. 단순 트래킹된 데이터를 제공하는 것은 어떤 의미를 가지고 있는지 모름
	- 2. 트래킹된 데이터에 기반해서 현상에 대한 알람을 주는 유용한 상호작용 많이 없음 -> 현상을 파악하기 위해 QS tool을 계속해서 살펴봐야 한다는 문제 발생.
- RQ
	- 트래킹된 데이터를 통해 발생하는 사용자 경험이 어떤 인식과 행동을 유발하는지 살펴보겠음.
	- 1. 데이터 추적을 통해 **행동 변화를 촉진하는 ux 요소**가 무엇일까?
		- 사회학) companion의 존재는 상대방의 생각과 행동을 유지하거나 변화시키는 데 중요
		- companion은 상대방에 대한 철저하고 친밀한 지식을 개발
		- 장기적 관계를 통해 상대방이 자신의 행동을 바꾸도록 촉진
		- HCI ) "computers are social actors" : H와 C와의 인터랙션이 H와 H 맥락에서 해석 가능하다는 패러다임 -> 인간과 컴퓨터가 정서적인 유대감을 가진 관계로 발전할 수 있음
		- ==companoid experience== : user experience of companion-like interactions with device or service **regularly**
				- 어떤 식으로 proactive interaction 만드는가?
				- emotional interaction
				- conversational messages
				- voice-based notifications
				- meaningful tactile vibration : 내일의 일기예보 제안...
		- proactive interaction 바탕으로 user는 디바이스를 장기적인 companion으로 인지 -> 지각된 companion이 사용자 행동에 중요한 영향을 미칠 것임.
		- percived companion : affected by experiencing companion like interactions
	- 2. 인지된 companion을 촉진시키기 위해서 **interaction을 어떻게 설계**할 것인가?
		- 사용자가 현 상태를 알 수 있게 함에 있어서 알림이 효과적이나 많은 디바이스에서 추적된 결과만 단순하게 전달한다는 문제 존재 -> 트래킹된 데이터와 실질적 활용 간의 gap 존재
		- MSF(Message Representation Formats) -> user의 companion perception에 영향 미칠 것이다.
		- CL(context level) : 나의 데이터를 얼만큼 반영하고 있는지
		- ST(statement type) : 트래커가 생각할 수 있다는 인상을 얼만큼 주는지

# Theoretical background
> 아동 분야에서 companion이 동등한 지위를 가진 사람이라고 정의되고 있음. 호혜성이라는 단어가 자꾸 생각나긴 함
> 기존에는 폼팩터 기반으로 companion이 형성되었지만 현재는 더 넓은 범위에까지 확장. 왜? 앞으로는 그럼 어떻게 될 것 같은가?
> 문서 기반의 정보가 올라갔던 HTML 시절, 정보의 양은 늘어나지만 공간은 부족했었음. 그런데 현재는 공간 기반의 정보가 올라가는 상태가 되버림. 정보로써의가 아니라 상태를 이해할 수 있는 기술로 발전되는 메타버스 시절이 오게 됨
> 사용자 개인의 정보를 저장해두는 DB는 확장된 자아가 될 수 있을 것 같다.
> 개인 사용자가 아닌 다수의 커뮤니티 사용자들과 companionship을 어떻게 맺을까?
> 메타버스에 디지털 트윈이라는 측면에서 확장된 자아와 자아를 둘러싼 환경을 가상 세계에 구축하려는 이동이 많이 발생할 것이다. 컴패니언십을 구축하기가 더 쉬워질 수 있음. 라이프로깅과 관련되어 생각해볼 수도 있다.!!!
> 에스파 사례 : ae-X와 X와는 companionship을 맺고 있다고 볼 수 있다.
> 사람들은 연결을 원하기 때문에 코시국에서 메타버스가 대두되었다고 볼 수 있음. 그런데 이 과정에서 윤리적 문제가 대두되고 있는데, 컨트롤이 가능한 디지털 프로덕트 내의 엔티티로써 컴패니언을 제한할 수 있을 것임
> VFX 기술의 발전에 따라 외관의 의인화 정도가 높아지고, 커스텀 정도가 높아짐. UGC에 가까운데 나의 정보를 잘 반영할 수 있어서 Companionship으로 여길 수 있음. 실제 감정노동자를 대체할 수 있음.
> p2e가 한때 유행이지만 c2e를 제안해볼 수 있을 것이다. 블록체인 등으로 관계가 돈이 될 수 있음
> 소복소복이 사용자 건강상태 아는 companion이 되어버렸네
> 호손효과 때문에 거짓 응답에 대한 비율을 줄이는 이슈도 중요할 것 같음.
## Perceived companion
companion
- “a person showing close connection with others.” - Mooers (1981)
- child relation field : 아동이 타인과 친밀감을 형성하는 공간에서 놀이의 경쟁자(동일한 지위를 가진 사람)
- married life : 동반자는 활동, 감정 및 기타 내적 및 외적 것들을 공유할 수 있는 파트너
- family relationship: 같은 공간에 머물며 아버지, 어머니, 형제, 자매 또는 기타 가족 구성원의 역할을 하는 자
- pet : 반려견과 같이 주인이 시간을 보내고 관계를 유지하기 위해 노력할 수 있는 사회적 친구
- medical health care : 간병에 관심이 있고 도구적 지원을 제공하는 지지자
- 초기 HCI : 주요 애플리케이션 폼팩터 ex. 모바일 장치, 로봇, 가상 에이전트 또는 기타 스마트 컴퓨팅 장치

companion의 기준
- accessible over longer periods of time (availability가용성 and proximity근접성)
- friendly relation (friendliness)
- makes sense of and uses personal information (helpfulness)
- interacts with users frequently
- assists humans in daily life
- spends time with the counterpart
- 인간과의 상호작용을 통해 친밀감을 키우고, 특정 역할을 수행하고, 앞서 언급한 과정을 기반으로 인간과 재상호작용하는 제품 또는 서비스로 정의

==디바이스나 서비스와 상호작용하는 UX는 companionship and extended-self라는 2가지 key factor를 포함한다.==

### Companionship

- companionship = jointness (decision-making in many daily events)
- companionship = 만족이나 향유라는 본질적인 목표를 위해 추구되는 공유 활동에 대한 사회적 참여
- social companionship = 여가 활동에서 다른 사람들과 시간을 보내는 것
- HCI에서의 companionship : companion과 본인과의 관계에 대한 user perception 측면의 내용. 특히 실제 펫과의 유사성이 높은 인공 펫에 대한 관심이 늘어나고 있는데 가능성을 보여줌
- intelligent system에서의 companionship : 두 명의 동반자가 상호 신체적 또는 심리적 활동을 공유하는 상호 관계 -> 제품 수명 주기와 관련 제품 개발 관련해서 영향을 미칠 수 밖에 없다.
- companionship : 타 엔티티 경험에 관련된 관계 측면 이야기. 
- companionship should be considered as the relational aspect of a perceived companion.
### Extended-Self
- 외부 대상, 개인 소유물, 사람, 장소, 신체 부위 및 중요한 기관("나" 또는 "내 것"으로 생각됨)이 포함
- 인체의 유기체일 뿐만 아니라 공책과 같은 단순한 대상을 포함하는 외부 유기체일 수 있는 물리적 또는 심리적 존재로 정의.
- 우리는 우리 자신에 대해 느끼고 행동하는 만큼 사물을 감지하고 우리의 특정 행동을 수행
- 확장된 자아의 일부인 대상이, 자신에 대한 지식을 가지고 있기 때문에, 대상을 해당 지식의 특정 기억으로 기억함
- 상대방(user)에 대한 정보를 개발하고, 이해하고, 상호작용 과정에 따라 적절한 피드백을 제공 -> 상호작용을 통해 동반자는 단순히 다른 사람과 함께하는 것이 아니라 상호 이해를 통해 서로 공감하는 한 쌍의 일부가 됨 -> 확장된 자아의 개념은 동반자에 대한 인식의 중요한 요소
- HCI 맥락에서 태블릿은 개인의 기억이나 지식을 확장시킨 자아의 확장으로 보고 있음
- 디지털 공간에서 digital artifact는 사용자를 위해서 의미있는 지식을 통합해야 한다.
- user는 자신의 물리적 정보나 심리적 정보를 디지털 개체에 제공. ex 본인을 닮은 아바타 -> 정신생리학적으로 본인이라고 느껴질 수 있음
- 확장된 자아로부터 특정 개체를 동반자라고 경험할 수 있어짐 : ownership, control, and attachment 감정 제공 -> personal power, a symbolic attachment, and a special meaning for users 증가
- 자기 중심적 경험에 영향을 미침 -> 사용자의 자아 개념이 외부 제품이나 서비스와 매끄럽게 결합되는 긴밀한 관계를 경험할 수 있음
- 따라서 확장된 자아를 동반자의 자아로 간주해야 함

## Quantified self and Behavior change
- 인간의 기억을 증강하고 외부화 -> 인간의 삶에 대한 total capture을 하려는 기술적인 시도 : lifelogging
- - 초반에는 자전적인 기억을 그리려고 했으나 기술이나 기기들이 발전함에 따라서 명시적인 목표에 해당하는 데이터를 모으는 쪽으로 발전했음.
- 정량화된 자아 : 환경적 요인(food consumed, quality of surrounding air), 생물학적 상태(mood, arousal, blood oxygen levels), 성과(mental and physical) 측면에서 개인의 일상 생활 측면에 대한 데이터 수집에 기술을 통합하려는 움직임
- 자기지식을 얻는 일반적인 방법 : 자신의 행동, 습관, 생각 등의 데이터를 수집하여 자신의 일상생활을 성찰하는 것 -> 컴퓨팅 장치는 이걸 촉진시킬 수 있음.
- 정량화된 자아의 차원 - 각 차원은 사용자가 특정 목표를 달성할 수 있도록 설계되어야 함
	- tracking : 특정 데이터를 캡처하고 추적하는 것을 기반. 추적을 통해 "정량화된 자아"는 자신의 가치를 수집하고 개선된 자기 지식을 얻을 수 있습니다.
	- triggering : 디지털 장치에서 제공하는 추적 기능을 사용하는 정량화된 자아가 인지하고 반영해야 합니다. ex 알림
	- recalling : 자기 지식에 대한 접근과 관련 있음. 수치화된 자아는 자신의 행동을 회상함으로써 자신이 먹는 음식의 종류, 하루/주에 걷는 걸음 수, 잠자는 시간과 같은 생활 방식의 세부 사항을 알 수 있습니다.
- 스마트폰과 웨어러블 기기는 자아정량화 도구로서 사용자가 자아정량화 과정을 인지할 수 있도록 지원해야 한다. but 단순한 기본적인 수준의 분석에 그침 - user engagement나 reminder 등의 연구가 발생
- 사용자는 실제 생활에서 자신의 행동을 변경하거나 관리할 필요성을 인식하지 못함 : 사용자는 자신의 응용 프로그램과 장치가 자아를 알도록 유발하고 회상하는 데 도움이 되는 적절한 상호 작용을 제공하지 않는다고 생각함
- 그래서 본 연구에서는...관계적 측면에서는 추적 데이터를 통해 분석된 사용자의 행동을 반영하여 자기계량화 과정에서 ==triggering== 을 인지하도록 지원할 수 있다.
- 사회과학에서 동반자의 존재는 social role 속에서의 interaction reflection을 통해 상대방의 건강 상태에 영향을 미침
- 사회적 역할을 하는 사람은 묻고, 관찰하고, 측정하는 등 다양한 상호작용을 통해 동반자에 대한 일반적인 지식을 얻음 : high level of context이 low level보다 동반자의 건강 상태에 더 긍정적인 영향을 미침
- 자아 측면에서, 기기를 통한 상태 표현은 quantified-self 과정에서 ==recalling==을 인식할 수 있게 함 : personal control에 대한 formalization는 동반자의 건강 상태에 더 긍정적인 영향을 미침. 높은 건강 상태를 유지하려는 의지
# Research hypothesis
## Effect of the level of context of tracked values on perceived companion
- 사람들은 경험을 할 때 과거의 기억에 기반한다. 이전의 경험을 바탕으로 새로운 관점을 가지거나 행동을 변경할 수 있음. 그러나 디지털 흔적들은 회상을 목적으로 설계되지는 않았다.
- 타임캡슐 만든다고 했을 때 쓸데 없는 쪼가리들 가져왔음. 이를 통해서 일상적인 라이프스타일을 트래킹 할 때 과거 회상에 대한 패턴을 제시해주는 것 보다 **특성의 스토리텔링**을 지원하는 것이 더 요하다는 사실을 알 수 있었음
- self knowledge를 형성하는데에 어떤 가치를 수집할지 아는 것은 어려움 -> 왜냐하면 사람들은 한정적인 기억을 가지고 있고 관찰할 수 없는 행동이 있고 관찰 시간이 부족하기 때문
- 대부분의 self knowledge는 companion과 interaction을 회상함으로써 형성된다. : companion이 다른 사람의 개인정보를 받아 공감대를 형성한다면그 다른 사람은 companion으로부터 완전한 자기지식을 받았기 때문에 상대방이 자신에 대해 얼마나 알고 있는지 알 수 있다.
- 따라서 사용자가 회상해야 할 표현과 comapnion이 트래킹된 값을 어떻게 표현해야 하는지를 숙고해야 한다. <-LC(level of context) : 높은 수준의 lc는 사용자의 목표랑 암묵적인 의도를 함께 고려함.
- comapnion이 사용자의 맥락적인 정보를 인식하면 개인화된 메시지를 실시간으로 형성할 수 있음. 반대로 고정적인 정보만을 인식하면은 낮은 레벨로 이어진다.

```
H1. A high level of context has more positive effect on a perceived companion than does a low level of context.
높은 수준의 맥락은 낮은 수준의 맥락보다 지각된 동반자에게 더 긍정적인 영향을 미칩니다.
```
## Effect of statement type of message with tracked values on perceived companion
- 사람들은 다른 사람이나 자신의 평가를 통해 자신의 현재 상태를 확인 -> 평가에 대한 인식은 자기 규제 행동에 영향을 미침
- Self-regulation = 자기기준에 맞게 자신의 행동을 통제하는 행동
- Behavior change stage
	- pre-contemplation
	- contemplation
	- pre- paration
	- action
	- maintenance
- 목표의 구체적인 가치와 현재의 실제 가치 사이의 부조화는 개인의 사고방식에 의미를 부여하고 동기를 유발한다. 이 차이를 인식시키기 위해서는 companion이 필요하다.
- Hawthorne effect : 일종의 반응 현상으로서 개인들이 자신의 행동이 관찰되고 있음을 인지하게 될 때 그에 대한 반응으로 자신들의 행동들을 조정, 순화시키는 것. 나는 관찰되고 있다
- companion의 기분 공유 타임라인이랑 사용자의 무드 점수를 공유하는 것이 상대방의 관찰에 대한 인식을 높였음. -> 동반자와 같은 감정을 전달하도록 고려해야함
- Statement type messages : 대화적이며 상대방의 감정과 메시지 수용에 영향을 미친다.
	- 나 메시지와 너 메시지
	- Companion 디바이스는 자기중심적인 툴이고 사용자 중심적인 툴이다.
- 데이터에서 생성된 메시지가 확장된 자기 감정을 반복적으로 전달하면 사용자는 이를 장치의 메시지로 인식할 뿐만 아니라 내면의 마음가짐이나 자기 성찰의 표현으로 인식할 수 있습니다. 너 메시지는 잔소리처럼 느껴질 수 있음. 그리고 자기 중심적인 메시지 호손 효과 유발 가능
- 자기 중심적 메시지(I 진술)가 자기 규제에 관한 동질적 진술(You 진술)보다 더 효과적일 수 있다

```
Egocentric statements have a more positive effect on a perceived companion than do the allocentric statements.
자기중심적 진술은 동종중심적 진술보다 지각된 동반자에게 더 긍정적인 영향을 미친다.
```
## Interaction effect of representation format of message on perceived companion
- Embodied cognition = sensory-motor (embodied) knowledge representa- tion acquired during typical learning
- "체화" : 것은 마치 개인이 바로 그 상황, 바로 감정적 상태, 바로 사유의 대상과 함께 그곳에 있는 것과 같음
- 인간의 의미를 포함하는 수행 가능한 문장은 동반자의 지각에 긍정적인 영향을 미친다
- 메시지의 중심성은 컴패니언 장치의 인식에 중요한 영향을 미칩니다. 특히 자기계량화 도구가 만들어내는 메시지가 자기중심적이라면 사용자는 LC가 높을수록 companionship을 더 많이 인지하게 된다.
- 추적된 값은 평소에 자기 규제의 기준으로 사용되기 때문에 계량화된 자기 도구를 통한 자기 지식의 표현은 높은 수준의 컨텍스트와 추적된 값을 통해 사용자의 일상 활동에 대한 반추를 용이하게 함
- 자기 중심적 메시지를 생성하는 장치는 높은 맥락의 메시지를 제시할 때 더 가깝게 인식되고 더 효과적일 것. 너 전달법 사용하면 상대방의 추론으로 인식할 수 있음.
```
H3. The positive effect of egocentric messages on the per- ceived companion will be stronger if the level of context is high.
따라서 맥락의 수준이 높을수록 자기중심적 메시지의 효과가 더 강하다고 가정한다. 따라서 우리는 다음과 같은 가설을 제안한다.
```

## Effect of perceived companion on behavior change
- 사람들은 동반자와 상호 작용할 때 행동 변화를 일으키려는 동기를 부여받는 경향이 있다
- 사람들이 웹사이트 및 장치와 동반자로서 상호 작용할 때 행동 변화를 만드는 데 더 열성적
- 행동 변화는 개별 기술을 사용하여 가능한 결과가 아니라 동료와 같은 다른 사람들이 촉진할 수 있는 것
- 우리는 사람들이 장치와의 교감에 대한 인식 수준이 높을수록 컴패노이드 경험을 할 준비가 더 잘 되어 있다고 가정
```
H4. Perception of a companion positively influences behavior change.
동반자에 대한 인식은 행동 변화에 긍정적인 영향을 미칩니다.
```
# Experimental study