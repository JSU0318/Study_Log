HTML 이란?

Hypertext Markup Language
웹 표준 기술 중 하나 (html / css / javascript)
Client인 Web browser가 인식할 수 있게끔 만들어둔 document (형식/구조가 있음)
웹 콘텐츠의 구조와 의미를 정의하고 부여하는 마크업 언어
마크업 언어 : 마크업 언어(Markup Language)는 문서가 화면에 표시되는 형식을 나타내거나 데이터의 논리적인 구조를 명시하기 위한 규칙들을 정의한 언어
웹 브라우저 : Chrome, Safari, Internet explorer 같은 웹페이지를 표시해주는 공간
URL : 서버 주소를 노출 시키지 않도록, 웹 브라우져에서 서버에 연결하고자 할 때 쓰는 경로
DOM 구조

문서 객체 모델 (The Document Object Model)
웹 페이지를 파싱하고, 해석하는 전체 모델을 지칭함
HTML의 구조

html은 opening tag, content, closing tag로 이루어져 있으며 이러한 조합을 요소라고 부른다.

기본 tag 구성
tag는 고유 속성을 갖고 있다. 이는 각 tag에 이벤트를 따로 걸고 구분할 수 있기 위함이다.

tag 속성

CSS란?

Cascading Style Sheets
태그들에게 스타일 효과를 주는 언어
구성 : 선택자 {속성명:속성값 ; 속성명:속성값;}
선택자 : 효과가 어떤 태그에 적용되는지를 정의하는 문법이 필요하게 되는데, 이때의 문법을 선택자 라고함
선택자는 3가지로 구성되어 있다 : 태그 선택자, id 선택자, class 선택자
태그 선택자 : 해당되는 태그 전부에 적용
id 선택자 / class 선택자 : 태그에서 설정한 id나 class 속성에 따라 스타일을 지정
Class : 공통 엘리먼트 지정, 한번에 여러 태그들 동시에 적용 가능
.Class{속성명:속성값 ; 속성명:속성값;}
Id : 특정 엘리면트 지정, 특정한 하나만 선택하고 싶을 때, class 선택자보다 id 선택자가 우선적으로 적용
#Id{속성명:속성값 ; 속성명:속성값;}
Margin & Padding

Margin : 바깥쪽 여백 / 부모로부터 떨어져있는 정도
Padding : 안쪽 여백 / 자신과 자식 요소 사이의 여백
