- HTTP와 HTTPS의 차이점은?

HTTP는 서버/클라이언트 모델을 따라 데이터를 주고받기 위한 프로토콜이다. HTTPS는 HTTP에 데이터 암호화가 추가된 프로토콜이다. 공개키/개인키 암호화 방식을 이용해 데이터를 암호화한다. HTTP는 암호화가 추가되지 않았기 때문에 보안에 취약한 반면, HTTPS는 안전하게 데이터를 주고받을 수 있다. 하지만 HTTPS를 이용하면 암호화/복호화 과정이 필요하기 때문에 HTTP보다 속도가 느리다(그러나 실 사용에서는 크게 차이는 없다.) HTTPS는 인증서를 발급하고 유지하는데에 추가 비용이 발생한다. 개인정보와 같은 민감한 데이터를 주고 받는다면 HTTPS를 이용해야 하지만, 단순 정보 조회 같은 사이트는 HTTP를 적용하면 된다.

- OOP의 특징에 대해서 설명하시오.

객체지향프로그래밍은 컴퓨터 프로그래밍 패러다임 중 하나로, 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고, 그 객체들간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방법으로 OOP의 장점은 코드 재사용성이다. 클래스를 한번 만들어 놓으면 계속 이용 가능하고, 상속을 통해 확장 가능하다. 수정해야할 부분이 클래스 내부에 멤버 변수 혹은 메서드로 있기 때문에 해당 부분만 수정하면 되어 유지보수가 쉽다. 단점은 처리속도가 느리고, 객체가 많으면 용량이 커진다는 것이다. OOP의 특징으로는 클래스와 객체, 캡슐화, 상속 등이 있다. 클래스는 집단에 속하는 속성과 행위를 변수와 메서드로 정의한 것이고, 객체 즉 인스턴스는 클래스에서 정의한 것을 토대로 실제 메모리 상에 할당된 데이터이다. 상속은 부모 클래스의 속성과 기능을 그대로 이어받아 사용할 수 있게 하고, 코드의 중복을 없애기 좋다.