- Cookie의 MaxAge, Expires 옵션이 무엇인지, 설정하지 않으면 어떻게 되는지 설명해주세요.

Exipires 속성을 사용하면 속성에 정의된 날짜에 삭제되는 쿠키를 만들고 언제 폐기할 것인지 지정하는 옵션이고, Max-Age 속성을 사용하면 속성에 정의된 기간 이후에 삭제되는 쿠키를 만들고 이 쿠키를 얼마나 유지할것인지 지정하는 옵션입니다. 하지만 이 두 옵션중 만약 설정하지 않는다면 해당 쿠키는 브라우저가 닫힐 때 폐기됩니다. 그래서 빠르게 폐기하고 싶다면 옵션설정을 하지말고, 계속 사용하고 싶다면 두개중 하나라도 설정해주는 것이 좋습니다.

- 순수함수란 무엇인가요? 불변성과 사이드 이펙트와 연결하여설명해주세요.

순수함수란 함수형 프로그래밍에서 오직 함수의 입력만이 함수의 결과에 영향을 주는 함수를 의미하고 사이드 이펙트가 없어야 합니다. 함수 body 내에 있는 코드만 점검하면 되기 때문에 간결하게 코드를 작성하는데 도움이되고 여기서 사이드 이펙트는 외부 변수를 참조하거나 변경하는 모든 종류의 코드를 말하는데 불변성을 지켜야하는 이유로는 값을 직접 변경하지 않고 늘 새로운 값을 리턴한다는 의미라서 이점은 예기치 못한 사이드 이펙트를 방지할 수 있다는 점과 state를 직접변경하지않고 setState를 사용하는 것이 불변성을 지키는 방법입니다.
