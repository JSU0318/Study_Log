- ESLint에 대해 설명해주세요.

  자바스크립트 언어와 소스코드를 분석하는 도구로 eslint패키지를 설치해주면 코드에 특정 스타일과 규칙을 적용해 에러를 찾고 패턴을 적용시킬 수 있는 분석 툴이다. 사용시 ECMAScript코드에서 문제점을 검사하고 일부는 더 나은 코드로 정정해주는 유용한 도구이다. 코드의 가독성을 높이고 잠재적인 오류와 버그를 제거해 단단한 코드를 만드는 것이 목적이다. 추가로 코드를 더 보기좋도록 포맷팅 해주는 prettier를 ESLint와 함께 사용해주면 더 효율적이다.

- ES6 문법에 추가된 것들을 아는대로 설명하세요

  String Literal, 객체 비구조화, 객체 리터럴, for .. of, Spread Operator, Rest Parameter, Arrow Function, Default Params, let & const, import & export, Map & Set

- DOM 과 가상 DOM이란?

  Document Object Model 의 약자로, HTML, XML 문서의 프로그래밍 인터페이스를 의미한다. HTML은 브라우저에서 실행될 수 있게끔 DOM Tree로 파싱되고, 이를 바탕으로 렌더링이 된다. 가상돔은 추상화된 DOM을 뜻한다. 기존 DOM을 조작하고 렌더링하는 부분에서 오는 시간을 줄인다. DOM과 유사한 객체를 메모리에 올려놓고, 변경 사항이 생기면 가상돔을 바꾸고, 실제 돔에서는 변경 사항만 변경하여 더 반응성 빠른 웹을 구현할 수 있다. 리액트도 가상돔을 이용하여 구현되어있다.
