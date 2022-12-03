Chapter 2
2-1 기본 자료형

프로그래밍에서 프로그램이 처리할 수 있는 모든 것을 자료라고한다.

기본적이면서 많이사용하는 자료형

```
숫자
문자열
불
문자열 자료형
alert(), console.log() 이와 같은 문자들의 집합을
"문자열"이라고 함
문자가 하나든 여러개든 모두 문자열 자료형 이라고함
```

이스케이프 문자란?
\n : 줄바꿈
\t : 탭
\\ : 역슬래시 그자체

```
문자열 연산자

문자열 + 문자열 = 문자열 연결 연산자
'가나다' + '라마' + '바사아' >> "가나다라마바사아"
문자열 길이 구하는법

문자열 뒤에 온점(.)을 찍고 length 입력
"안녕하세요".length / " ".length >> 빈문자열도 문자열임
Uncaught SyntaxError: Unexpected identifier

식별자가 예상하지 못한 위치에서 등장했다는 오류
숫자 자료형

숫자는 소수점이있는 숫자와 없는 숫자 모두 같은 자료형으로 인식한다 그냥 숫자입력하면 숫자 자료가 만들어진다.
```

```
숫자 연산자

(5 + 3) \* 2 >> 괄호가 있으면 먼저 연산한 후 출력
"%"는 나머지 연산자이다
불(Boolaen) 자료형

참과 거짓을 나타낼 때 사용
true, false >> 2가지
비교 연산자 종류

" === " - 양쪽이 같다
" !== " - 양쪽이 다르다
" > " - 왼쪽이 더 크다
" < " - 오른쪽이 더 크다
" >= " - 왼쪽이 더 크거나 같다
" <= " - 오른쪽이 더 크거나 같다
불 표현식 손코딩해보기
```

```
<script>
	if (273 < 52) {
    alert('273은 52보다 작습니다.')
    }
    if (273 > 52) {
    alert('273은 52보다 큽니다.')
    }
</script>
```

ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

실행결과

```
273은 52보다 큽니다.
불 부정 연산자

앞에 " ! " 기호를 넣으면 참을 거짓으로 거짓을 참으로 바꿈
단,이,삼항연산자

!true 결과 : false // 피연산자가 true 1개로 단항
10 + 20 결과 : 30 // 피연산자가 10과 20 2개로 이항
true ? 10 : 20 결과 : 10 // 피연산자가 true,10,20 3개로 삼항
```

```

불 논리합/논리곱 연산자

&& = 논리곱 연산자 >> 양쪽 변의 값이 모두 true 일때 true 결과
|| = 논리합 연산자 >> 양쪽 변의 값 중 하나만 true여도 true
자료형 검사 typeof 연산자

typeof('문자열') // 결과 = "string"
typeof(273) // 결과 = "number"
typeof(true) // 결과 = "boolean"
템플릿 문자열

템플릿 문자열은 백틱( ` )으로 문장을 감싸만든다
${555+55}이런식으로 표현식을 넣으면 표현식 안 에서 연산 시켜준다
2-2 상수와 변수

상수 = '항상 같은 수'라는 의미로 값에 이름을 한 번 붙이면 값을 수정할 수 없다
변수 = '변할 수 있는 수'로 값을 수정할 수 있다

상수
const 뒤에 문자를 붙이면 선언이된다 ex) const pi
pi라는 내가 정한 이름의 상수가 되는것이다
상수 구문오류

Idendifier has already declared
상수는 한 파일에서 한번만 선언가능하지만 만약 같은 이름으로 상수를 한 번 더 선언하면 위와 같은 오류가 발생

Missing initializer in const declaration
선언할 때 반드시 값을 지정해줘야한다. 변수와 달리 선언하고 값을 지정해야하며 지정안해준다면 위와 같은 오류 발생

Assignment to constant variable
상수는 값 지정하면 변경 못시키기 때문에 값을 변경시키면 위와 같은 오류 발생

변수
let 뒤에 문자를 붙이면 선언된다 ex) let a
a라는 내가 정한 이름의 변수가 되는것이다
값을 상수와 같이 지정해 줄 수도있고 값을 넣지않고 선언만도 가능

변수 구문오류

Identifier has already been declared
상수와 마찬가지로 특정한 이름의 변수는 한 파일에서 한 번만 선언할 수 있다 똑같이 한번더 선언하면 위와 같은 오류가 뜬다
하지만 nameA, nameB 이렇게 식별자를 사용하면 해결 가능하다
복합 대입 연산자 종류

+= 기존 변수의 값에 값을 더한다
-= 기존 변수의 값에 값을 뺀다
\*= 기존 변수의 값에 값을 곱한다
/= 기존 변수의 값에 값을 나눈다
%= 기존 변수의 값에 나머지를 구한다
증감 연산자

변수++ 기존의 변수 값에 1을 더합니다(후위)
++변수 기존의 변수 값에 1을 더합니다(전위)
변수-- 기존의 변수 값에 1을 뺍니다(후위)
--변수 기존의 변수 값에 1을 뺍니다(전위)
2-3 자료형 변환
```

문자열 입력
함수는 prompt() 이다
prompt(메시지 문자열, 기본 입력 문자열)

```
<script>
	const input = prompt('message', '_default')
    //prompt()함수는 사용자로부터 내용을 입력받아서 사용한다
    //웹 페이지에서 입력할 수 있는 창이 나타나면 거기에 입력을 받는것
    alert(input)
</script>
```

![img](https://velog.velcdn.com/images/dnr0000/post/d398862c-a906-4453-9a6b-8a215480aadb/image.png)

입력한 값을 그대로 받아와 출력해낸다

![img](https://velog.velcdn.com/images/dnr0000/post/0e271ed1-7cc6-45a4-b3a3-e75318804c16/image.png)

불 입력
confirm() 함수를 사용한다 이 함수는 prompt()와 비슷한 형태로 사용한다
confirm(메시지 문자열)

```
<script>
        const input = confirm('수락하시겠습니까?')
       // 웹페이지에는 확인과 취소 즉 true,false 단답형 yes or no이다
        alert(input)
    </script>
```

![img](https://velog.velcdn.com/images/dnr0000/post/5231e0d8-3668-49cc-bbf0-c5b4f1fd957c/image.png)

수락한다면 true 취소한다면 false 출력

![img](https://velog.velcdn.com/images/dnr0000/post/a5cc13df-583a-447a-ba56-379bbeedce4c/image.png)

숫자 자료형으로 변환하기

Number() 함수를 사용한다
Number(자료)

```
Number("273")
결과 : 273
typeof(Number("273"))
결과 : "number" // 자료형은 숫자다
```

NaN(Not a Number) 라는 값을 출력할 경우 자바스크립트에서 숫자이지만, 숫자로 나타낼 수 없는 숫자를 뜻한다.

Number() 함수를 사용하지 않고도 바로 숫자연산자를 사용하면 숫자 자료형으로 변한다

```
ex) "52" - 0
52
typeof("52" - 0)
"number"
```

문자열 자료형으로 변환하기
다른자료를 문자열 자료형으로 변환할때는 String() 함수를 사용한다
String(자료)

```
ex) String(52.273) 이라 입력하면 문자열로 출력해줌
"52.273"
String(true)
"true"
String(false)
"false"
```

```
불 자료형으로 변환하기
Boolean() 함수를 이용하며 대부분 true로 변환되지만
0,NaN,'',"",null,undefined는 false로 변환된다
위의 5개는 꼭 외워서 기억하자!

Boolean()을 사용하지 않고 논리부정연산자(!)를 사용해서 다른 자료를 불자료형으로 변환시킬수 있다.
"!!" 두번사용하여야 한다
```

```
ex) !273
true
!!0
false
!!'안녕하세요'
true
!!''
true
```

```
<script>
        const rawInput = prompt('inch 단위의 숫자를 입력해주세요.')

        //prompt로 입력받은 데이터를 숫자형으로 변경하고 cm 단위로 변경시킨다
        const inch = Number(rawInput)
        // 상수에 선언한 자료 rawInput을 넣고 상수 cm을 만들어
        // inch를 어떤값으로 변경시킬지 값을 입력한다
        const cm = inch * 2.54

        //그 다음 출력할 수 있게 alert해준다
        alert(`${inch}inch는 ${cm}cm 입니다.`)
    </script>
```

실행시켜보자

![img](https://velog.velcdn.com/images/dnr0000/post/e4c03c0b-efe4-4867-a671-3d98c16f904d/image.png)

prompt를 이용했으므로 입력받을 수 있는 창이 뜬다

![img](https://velog.velcdn.com/images/dnr0000/post/cf5688fd-53fa-4025-a3c0-27b8ec0cd878/image.png)

그리고 임의로 50인치를 테스츠 해보았는데 127cm로 제대로 출력되었다
