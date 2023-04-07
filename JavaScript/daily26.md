- Prototype이란? Prototype Chaining은?

  프로토타입이란 객체가 만들어지기 위해서는 자신을 만드는데 사용된 원형인 프로토타입 객체를 만든다. 이때 만들어진 객체 안에 **proto** 속성이 자신을 만들어낸 원형을 의미하는 프로토타입 객체를 참조하는 숨겨진 링크가 있다. 그 링크를 프로토타입이라고 한다. 어떤 데이터의 **proto** 프로퍼티 내부에서 다시 **proto** 프로퍼티가 연쇄적으로 이어진것을 프로토타입 체인(prototype chain)이라 하고, 이 체인을 따라가며 검색하는 것을 프로토타입 체이닝(prototype chaining) 이라고 한다.

- undeclared 란? (null, undefined와 비교)

  undefined과 null의 차이는 둘다 선언은 되어있지만, 값의 할당 차이

  Undefined: 접근 가능한 스코프에 변수가 선언되었으나 현재 아무런 값도 할당되지 않은 상태
  var amy; console.log(amy) => undefined

Undeclared: 접근 가능한 스코프에 변수 선언조차 되어있지 않은 상태.

Null: 변수를 선언하고 "null" 이라는 빈값을 할당한 경우 (null은 객체임)
var amy; (선언), amy = null; (할당)

- forEach와 Map의 차이점은?

  두 메소드 다 배열의 모든 원소를 돌면서 해당 요소에 관한 작업을 실행하는데, forEach는 원본을 변경시키는데, map은 새로운 배열을 반환한다.

- 이벤트 루프란?

  싱글 스레드 기반의 언어인 자바스크립트는 이벤트 루프를 이용해서 비동기 방식으로 동시성을 지원한다. 이벤트 루프는 콜스택과 콜백큐의 상태를 체크하여, 콜 스택이 빈 상태가 되면 콜백 큐의 첫번째 콜백을 콜 스택으로 밀어주는 역할을 한다. 즉, 자바스크립트 엔진이 코드 조각을 하나씩 처리할 수 있도록 작업을 스케쥴하는 동시에 JS에서 비동기 작업을 처리할 수 있게 해준다. 모든 비동기 방식의 API들(setTimeout, ajax 등)은 이벤트 루프를 통해 콜백 함수를 실행한다고 볼 수 있다.