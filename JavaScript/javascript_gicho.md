Chapter 1
1-1 자바스크립트의 활용

웹 서버 애플리케이션 개발
C#, 자바, 루비, 파이썬

ㅡㅡ

Node.js

웹 서버 애플리케이션을 개발할 때 꼭 필요한 간단한 모듈만 제공한다.

빠르다 - 다른 스크립트언어 및 프레임워크 개발한 서버 애플리케이션을 노드 1대로 대체가능하다.

유지비용이 낮다

ㅡㅡ

모바일 애플리케이션

안드로이드와 아이폰은 자바/코틀린, 스위프트 프로그래밍 언어로 개발

자바스크립트는 공통된 프로그래밍 언어라 모든스마트폰에서 동작 가능

현재 안드로이드,아이폰에 있는 페이스북, 인스타, 핀터레스트, 우버 등 어플은 모두 자바스크립트로 만든 네이티브 어플이다.

ㅡㅡ

데스크톱 애플리케이션

NW.js 모듈 등으로 데스크톱 애플리케이션 개발에 활용하기 시작함
깃허브에서 NW.js 개발자들을 흡수하여 자바스크립트 개발전용 텍스트 에디터인 아톰을 만들어 배포함

ㅡㅡ

데이터베이스 관리

데이터를 저장할 때 사용하는 프로그램

데이터베이스는 SQL이라는 프로그래밍 언어를 사용해 관리
대표적으로 Oracle, MySQL등 관계형 데이터베이스 관리시스템(RDBMS)는 모두 SQL 프로그래밍 언어를 사용함

Not-Only-SQL이라 불린 NoSQL은 2010년 이후 페이스북, 트위터 등으로 인해 폭발적으로 증가한 빅데이터를 처리하기 위한 기술

그중 MongoDB가 데이터베이스를 관리할 때 자바 스크립트를 활용하는 대쵸적인 NoSQL 데이터베이스이다.

ㅡㅡ

모바일 애플리케이션의 종류

C와 자바를 이용해서 제조사가 추천하는 프로그래밍 언어를 사용해서 만들어진 애플리케이션을 네이티브 앱이라 한다.

웹사이트 화면을 애플리케이션으로 감싸기만 해서 보여주는 모바일 웹 등장, 하지만 성능도 좋지 않고 스마트폰이 가진 기능을 제대로 활용 할 수 없다

보완하고자 중간에 스마트폰의 기능과 웹 페이지를 연결할 수 있는 층을 설치해서 웹사이트가 스마트폰의 기능을 활용할 수 있게 만든 것을 하이브리드 앱이라고 한다.

ㅡㅡ

1-2 개발환경과 코드실행 (VisualStudio .ver)

![img](https://velog.velcdn.com/images/dnr0000/post/5a8b19e6-3b4b-4794-a957-9dcdf997f053/image.png)

콘솔창에서

헬로 자바스크립트...! 가 출력되었다.

console.log("Hello JavaScript...!") // 입력한 코드
VM196:1 Hello JavaScript...! // console.log()로 출력된 내용이다
undefined // 해당 줄의 결과를 나타낸다.
"html:5"를 입력하면 자동완성코드가 뜨는데 수정해보도록 한다

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

![img](https://velog.velcdn.com/images/dnr0000/post/eed0db8c-7561-47fb-bb58-bef007012f4d/image.png)

코드 수정 후 alert 명령어 내려 알람으로 헬로월드가 나온거같다

타자오타로 오류일경우 어떻게 될까

```
<script>
        alrt('Hello world')
    </script>
```

검사로 콘솔에 들어가니 친절하게도 오류를 알려줘서 쉽게 찾을수 있는거 같다!

예상대로 현재작성중인 파일의 8~9번째줄에 문제있다고 표기되는거 같다.

ㅡㅡ

구문 오류 시

Uncaught SyntaxError: Invalid or unexpected token
-> 토큰(기호)을 잘못 입력했을 때나 빼먹었을 때의 오류다. 다음코드는 따옴표를 열었으나 닫지않았을 때 나타난다.

Uncaught SyntaxError: missing ) after argument list
-> 위와 같이 기호문제이지만 괄호를 열고 닫지않았을 때 나타난다.

Uncaught SyntaxError: Invalid left-hand side expression in postfix operation
-> 존재하지 않는 연산자가 들어가면 뜨는 오류다

Uncaught SyntaxError: Unexpected token ')'
-> 빠진 괄호를 알려주면서 오류를 나타내어준다

ㅡㅡ

1-3 알아두어야 할 기본 용어

표현식 = 값을 만들어 내는 간단한 코드

const, 10, +, require, '안녕'
문장 = 표현식이 하나 이상 모인 것

10 +10;, console.log('안녕'), alert('Hello...!)
프로그램 = 문장이 모인 것

const fs = require('fs) fs.readFile('text',(e, c) => { console.log(c)}) 등등
키워드(명령어)는 언어라서 날이갈수록 키워드도 증가하니
외우기보다는 무엇인지 정도만 알고넘어가자!

식별자 = 언어에서 이름을 붙일 때 사용하는 단어이다. 주로 변수명이나 함수명에 사용된다

키워드를 사용하면 안된다
숫자로 시작하면 안된다
특수문자는 \_와 $만 허용한다
공백문자를 포함할 수 없다

주석처리

1. HTML 태그 주석

- `<!-- 이 안의 내용은 주석처리 -->`

2. 한 줄 주석

- // 내용주석

  ㅡㅡ
