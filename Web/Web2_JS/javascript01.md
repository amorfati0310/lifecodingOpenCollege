# Web2수업 OverView 

## 01 HTML과 JS 만남 :D 

## Javascript 란 무엇인가ㄴ

Javascript 는 Brendan Eich 라는 분이 1995년에 달랑 10일 만에 만든 언어다.
크로스-플랫폼  [객체지향언어](http://blog.daum.net/istae0430/194)다.
일반적인 용도는 웹 페이지에 기능을 더해 HTML 를 동적으로 만드는 것이다.
현재는 클라이언트와 서버 양쪽 모두에서 범용적으로 사용되고 있다.

인터프리터 언어 동시통역, 바로바로 처리 
컴파일 언어 번역 쭈욱 -> 슥슥 , 속도 빠르나 컴파일 시간

1. JS는 동적
`document.wrtie 문서에 출력할 때 쓴다.`

`script태그를 js를 쓸 떄 쓴다`

## HTML 과 JS 만남 02 Event 

```

<body>
    <input type="button" value="hi" onclick="alert(hi")">
</body>

이벤트가 일어났을 때, 자바스크립트가 실행하도록 하는 것 
배운 event 
onClick 
onChange
onKeydown
대략 10개 20개 
```

## HTML 과 JS 만남 03 Console

파일을 만들지 않고도 즉시 실행할 수 있음 
> Repl환경 

`const letter = alksjdlkasdj`
`letter.length` 글자수 체크  
<br>
element에서 esc키 누르면 

[기스트_이고잉님](https://gist.github.com/egoing)
기스트가 뭐지?
```
var 당첨자수 = 2;
var 댓글선택자 = '._3b-9>div>.UFIComment .UFICommentActorName';
function shuffle(a) {
    for (let i = a.length; i; i--) {
        let j = Math.floor(Math.random() * i);
        [a[i - 1], a[j]] = [a[j], a[i - 1]];
    }
}
var list = [];
document.querySelectorAll(댓글선택자).forEach(function(e){
	list.push(e.innerText);
});
list = list.filter((v,i,a) => a.indexOf(v)===i);
shuffle(list)
console.log(list.slice(0,당첨자수));


```


## Data type 자료형 

[자바스크립트 데이터 타입](https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures)

* Six primitive type (Boolean, Null, Undefined, Number, String, Symobl )<br>
Object
* Reference type
1. fn
1. object
1. Array 

> 콘솔로 연습해보기
숫자 연산 
String.length
String.toUpperCase
String.indexOf() -1 찾을 수 없다.
String.trim()


## 변수와 대입 연산자 

변수 변하는 수 바뀔 수 있는 값
= 대입하는 의미 왼쪽에 상자에 오른쪽 걸 대입합니다.

변수를 왜 쓰는가 
1. 직관적으로 끊어 쓸 수 있고 , 의미있게 저장  
2. 재사용성 겹치는 부분 !!!

## 웹브라우저와 제어  

## CSS 기초

div, spann  무의미한  태그 디자인적인 용도로

## 제어할 태그 선택하기

javascript select css selector 
Document.querySelector('css 선택자')

## 프로그램, 프로그래밍, 프로그래머 프로그래밍 언어!

프로그램 , 프로그래밍, 프로그래머 
순차적으로 
반복, 선택, 처리 

## 조건문 예고 

## 비교 연산자와 Boolean Data type

```
'===' 혹은 '!==' : 변수의 타입과 값 모두 비교.
'==' 혹은 '!==' : 변수의 값 비교.

&,| 
<=, >=, <,>

```

## 리팩토링 

여러개를 만들어보고 여러번 사용 다른데서
this-> 
중복을 없애버리기

## 반복문과 배열 

* 배열 

수납상자 , 차곡차곡 
배열은 []

배열.length 
배열.push 
배열 0부터 시작 

i  관습적으로 iterator 

concat, fill , map, filter, reduce,  

* 반복문

for 문 
while문 

* 반복문과배열

Ref [Entity](https://www.w3schools.com/html/html_entities.asp)

* 반복문과배열 활용

Document.querySelectorAll
유사배열 NodeList 

* 함수 

일련의 명령문 모음  -> 반복되는 것 or 같은 논리 재사용성으로 찍어낼 수 있는 것들 :D 
함수로 고우~~ 
엔티티 코드 ~~!!:D 

* 함수의 활용

일련의 명령문 모음  -> 반복되는 것 or 같은 논리 재사용성으로 찍어낼 수 있는 것들 :D 
함수로 고우~~ 
엔티티 코드 ~~!!:D 

* 객체 

어려움 객체지향 프로그래밍,
객체<-> 상태, 행동(함수) n
Property, Method
자바스크립트는 객체다 
나도 객체 우선은 ... 공부 더 해야겠네요 

생활코딩 -> 연관된 함수 및 변수들을 그룹핑해서 정리하기 위해서 객체:D 

배열은 순서대로 저장 
객체 
객체 기본 사용 

```
  <script>
 +      var coworkers = {
 +        "programmer":"egoing",
 +        "designer":"leezche"
 +      };
 +      document.write("programmer : "+coworkers.programmer+"<br>");
 +      document.write("designer : "+coworkers.designer+"<br>");
 +      coworkers.bookkeeper = "duru";
 +      document.write("bookkeeper : "+coworkers.bookkeeper+"<br>");
 +      coworkers["data scientist"] = "taeho";
 +      document.write("data scientist : "+coworkers["data scientist"]+"<br>");
 +    </script>
```

객체 반복 For in (key in your object)

프로퍼티와 메소드 

* 파일쪼개서 정리 정돈 하기 

* JQuery CDN ContentDeliveryNetwork 

* ui and api
user interface
api application programming interface

사용설명서 


[기본개념_공부](https://slides.com/chany/deck-3/live)