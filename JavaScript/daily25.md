- use strict 이 무엇인가요? 사용시 장단점이 무엇인가요?

  자바스크립트 언어의 문법을 보다 엄격히 적용하여 기존에는 무시되던 오류를 발생시킬 가능성이 높거나 자바스크립트 엔진의 최적화 작업에 문제를 일으킬 수 있는 코드에 대해 명시적인 에러를 발생시킨다. 전역에서 선언하면 모든 소스코드가 대상이고, 로컬로 선언하면 함수 내에서만 대상이 된다. use strict 모드에서는 삭제가 불가능한 프로퍼티를 삭제하거나 함수의 매개변수를 중복해서 사용하는 것 등이 금지된다.
  코드의 문제를 더 빨리 알게되기에 디버깅이 쉬워지고 실수로 전역변수를 만드는 것이 불가능하지만, 단점으로는 엄격모드를 지원하지 않는 브라우저에서는 엄격 모드의 코드가 다른 방식으로 동작할 수 있다는 것이다.

- Box model에 대해 설명해주세요.
  모든 HTML 요소는 BOX모양으로 구성되며, 이것을 박스모델이라고 한다. 문서의 레이아웃을 계산할 때, 브라우저의 렌더링 엔진은 표준 CSS 기본 박스 모델에 따라 각각의 요소를 사각형 박스로 표현한다. 박스 모델은 총 네 부분(영역)으로 이루어지고, 이 네가지 부분은 패딩, 테두리(border), 마진, 내용(content)로 구분한다. 내용은 텍스트나 이미지가 들어가있는 박스의 실질적인 부분으로 색상, 너비, 높이 등을 지정할 수 있다. 패딩은 내용과 테두리 사이의 간격이다. 패딩은 눈에 보이지 않는다. 테두리(border)는 내용과 패딩 주변을 감싸는 테두리이다. 마진은 테두리와 이웃하는 요소 사이의 간격이고 마진은 눈에 보이지 않는다.