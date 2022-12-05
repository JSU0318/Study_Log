Chapter 3
3-1 if 조건문

if 조건문이란?
조건에 따라서 코드를 실행하거나 실행하지 않을 때 사용하는 구문이다
이때 조건은 불 자료형을 의미한다 비교연산자와 논리 연산자를 활용해 조건을 만들어
이 조건을 사용해 조건 분기를 하는 것을 말한다

if( 불 값이 나오는 표현식 ) {
불 값이 참일 때 실행할 문장
}

```
<script> // 시간은 0~23 12이상부터 오후로 인식함
       const date = new Date()
       const hour = date.getHours()

       if (hour < 12) {

        alert('오전입니다.')
       }
       if (hour >=12) {

        alert('오후입니다.')
       }

    </script>
```

```
if else 조건문이란?
오전과 오후처럼 서로 반대되는 조건을 좀 더 편리하게 조건문을 사용할 수 있도록 상황을 표현하는 구문이다. else구문은 if 조건문 바로 뒤에 붙여 사용한다.

if( 불 값이 나오는 표현식 ) {
불 값이 참일 때 실행할 문장
} else {
불 값이 거짓일 때 실행할 문장
}
```

```
<script> // 조건을 2개를 만들지 않고 if else를 씀으로써 if조건에 참이라면 오전 나머지는 전부 오후라고 나타냄
       const date = new Date()
       const hour = date.getHours()

       if (hour < 12) {

        alert('오전입니다.')
       } else {


        alert('오후입니다.')
       }

    </script>
```

```
중첩조건문이란?
조건문 안에 조건문을 중첩해서 사용하는 것을 중첩조건문이라한다

if( 불 값이 나오는 표현식 1 ) {
if ( 불 값이 나오는 표현식 2 ) {
표현식 2가 참일 때 실행할 문장
} else {
표현식 2가 거짓일 때 실행할 문장
}
} else {
if( 불 값이 나오는 표현식 3) {
표현식 3이 참일 때 실행할 문장
} else {
표현식 3이 거짓일 때 실행할 문장
}
}
```

```
<script> // 10시까진 아침 , 12시부터 3시까지 점심, 그 외는 저녁먹을시간의 중첩 조건문
       const date = new Date()
       const hour = date.getHours()

       if (hour < 11) {

        alert('아침 먹을 시간입니다..')
       } else {


        if (hour < 15) {

            alert('점심 먹을 시간입니다.')

       } else {

        alert('저녁 먹을 시간입니다.')
        }
       }

    </script>
```

```
3-2 switch 조건문과 짧은 조건문

switch 조건문의 기본 형태이다. default는 생략가능

<script>
switch (자료) {
	case 조건A:
    	break
    case 조건B:
    	break
    case default: // default - 생략가능
    	break
</script>
<script> // 변수선언
       const input = Number(prompt('숫자를 입력하세요', '숫자'))

       // 조건문

    switch (input % 2) { // 나머지 연산자 사용하여 홀수,짝수 구분
        case 0:input
            alert('짝수입니다.')
            break // break를 구문마다 걸쳐주지 않으면 연속적으로 출력된다
            	  // ex) 짝수입니다, 홀수입니다, 숫자가 아닙니다.
        case 1:
            alert('홀수입니다.')
            break
        default:
            alert('숫자가 아닙니다.')
            break
    }
    </script>
```

실행결과는 2라고 치면 짝수가 나오고 81치면 홀수가 나온다.

<center>

2의 실행결과

![img](https://velog.velcdn.com/images/dnr0000/post/bb1dac94-3fe3-42a1-ae89-daeefd632444/image.png)

![img](https://velog.velcdn.com/images/dnr0000/post/b76baebb-2011-429a-a67c-9421da419a0f/image.png)

81의 실행결과

![img](https://velog.velcdn.com/images/dnr0000/post/51d2620e-c944-4e0b-9e5f-131d0a810ab5/image.png)

![img](https://velog.velcdn.com/images/dnr0000/post/774106ee-1688-44c0-95c6-648e7134f735/image.png)

</center>

```
조건부 연산자란?

조건문과 비슷한 역할을 하는 연산자다 <조건부 연산자 = 삼항 연산자 (유일)

불 표현식 ? 참일 때의 결과 : 거짓일 때의 결과

<script> // 0보다 이상이면 '0 이상의 숫자입니다' 반대로 음수라면 '0보다 작은 숫자입니다.'
    const input = prompt('숫자를 입력해주세요.','')
    const number = Number(input)

    const result = (number >= 0) ? '0 이상의 숫자입니다.' : '0보다 작은 숫자입니다.'
    				    ^						^					^
                      조건주제 		    0이상의 숫자이거나        그게아니라면?
    alert(result)
    </script>
```

```
짧은 조건문
< 논리합 연산자를 사용한 짧은 조건문 >

논리합 연산자를 사용한 표현식 뒤에 어떠한 값이 들어가도 항상 참이다

true || OOO

true || console.log('실행될까요?')
true
false || console.log('실행될까요?')
실행될까요?
// 좌변 우변 중 우변을 실행한다
undefined

즉, 좌,우변 중 한쪽이 참인것을 출력한다 거짓은 무시한다

불 표현식 || 불 표현식이 거짓일 때 실행할 문장

< 논리곱 연산자를 사용한 짧은 조건문 >

논리곱 연산자를 사용한 표현식은 양변이 모두 참일 때만 참이다

false && OOO

즉, 반대로 논리곱 연산자는 좌변이 거짓이면 우변을 실행하지 않는다

결과가 거짓인 불 표현식 && 불 표현식이 참일 때 실행할 문장
```

```
짝수와 홀수 구분하기 프로그램 만들어보자
(1)

<script>

    const 입력 = prompt('정수를 입력하시오','')
    const 끝자리 = 입력[입력.length - 1] // 0부터 시작하기에 끝자리에 -1을 해줘야 정상출력됨

    //끝자리 비교
    if (끝자리 === "0" ||
    끝자리 === "2" ||
    끝자리 === "4" ||
    끝자리 === "6" ||
    끝자리 === "8") {
        alert(`${입력}은 짝수입니다.`)
    }   else {
        alert(`${입력}은 홀수입니다.`)
    }
    </script>
(2)

<script>
// (1)보다 간단함짝수만 조건 내어주고 그외에는 거짓이기 때문에 홀수를 나타냄
    const 입력 = prompt('정수를 입력하시오','')
    const 숫자 = Number(입력)

    //끝자리 비교
    if (숫자 % 2 === 0) {
        alert(`${입력}은 짝수이다.`)
    } else {
        alert(`${입력}은 홀수이다.`)
    }
    </script>
태어난 연도를 입력받아 띠 출력하기

<script>
    rawInput = prompt('태어난 해를 입력해주세요','')
    const year = Number(rawInput)
    const tti = '원숭이,닭,개,돼지,쥐,소,호랑이,토끼,용,뱀,말,양'.split(',')

    alert(`${year}년에 태어났다면 ${tti[year % 12]} 띠입니다.`)
    </script>
```
