- 배열, 객체를 const로 선언했는데 요소나 속성을 추가할 수 있는 이유에 대해서 설명해주세요.

배열과 객체는 참조자료형이기 떄문에 변수에 값 자체가 아닌 주소를 할당하고 const키워드로 선언 및 할당을 하더라도, 해당변수에는 주소만 담겨있기 때문에 요소나 속성을 추가할 수 있습니다. 그리고 새로운 값이 할당되는 것을 방지하고 깔끔하고 안정적인 코드작성이 가능합니다.

- useRef가 필요한 상황을 예시를 들어 설명해주세요.

우선 useRef는 리렌더링을 하지않고 컴포넌트의 속성만 조회 및 수정이 가능합니다. 그래서 포커스, 텍스트 선택영역 또는 미디어의 재생을 관리할때나, 애니메이션을 직접적으로 실행시킬 때, 그리고 서드파티 DOM 라이브러리를 React와 같이 사용할때 useRef가 필요하다고 생각합니다.

- 서드파티란?

plug_in이나 library등을 만드는 회사를 말하는데
개인 개발자나 프로젝트 팀 혹은 업체등에서 개발하는 즉,3자 라이브러리라고 볼 수 있습니다.
