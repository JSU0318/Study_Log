- var, let, const의 차이점을 설명해주세요.

let과 const는 블록 스코프를 갖고 공통적으로 재선언이 되지 않는다. 그러나 let은 재할당이 가능하고, const는 선언과 동시에 할당이 되기에 재할당이 불가능하다.

- MVC, MVVM 모델에 대해 설명해주세요.

MVC패턴은 모델 + 뷰 + 컨트롤러를 합친 용어이다. 모델은 데이터 및 데이터를 처리하는 부분이고, view는 사용자에게 보여지는 UI 부분이다. 컨트롤러는 사용자의 입력을 받고 처리하는 부분이다. MVC는 사용자의 액션이 컨트롤러에 들어오면, 컨트롤라가 액션을 확인하고 모델을 업데이트한다. 컨트롤러는 모델을 나타내줄 view를 선택하고, view는 모델을 이용하여 화면을 나타낸다. 컨트롤러는 여러개의 view를 선택할 수 있는 1:n 구조이고, 뷰를 선택할 뿐 직접 업데이트는 하지 않는다. 보편적으로 널리 사용되는 패턴이며, 단점은 뷰와 모델사이의 의존성이 높고, 어플리케이션이 커질수록 복잡하고, 유지보수가 어렵다는 점이다.