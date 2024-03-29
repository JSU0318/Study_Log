- 고차 컴포넌트(HOC)란? 사용해본 적 있는지?

  고차 컴포넌트는 컴포넌트를 취하여 새로운 컴포넌트를 반환하는 함수입니다. 즉 리액트 컴포넌트를 인자로 받아서 새로운 리액트 컴포넌트를 리턴하는 함수이다. 컴포넌트 로직을 재사용하기 위한 아주 고오급 리액트 기술이고, 유저 인증 로직 처리 혹은 로딩 중 화면 처리, 컨테이너 컴포넌트와 프레젠테이션 컴포넌트를 분리하는 등에 자주 활용된다. 나는 유저 인증 로직을 처리할때 사용해보았다.

- 이벤트 바인딩이란?

  이벤트 바인딩이란, 발생하는 이벤트와 그 후에 어떤일이 일어나는지 알려주는 콜백함수와 연결해준 다는 뜻이다. 이벤트 바인딩이는 총 3가지 방법이 있는데, HTML이벤트 핸들러, 전통적인 DOM핸들러, EventListener을 이용한 핸들러가있다. HTML핸들러는 HTML요소의 이벤트 Attribute에 이벤트 핸들러를 넣는 방식이다. 현재에서는 지양하는 방식이고, HTML과 JS가 혼용될 수 있는 문제가 생긴다. 전통적인 DOM이벤트 핸들러는 HTML과 JS가 혼용되는 문제를 해결했으나, 이벤트 핸들러에 하나의 함수만 바인딩 할 수 있고, 함수에 인수를 전달하지 못하며, 바인딩 된 이벤트 핸들러가 2개 이상인 경우 제일 마지막에 추가다된 코드의 이벤트 핸들러만 실행된다.앞에서 설명한 것의 단점을 보완하기 위해 만든 것이 EventListener을 이용한 이벤트 핸들러이인데, addEventListener함수를 이용하여 대상 요소에 이벤트를 바인딩하고, 해당 이벤트가 샐행될 콜백함수를 지정한다.하나의 이벤트에 대해 다수의 핸들러를 추가할 수 있고, 캡쳐링과 버블링을 지원하며 HTML뿐만 아니라 DOM요소에도 동작한다는 장점이 있다.
