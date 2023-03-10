# Daily_topic

# 목적
* CS 및 키워드공부는 암기가 아닌 응용이 중요 하다고 생각했다. 다양한 상황에서 접목시키고, 다양한 상황을 떠올리며 대응해야 한다고 생각했다. 그래서 간단하게 물음을 던지고, 답하는 식으로 한줄씩 늘려가볼까 한다.

# 방법
* 하루에 하나의 토픽을 정해 답변을 기록하고, 답변이 적절했는지 고민해본다.
* 거창한 키워드가 아니여도 좋다. 간단한 키워드로써, 내가 CS, DATA, NETWORK등.. 다양하게 컴퓨터 관련이라면 하루에 하나씩 해보자

<details><summary style="color:skyblue">Polymorphism - 다형성(동질 이상)</summary>
<p>

다형성이란 어떤 변수, 메소드가 상황에 따라 다른 결과를 내는 것

* 오버 로딩- 같은 메서드 이름 / 다른 인자 목록 / 다수의 메서드 = **재정의**
* 오버 라이딩 - 같은 메서드 이름 / 같은 인자 목록 / 상위클래스의 메서드 재정의 = **중복정의**
</p>
</details>

<details><summary style="color:skyblue">Encapsulation - 캡슐화</summary>
<p>

public - 모두 / protected 상속, 같은 패키지 내 클래스 / default 같은 패키지 내 클래스 / private - 본인

* 실제로 구현 부분을 외부에 드러나지 않도록 하는 것
* 변수와 메소드를 하나로 묶음
* 데이터를 외부에서 직접 접근하지 않고 함수를 통해서만 접근
</p>
</details>

<details><summary style="color:skyblue">Inheritance - 상속</summary>
<p>

* 자식 클래스가 부모 클래스의 특성과 기능을 물려받는 것
* 기능의 일부분을 변경하는 경우 자식 클래스에서 상속받아 수정 및 사용함
* 상속은 캡슐화를 유지, 클래스의 재사용이 용이하도록 해 준다.

* 하위 클래스 - 상위 클래스
* 하위 클래스는 상위클래스 특성을 재사용하고, 확장한다.
* 상위 클래스의 물려줄 특성이 많을수록 좋다 (LSP)
* 상위 클래스가 너무 빈약하면, 불필요한 형변환이 자주 일어난다.
</p>
</details>

<details><summary style="color:skyblue">OOP 5원칙</summary>
<p>

S (SRP : Single Responsibility Principle)
한 클래스는 하나의 책임만 가져야 함.

O (OCP : Open/Closed Principle)
확장에는 열려(Open) 있으나, 변경에는 닫혀(Closed)있어야 함.

L (LSP : Liskov’s Substitution Principle)
프로그램의 객체는 프로그램의 정확성을 깨뜨리지 않으면서 하위 타입의 인스턴스로 바꿀 수 있어야 함.

I (ISP : Interface Segregation Principle)
특정 클라이언트를 위한 인터페이스 여러 개가 범용 인터페이스 하나보다 남.

D (DIP : Dependency Inversion Principle)
추상화에 의존한다. 구체화에 의존하면 안됨.
</p>
</details>

<details><summary style="color:skyblue">Devops / MLops</summary>
<p>

**데브옵스** -  소프트웨어의 개발(Development)과 운영(Operations)의 합성어
* 소프트웨어 개발자와 정보기술 전문가 간의 소통, 협업 및 통합을 강조하는 개발 환경이나 문화

* 이점 - 속도 / 신속한 제공 / 안정성 / 확장가능 / 협업강화 / 보안

**ML옵스** - 머신러닝 (Machine Learning)의 약자인 ML과 Operations의 약자인 Ops가 합쳐져 탄생한 단어로, 모델 개발 시스템과 운영 시스템을 통합하여 더욱 유연하고 효율적인 개발을 가능케 하는 도구이자 개발 환경

* ML 옵스에서는 코드 저장 및 배포 단계에 앞서 데이터 셋 분석 및 모델 개발을 담당하는 ML Research 팀의 역할이 추가

**주요 기능 및 기술**
* 모델관리 / 연구 과정 중 수행한 모델들과 그 성능을 기록하는 행위
* 모델 서빙 /  모델이 성공적으로 저장되면, 모델을 배포 환경에 서빙
* 백엔드 엔지니어 (Back-end Engineer)가 구축한 비즈니스 로직 서버에서 모델이 필요한 부분에 대해 API (Application Programming Interface) 형태로 호출하는 API 서빙
* 여러 데이터를 한 번에 처리하는 Batch 서빙
* 모델 모니터링 / 모델 서빙 단계에서는 외부 소프트웨어 컴포넌트가 API를 통해 모델로 추론 요청을 보내고, 모델은 추론 결과를 응답으로 보내는 사이클이 진행 모니터링
* 지속적 학습 /  Continuous Training (CT)과정을 통해 변화하는 데이터에 맞추어 모델을 지속적으로 학습하고 배포해, 모델의 성능을 유지
</p>
</details>

<details><summary style="color:skyblue">CISC / RISC</summary>
<p>
CPU가 이해할 수 있는 명령어 집합인 ISA종류이다.

* CISC(Complex Instruction Set Computer) - 필요한 명령어 셋을 갖추도록 설계된 마이크로 프로세서에 관련된 용어로, 요구되는 능력을 가장 효율적인 방법으로 제공. 트랜지스터 집적에 있어서 효율성이 떨어지고 전력소모가 크며 속도가 느리고 비쌈.

* RISC(Reduce Instruction Set Computer) - 적은수의 컴퓨터 명령어를 수행하도록 설계된 마이크로프로세서로써 CISC보다 좀더 빠르게 동작, CPU의 명령어를 최소화하여 단순하게 제작된 프로세서, 효율특화된 CPU구조. 하드웨어가 단순하지만 소프트웨어가 복잡하고 크기가 커지는것이 단점. 전력소모가 적고 속도가 빠르며 저렴
</p>
</details>

<details><summary style="color:skyblue">HashMap / HashTable</summary>
<p>

Hash - 키_벨류로 데이터를 저장하는 자료 구조중 하나로, 빠르게 데이터를 검색할 수 있도록지원. 해시 함수를 통해 '키'와'벨류'로 저장되는 위치를 결정하므로 사용자는 위치를 알수 없고, 삽입되는 순서와 위치는 관계가 없음.

* HashMap - 동기화를 지원하지 않기(병렬처리 불가능)때문에 속도가 빠르고, Null 값을 허용 / Not-Tread-safe / Enumeration 을 지원하지 않음 / 보조해시를 사용해 테이블에 비해 충돌이 덜 발생

* HashTable - 동기화(병렬 처리 가능)를 지원하고, Null 값을 허용하지않음 / Tread-safe / Not Fail-Fast Enumeration지원 /

%fail-fast 방식 - 작업 중 오류 발생시 즉시 중단 후 오류 출력

%fail-safe 방식 - 작업 중 오류가 발생해도, 작업 중단 X
</p>
</details>

<details><summary style="color:skyblue"> 컨테이너 </summary>
<p>

컨테이너는 어떤 환경에서나 실행하기 위해 필요한 모든 요소를 포함하는 소프트웨어-
이점 - 책임 분리 / 워크로드 이동성 / 애플리케이션 격리
VM과의 차이 - 경량, OS /  하드웨어 수준의 가상화 차이 / OS 커널을 공유해, VM보다 적은 메모리 사용
</p>
</details>
