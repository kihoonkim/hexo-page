---
title: 페어 프로그래밍이란 무엇 일까?
date: 2018-01-01 16:16:39
tags:
  - agile
  - pair programming
categories: Agile
---
## 대화를 통해 서로의 생각을 공유하는 방법

![pair programming](/images/pair-photos.jpg "")  


우리팀(ACT)에서는 개발자뿐만 아니라 PM, CX등 모든 역할자가 Pair로 일을 한다. 그래서 Pair Programming보다는 Pairing 이라는 용어로 사용하고 있기도 하다. 결국엔 두 명이 짝을 지어 일을 한다는 것인데, 페어 프로그래밍의 진행 방법과 장단점 등에 대해 경험을 공유해 볼까 한다.

> Pair programming is an agile software development technique in which two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently.   - wikipedia -

페어 프로그래밍 진행 방법은 기본적으로 한 명이 타이핑을 하고 다른 한 명은 실시간 리뷰를 하는 것이다. 그리고 역할을 주기적으로 변경하며 진행하면 된다.
장비는 모니터, 키보드, 마우스 하나만으로 진행 할 수 도 있고, 모니터, 키보드, 마우스를 두 개씩 연결하고 각자 사용 할 수 도 있다.

아래는 딱히 정확한 명칭 없지만 개인적으로 진행해 봤던 방식들이다.

#### 드라이버 & 네비게이터
가장 일반적이고 전통적인 방법으로 한 명은 드라이버로 소스코드를 타이핑 하고, 다른 한 명은 네비게이터로서 작성되는 소스코드를 실시간으로 리뷰를 하고 큰 그림을 염두에 두고 가이드를 해 나가는 방법이다. 

#### 핑퐁(Ping-Pong)
TDD로 개발을 하는 경우, 한 명은 실패하는 테스트 케이스를 작성하고, 다른 한 명은 테스트를 성공시키기 위한 구현코드를 작성하는 방법이다. 한 명이 계속 키보드를 잡고 코딩을 하는 것을 방지 할 수 있다.

#### 키보드 & 마우스
한 명은 마우스만 사용하고, 다른 한 명은 키보드만 사용하는 방법이다. 잘 사용하지 않는 방법이긴 하지만, 새로운 툴이나 단축키 등을 배울 때 사용하면 유용할 수 있다.

#### 몹(Mob) 프로그래밍
일명 떼 코딩이라고 불리는 방법으로, 돌아가면서 한 명씩 드라이버가 되고 나머지는 네비게이터가 되어 개발을 진행한다. 가장 큰 장점은 커뮤니케이션 비용을 줄일 수 있다는 것이다. 프로젝트 초반에 코딩 스타일을 맞춰야 하거나, 주기적으로 코드리뷰를 하는 경우에도 사용하면 좋다. 하지만 단점은 네비게이터가 여러 명이다 보니 의견 통합이 어려울 수 있고, 간혹 자리를 비우거나 딴짓을 하는 사람이 생기기도 한다.

우리 팀의 경우는 모니터, 키보드, 마우스 모두 두 개씩 준비해서 각자 사용하고, 정해진 역할, 시간 없이 실시간으로 대화를 하면서 누구라도 타이핑을 할 수 있게 한다.

![pair programming](/images/pair-work.jpg "")

### 페어 프로그래밍을 하면 좋은 점
#### 지식 공유
같이 페어 프로그래밍을 진행 했던 사람들에게 물어보면 가장 많이 장점으로 언급되는 부분이다. 웹 개발을 하더라도 누구는 JavaScript를 잘하고 누구는 CSS를 잘 할 수 있는데, 이런 경우 같이 페어를 하면 서로 몰랐던 부분을 많이 배울 수 있게 된다. 그리고 팀에 새로운 멤버가 들어온 경우, 팀의 개발환경이나 개발 스타일 등에 대해서 문서로 전달 하는 것이 아니라 페어 프로그래밍을 통해 같이 개발하면서 공유해 줄 수 있다. 또한 기술적인 스킬 뿐만 아니라 페어가 가지고 있는 좋은 습관들도 배울 수 있는 좋은 기회가 된다.

#### 심리적 안정감
개발을 할 때, 간혹 어려운 문제가 있더라도 ‘페어가 있으니 해결할 수 있겠지?’ ‘페어가 해결해 주겠지?’ 등의 심리적으로 기댈 수 있다. 실제로 페어가 해결 하기를 기다리는 것이 아니라 같이 고민을 하게되는 것이다.
새로운 언어나 프레임워크 등을 사용해야하는 경우에도 혼자서는 중간에 포기하는 경우가 있는데, 페어와 함께 하다 보면 끝까지 도전을 해보게 되기도 한다.

#### 높은 업무 집중도
9시 출근해서 6시 퇴근 할 때까지 어느 정도로 집중해서 일을 할 수 있을까? 카카오 톡이나 라인 같은 메신저로 친구들과 대화도 나누고, 사내 메신저를 통해 동기들과 대화도 하고, 이메일도 주고 받게 되고, 티타임을 가지는 등 업무 외적으로 사용하는 시간이 많이 있을 것이다.
덕분에 중간중간 일의 흐름이 많이 끊기게 된다. 하지만 페어와 함께 개발을 하다 보면 불필요하게 사용하던 개인적인 시간을 최소화 하고, 개발에 집중을 하게 된다.

#### 실시간 코드 리뷰
작은 타이핑 실수부터, 큰 설계 결함 등 페어 프로그래밍을 하다 보면 실시간으로 해당 로직에 대해서 코드리뷰를 할 수 있다. 내 소스코드에 대한 피드백을 가장 빠르게 받게되는 것이다.
이를 통해 설계가 좋아지고, 결함도 줄어 들고, 일정한 수준의 코드 품질을 유지할 수 있었다는 의견이 많이 있다. 그리고 페어와 함께 개발을 하다 보면 코드 리뷰뿐만 아니라 같이 설계에 대한 고민을 끊임 없이 나눌 수 있는 사람이 있다는 것이 큰 장점 인것 같다.

#### 집단적 코드소유
[Collective Ownership](http://www.extremeprogramming.org/rules/collective.html)
페어 프로그래밍을 하게 되면 자연스럽게 일의 담당자를 지정할 수 없게된다. 즉, 업무마다 담당자를 정하고 그 업무만 개발 하는 것이 아니라, 팀으로서 전체 제품에 대해서 함께 고민하고 개발을 해나가는 것이다. 모든 개발자들이 어떤 기능이든지 추가나 버그 수정, 리팩토링 등을 진행할 수 있다. 특정 업무에 대한 병목이 발생하는 것을 막을 수 있고, 코드 전체에 대해서 개발자들이 함께 아이디어를 내고 공유할 수도 있다.

#### 피어 리뷰(Peer Review)
우리 팀은 항상 같이 일한 팀원 들에게 피어 리뷰를 하고 있다. 하지만 사실 같은 팀에 속해서 일을 하더라도 업무적으로 엮이지 않는다면 그 사람에 대해서 제대로 알기 어렵고 대외적인 이미지만 가지고 평가를 하게 된다. 하지만 페어 프로그래밍을 진행하면서 모든 팀원들과 같이 일을 하고 많은 대화를 나누게 됨으로써 동료들의 장단점을 더 잘 알게 되고, 그 사람의 성장을 위한 진실된 피드백을 줄 수 있었다. 자연스럽게 팀워크도 더 좋아지게 됐던 것 같다.

### 페어 프로그래밍을 하면 안 좋은 점
#### 생산성저하
많은 팀이 페어 프로그래밍을 하지않는 가장 큰 이유라고 생각된다. 관리자 입장에서는 한 명이 할 일을 두 명이 하고 있으니, 생산성이 반으로 줄어든다고 생각하기 때문일 것 이다.
경험상 봤을 때, 1/2은 아니더라도 분명히 생산성이 두 명이 각자 개발하는 것에 비해서 많이 떨어진다는 느낌을 받기는 했다. 오래되긴 했지만 몇 몇 논문에서 15% 시간이 더 걸리고, 15% 결함이 줄었다는 연구 결과도 있다.
앞서 장점으로 말했던 가치를 위해서 떨어지는 생산성은 미래를 위한 투자로 생각하는 것이 좋은 것 같다.

[참고 논문]
[Pair programming productivity](http://www.cs.utexas.edu/users/mckinley/305j/pair-hcs-2006.pdf)
[The Costs and Benefits of Pair Programming](https://collaboration.csc.ncsu.edu/laurie/Papers/XPSardinia.PDF)

#### 키보드 정복자
실제 페어 프로그래밍을 하다보면, 시니어와 주니어 개발자가 같이 하는 경우가 많은데, 드라이버와 네비게이터의 역할 바꿔가면서 진행해야 하지만 시니어 개발자 혼자 개발을 하게 되는 것을 자주 볼수 있다. 생산성이 떨어지는 문제를 못 참는 문제도 있고, 주니어 개발자가 작성하고 있는 코드를 가만히 보고만 있을 수 없는 것이다. 처음에는 말로 이렇게 해 저렇게 해 지시를 하다가 결국 키보드를 점령해 버린다. 이런 일이 반복되면서 주니어 개발자는 의기소침하게 되고 키보드 타이핑 하는 것을 두려워하게 된다. 페어 프로그래밍을 했다고는 하지만 대화 없이 한 사람의 주도하에 개발이 끝나게 되는 것이다.

#### 감정 노동
항상 좋은 사람과 일을 하면 좋겠지만, 우리는 언제나 마음이 맞지 않은 팀원과 함께 하게 될 것이다. 혹은 마음은 잘 맞더라도 개발하는 스타일이 매우 다른 사람이 있을 수도 있다. 사람 마다 가지고 있는 성격이나 스타일이 쉽게 바뀌거나 개선 할수 있는 부분이 아니기 때문에 해결하기 어려운 문제라고 생각된다. 우리나라 정서 상 대놓고 말하기 어려운 부분이기도 하다.
그 날 하루는 어쩔 수 심한 감정 노동에 시달리게 될 것이다.

#### 피곤함
페어와 함께 하루 종일 집중해서 개발을 하고, 끊임없이 대화를 한다는 것은 매우 많은 에너지를 소모하게 만든다. 중간 중간 쉬는 시간을 갖지 않으면 체력적으로 힘들어서 포기하게 될 것이다.


### 페어 프로그래밍을 잘하기 위한 방법들

페어 프로그래밍은 매우 단순한 agile Practice이다. 그냥 두 사람이 같이 앉아서 같은 것을 함께 개발하는 것이다. 하지만, 실제로 해보면 매우 어렵게 느껴지고, 금새 ‘우리랑은 맞지 않는 방법이야‘ 라며 포기를 하게 된다. 어떻게 하면 좀 더 잘할수 있을까?

너무 상투적인 얘기이지만 가장 중요한 방법은 "많은 대화와 소통" 이다.

언제나 설계에 대해서 같이 고민하고 대화를 해야 한다. 화이트 보드를 이용해서 시각적으로 표현해 가면서 이야기 하는 것을 추천한다. 페어 프로그래밍을 한다고 모니터 앞에만 앉아 있어야 한다는고 생각하는 것은 옳지 않다. 그리고 꼭 페어끼리만 대화를 해야하는 것도 아니다. 그 순간 필요하다면 다른 팀원들도 불러서 의견을 듣는 것도 좋을 것이다.

그리고 코딩을 하는 순간에도 ‘이런 생각을 가지고 있는데, 이렇게 한번 개발해 볼게요.’ 라며 현재 머리 속에 있는 생각을 계속해서 공유를 해야 한다. 그렇지 않으면 한 사람이 드라이버가 되서 개발 하는 순간에 정적이 흐르게 되고, 네비게이터는 딴 짓을 하게 될 것이다. 항상 현재 머리 속에 있는 생각을 가감없이 공유하길 바란다.

무엇보다 생각하는 것을 멈추면 안된다. ‘페어가 알아서 하겠지’ 라는 안일한 생각보다는 항상 더 나은 코드를 작성하기위해 노력하고, 함께 일을하는 페어에게 하나라도 더 공유하기 위해 노력해야 한다. 생각이 멈추면 대화도 멈추게 된다. 항상 끊임없이 더 나은 방법을 위해 생각을 하고 이야기를 해야 할 것이다.

만약 시니어 개발자와 주니어 개발자가 같이 페어를 하는 상황이라면 다음 글을 한번 읽기를 추천한다. 아래와 같은 5가지 팁이 나와있다.

※ 주니어와 함께하는 페어링 방법([Pairing with Junior Developers](https://www.devmynd.com/blog/2015-1-pairing-with-junior-developers/))

![Pairing with Junior Developers](/images/PairingwJuniors.jpg "")

**Don’t type.**  
직접 개발을 하지 말고, 주니어에게 무엇을 입력해야 하는지 알려주세요. 토론하고 질문하세요.

**Let them make mistakes.**  
직접 문제를 해결해 주면 일련의 규칙만 배우게 됩니다. 그냥 시도하게 하고 어떻게 되는지 지켜보세요. 문제가 발생하면 왜 안 되는지 이해할 수 있도록 도와주세요.

**Take Breaks**  
주니어와 시니어의 경험의 차이로 인해 많은 추가 설명을 해야 될 것입니다. 정말 많이 피곤할 것입니다. 휴식을 취하세요.

**Be prepared to say “I don’t know”**  
"나도 모른다. 그래도 좋은 질문이다. 같이 알아보자."
모르는 것에 대해 학습하는 방법을 알려줄 수 있는 좋은 기회입니다.

**Find what they can teach you.**  
멋진 연주자 이거나 암벽 등반가 일수도 있습니다. 그들이 가르쳐 줄 수 있는 것을 찾고, 배우고 싶다고 하세요. 둘 사이의 관계가 뒤집어 지는 순간 사회적 평등을 느낄 것입니다.

위 아티클의 마지막에 다음과 같이 강조하고 있다.

**“Just Remember: Don’t Type”**

시니어든 주니어든, 누구랑 같이 페어 프로그래밍을 하게 되든, 잊지 않았으면 한다. 타이핑을 하는 것 보다 대화를 하는 것이 더 중요하다. 대화를 통해 서로의 생각을 공유하자. 이것이 페어 프로그래밍을 잘 하는 가장 중요한 방법일 것이다.

당장의 속도 보다 팀의 성장을 원한다면 꼭 한번 페어 프로그래밍을 시도해 보길 바란다.

> “빨리 가고 싶으면 혼자 가고, 멀리 가고 싶으면 함께 가라”
