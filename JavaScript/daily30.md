- 원시값과 참조값(array, object)의 차이점을 메모리 관점에서 설명해주세요

  원시값은 복제할 때 값이 담긴 주솟값을 바로 복제하고, 참조형은 값이 담긴 주소값들로 이루어진 묶음을 가리키는 주솟값을 복제한다. 원시값은 불변값이므로 원시값을 재 할당하면 새로운 메모리 공간을 확보하고 재 할당한 값을 저장하고 참조하던 메모리 공간 주소를 변경한다. 참조값은 가변값이므로 객체가 할당된 메모리 공간에는 실제 객체의 주소가 저장된다. 객체를 할당한 변수는 재할당없이 객체를 직접 변경할 수 있다. 프로퍼티를 동적으로 추가할 수 있고, 갱신, 삭제도 가능하다.

- 리액트의 useCallback, useEffect등을 사용할 때 의존성 배열을 받게 됩니다. 이 배열의 역할은 무엇인가요?

  useEffect의 의존성 배열은 두 번째 매개변수로, 의존성 배열의 내용이 변경되었을 경우, 부수 효과 함수(이펙트 함수)가 실행된다. 의존성 배열안의 값이 바뀔때만 렌더링 되는 특성을 이용해 state 혹은 props값이 변경될 때 특정 함수를 실행하거나, 컴포넌트가 마운트 될 때 API를 이용해 데이터를 가져오거나 하는데 사용된다. 빈 배열을 넣게 되면 최초 마운트 될 때 한번만 호출되도록 할 수 있다. 이펙트 내부에서 사용되는 모든 변수는 deps에 명시를 해야 버그가 발생하지 않는다.
  useCallback은 특정 함수를 새로 만들지 않고 재사용하고 싶을 때 사용하는 훅으로 함수 안에서 사용하는 상태나 props가 있다면 의존성 배열에 추가하게 된다. 추가하지 않으면 함수 내에서 해당 값들을 참조할 때 가장 최신의 값을 참조할 것이라는 보장이 없다. 의존성 배열에 넣은 값이 변할 때만 함수를 새로 만들게 된다.

- "attribute"와 "property"의 차이점은 무엇인가요?

  Attributes는 HTML 요소의 추가적인 정보를 전달하고 이름="값" 이렇게 쌍으로 온다. 예를들어 <div class="my class"></div> 를 보면 div 태그가 class라는 값이 "my class"인 attribute를 가지고 있다.
  Property는 attribute에 대한 HTML DOM트리 안에서의 표현이다. 같은 예시에서 attribute는 값이 "myclass"이고 이름이 className인 property를 가진다.
  둘의 차이는 Attribute는 HTML 텍스트 문서에 있는 것이고, property는 HTML DOM 트리에 있는 것이다. attribute는 변하지 않고, property는 변할 수 있다. 가령 사용자가 체크박스를 체크하면 property의 값은 변하는 것이다.(DOM안에 존재하고 동적이기 때문에)
