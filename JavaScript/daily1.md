웹페이지가 브라우저에 랜더링 되는 과정을 설명해주세요
우선 HTML과 CSS파일을 파싱하여 각각의 Tree를 만들고,
2개의 Tree를 합쳐 RenderingTree를 만들어 각 노드의 위치와 크기를 계산하여 그 값을 이용해 각 노드를 화면상의 실제 픽셀로 변환하고 레이어를 만들고 합성하여 화면에 나타내게됩니다.

Restful API에 대해 설명해주세요.
간단하게 REST 원리를 따르는 시스템은 RESTful이라고 하고, 주된 목적으로는
이해하기 쉽고 사용하기 쉬운 REST API를 만드는것과 성능향상 뿐만 아니라 일관적인 컨벤션을 통한 이해도와 호환성을 높이는게 목적입니다 그리고 성능이 중요한 상황에서는 굳이 RESTful한 API를 구현할 필요가 없습니다.

GET,POST외 알고있는 메소드와 그 기준을 설명해주세요.
이외에 PUT,PATCH,DELETE등이 있고 PUT은 POST와 비슷하지만 리소스의 위치를 알고 URI를 지정해줘야하고 현재 메시지 값으로 생성하거나 만약 존재하는 데이터라면 기존리소스를 삭제하고 덮어쓰기해줍니다. 그리고 PATCH는 리소스를 부분적으로 변경할때 쓰며 보통 여러 정보를 데이터 전송할 때 하나만 수정해서 데이터를 저장시키고싶다 할때 사용하고, 예로는 회원정보수정 등에 쓰입니다, 그리고 DELETE는 말그대로 리소스의 삭제를 요청하는데 예로는 회원탈퇴 등이 있습니다.

RESTful API 가 아닌것들은 어떤게있나요?
각 구성요소들의 역할이 완벽하게 분리되어있는 경우가 아니거나 가독성이 떨어지고, 파일확장자가 URI에 포함되거나 한다면 RESTful API가 아닙니다.
CRUD 기능을 모두 POST로만 처리한다거나 route에 리소스, 아이디 외의 정보들이 들어가는경우는 RESTful 하지 않다고 할 수있습니다.
