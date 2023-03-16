- Promise란?

비동기 동작을 다루기 위한 패턴으로, 비동기 요청을 보내면 성공 또는 실패가 다양한 형태로 발생한다. 프로미스를 사용하면 이러한 성공(resolve)이나 실패(reject)를 편리한 방식으로 환원할 수 있다. new 연산자와 함께 호출한 promise의 인자로 넘겨주는 콜백함수는 호출할 때 바로 실행, 그 내부에 resolve 또는 reject 함수를 호출하는 구문이 있으면 둘 중 하나가 실행되기 전까지는 다음 then or catch 구문으로 넘어가지 않는다. pending, fulfilled, rejected 3가지 상태를 가진다.

- Async, Await와 Promise의 차이는?

promise를 사용할 때는 .catch()문으로 에러 핸들링 가능 but async/await은 에러 핸들링 기능이 따로 없어 try-catch() 문을 활용해야한다.
promise는 .then() 지옥의 가능성이 있어, 코드가 길어질수록 async/await문을 사용하면 가독성이 좋다.
