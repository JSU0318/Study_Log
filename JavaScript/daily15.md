- Flex 속성을 설명해주세요.

Flexbox란 기존 컨텐츠를 수평으로 배치할 때, float나 inline-block으로 마크업할때의 불편함을 쉽게 해결할 수 있도록 추가된 기능이다. 다양한 디바이스 환경에서 언제나 똑같은 레이아웃을 유지시켜줌으로써 반응형 웹 사이트에 유용하게 쓰인다. Flex는 컨텐츠를 감싸는 상위 부모요소인 Flex Container와 각 컨텐츠들인 자식요소 Flex Item으로 구성되어있다. Flexbox css 적용방법은 부모요소인 container에 display:flex를 선언하면 된다. Flex Container에는 전체적인 정렬과 관련된 속성인 display, flex-direction, align-items, flex-wrap 같은 속성을 정의하고, 자식요소인 flex item에는 flex-grow, flex-shrink 같은 크기나 순서 같은 속성을 정의한다.

- 주소창에 naver.com을 입력하면 생기는 일

사용자가 입력한 url 주소 중에서 도메인 네임을 DNS 서버에서 검색한다. -> DNS 서버에서 해당 도메인 네임에 해당하는 IP주소를 찾아 사용자가 입력한 URL 정보와 함께 전달함. -> 웹 페이지 URL + IP 주소는 HTTP 프로토콜을 사용하여 HTTP 요청 메세지를 생성한다 -> HTTP 요청 메세지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 해당 IP 주소의 컴퓨터로 전송된다 -> 이렇게 도착한 HTTP 요청 메세지는 HTTP 프로토콜을 사용하여 웹 페이지 URL 정보로 변환된다. -> 웹 서버는 도착한 웹 페이지 URL 정보에 해당하는 데이터를 검색한다 -> 검색된 웹 페이지 데이터는 또다시 HTTP 프로토콜을 사용하여 HTTP 응답 메세지를 생성한다 -> 이렇게 생성된 HTTP 응답 메세지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 원래 컴퓨터로 전달된다. -> 도착한 HTTP 응답 메세지는 HTTP 프로토콜을 이용하여 웹 페이지 데이터로 변환되고, 웹 브라우저에 의해 출력되어 사용자가 볼 수 있게 된다.
