Vue.js란 무엇인가?
MVVM 패턴의 ViewModel 레이어에 해당하는 화면단 라이브러리

View Model Layer

데이터 바인딩과 화면 단위를 컴포넌트 형태로 제공하며, 관련 API 를 지원하는데에 궁극적인 목적이 있음
Angular에서 지원하는 양방향 데이터 바인딩 을 동일하게 제공
하지만 컴포넌트 간 통신의 기본 골격은 React의 단방향 데이터 흐름(부모 -> 자식)을 사용
다른 프런트엔드 프레임워크(Angular, React)와 비교했을 때 상대적으로 가볍고 빠름.
문법이 단순하고 간결하여 초기 학습 비용이 낮고 누구나 쉽게 접근 가능
MVVM 패턴이란?
위키에 명시된 것처럼, Backend 로직과 Client 의 마크업 & 데이터 표현단을 분리하기 위한 구조로 전통적인 MVC 패턴의 방식에서 기인하였다. 간단하게 생각해서 화면 앞단의 회면 동작 관련 로직과 뒷단의 DB 데이터 처리 및 서버 로직을 분리하고, 뒷단에서 넘어온 데이터를 Model 에 담아 View 로 넘어주는 중간 지점이라고 보면 되겠다.

mvvm-pattern

Vue.js 시작하기
다른 주요 프런트엔드 프레임워크(Angular, React)와 비교했을 때 뷰위 가장 큰 강점은 바로 시작하기가 정말 쉽다는 점이다.

<!DOCTYPE html>
<html>
  <head>
    <title>Vue.js Sample</title>
  </head>
  <body>
    <div id="app">
      {{ message }}
    </div>

    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    <script>
      new Vue({
        el: "#app",
        data: {
          message: "Hello Vue.js!"
        }
      });
    </script>

  </body>
</html>
HTMLCopy
CDN으로 코드 땡겨오고 바로 Vue 인스턴스를 하나 생성하여 간단한 페이지를 만들어보았다. 기존의 구현된 시스템에 적용하기도 훨씬 수월할 것으로 보인다.
