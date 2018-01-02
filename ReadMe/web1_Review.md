## Web1_HTML_Review
---

* 강의 Overview
> 프로젝트 동기

사람들과 공유하다보니,
 Web상 + HD화질 영상 컨텐츠를 만들기 원할한 시대의 발전

> 기획

기획자가 되볼까요?
Web (HTML, CSS, JS )
참고로</br>
Web을 구성하는 3가지 언어

 1. HTML
 1. CSS
 1. JavaScript

HTML은 컨텐츠
CSS는 스타일 및 레이아웃 및 애니메이션
JS는 사용자 interaction에 따른 변화 / 애니메이션/ 동적 처리
애니매이션은 css로 처리하는 것이 더 빠릅니다 ~:D
GPU가 연산 처리가 훨씬 빠른것 처럼 스타일 관장하는 CSS에서 처리 하는 것이 더 좋다 정도로 알아두시고 자세한 사항은
[요기](https://www.html5rocks.com/ko/tutorials/speed/high-performance-animations/)
살펴보시면 좋을 것 같습니다

> 코딩과 HTML

코드 , 소스 언어 -> 어플리케이션 ,앱, 프로그램, 웹페이지 웹사이트
웹은 퍼블릭 도메인 !
누구나 접근 가능 , 그래서 지금 처럼 가치 있지 않나

> HTML 코딩 실습 환경 준비~

브라우저 -> 크롬, ... 크롬을 사용합시다!
텍스트 에디터 -> 소스 코드 작성
(아톰, Vscode, Webstorm, Braket, SublimeText ...)
이고잉님 수업에서는 아톰을 쓰지만 , 다양한 툴을 한 번 접해보기 위해서
오프라인 수업에서는 요.대.세인 에디터 VsCode를 다뤄봅시다 

[VSCode](https://code.visualstudio.com/)
[VSCode_Setting](VSCodeSetting.md)

.html 확장자 -> 브라우저가 html문서를 해석할 수 있는 포맷!

텍스트 에디터에 아무텍스트나 입력해보고 저장하고 브라우저로 열어봅시다 예시```
hi there!```

> 기본문법 태그

수업 말고 내가 좋아하는 걸로 한 번 따라가봅시다</br>
example)2018년 목표</br>
** bold **</br>
첫번째 태그 strong html문법은 열고 닫고 <></></br>```
<strong> 2018 이번엔 성공한다!</strong>```

> 혁명적인 변화

쉬운것이 가장 중요하다. </br>
개발자도구, 소스보기 [W3C_(월드와이드웹_컨소시옴_페이지](https://www.w3.org/)</br>
구조파악 or
가져와서 뭔지 텍스트에디터에다가 붙여놓고 열어보기:D
그리고 모르는 태그 검색해서 사용법을 알아봅시다</br>
수업에서는 heading

> 통계로 기반한 학습

![중요태그](https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7624.png)
영단어 1000개만 알아도 90%대화가능?
숫자기호나 +,-를 아는 것 처럼 이런것들!!!
```
html,head,body,meta,title 등은 늘 쓰이는 부분이니까
a,div,link,script,img,p,span,ul,li,form,input,style 
그리고 html5에서 semantic tag
<header>, <footer>, <article>, <section>, <nav>, <main>, <aside>
등을 먼저 알아봅시다.

```

> 줄바꿈 & html이 중요한 이유

줄바꿈은 필요할때만, 각각 의미에 맞는 블락 엘리먼트들을 사용하여 단락 구분을 하고, 단순히 단락안에서 줄을 바꿀 필요가 있을 때 사용하는 것이 제대로 된 사용
```
<h3></h3>
<strong><span style="font-size:22px;">coding</span></strong>
```
접근성, SEO관점으로 모두 의미에 맞는 태그 사용하는 것이 중요!
물론 자기 만족을 위해서도지만, 남들에게 보여주기 위해 작성하는데 시멘틱한 태그를 안 지켜서, 100Page뒤에 있다고 생각해보자... 절대 노출될 수 없을 것이다

> 최후의 문법과 속성

```
<a href="" >
<img src="" alt="" />
<input type="password" />
```
태그들은 각각 사용에 따라 특수한 attr을 가지고 있다

> 부모 자식 태그

html태그는 트리구조 부모안에 자식있고 그 안에 또 자식 있고 이런 구조로 이루어져 있습니다.
```
크게 이렇게 이루어져 있습니다.
<html>
    <head></head>
    <body></body>
</html>
```
head는 문서 정보 body는 실제 보이는 컨텐츠 영역
List를 나타내는 ul,ol태그는 자식을 li로만 가집니다.
리스트 그리고 리스트아이템
ul(unordered list),ol (ordered list)은 순서가 있는 없는으로 나눠집니다.

> 문서구조와 슈퍼스타들

VSCode에서 !+ tab해서 나오는 html 기본 boilerplate를 살펴봅시다.
```
<!DOCTYPE html>
html5을 명시적으로 선언하겠습니다.
<html lang="en">
html tag시작 주 언어는 영어로 쓸께요
head 문서의 정보를 담고 있습니다.
문서의 이름,성격 같은 거라고 생각하면 이해하기 편하실거에요
눈에 실질적으로 보이지는 않는데!

head안에 meta tag속성 charset utf-8은 unicode 모든 문자를 지원하는 포맷으로 작성하겠다.

meta name="viewport" 이 구문은 viewport width는 디바이스 width, 처음 비율은 1.0으로 가져가겠다.

meta http-equiv="X-UA-Compatible"
IE=edge 사용자가 사용하고 있는 가장 최신 버전 기준으로 렌더링 하겠다는 의미입니다.
IE=7; IE=8; IE=9; IE=10; IE=edge
유독 ie만 버전별로 이렇게 있는 이유는 그 만큼 버전별로 호환되는 부분이 달라서 인 것 같은데 자세한 사항은 좀 더 알아봐야겠습니다.
http-equiv
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
</body>
</html>

```
> html Tag 의 제왕

두둥```<a></a>```태그입니다.
HyperText를 의미하는 a태그, 문서 문서 연결고리 역할
```
<a href="https://www.w3.org/TR/html5/" target="_blank" title="html5 specification">Hypertext Markup Language (HTML)</a>
a tag의 대표 attr은 href,target,title
_blank는 새창에서 열기,
title은 툴팁으로 나타내는 text를 의미합니다.
``` 

> 웹사이트의 완성

방금 배운 a tag를 이용해서 웹 문서들을 연결해봅시다!

> 웹 접근성
누구나 쉽게 정보를 공유할 수 있도록 Universal Design

> 수업 때 해본것을 이용해서 웹 문서를 만들어봅시다.
자기소개서, 2018년 계획,...등등

> 크롬 개발자 도구 

> Ref
코드카데미 
생활코딩 
Udacity 
인프런 

> 웹의 역사 
인터넷과 웹은 다른 개념 
인터넷은 전체를 연결하는 연결망 
웹은 앱서비스나 다른 통신망이 들어가는 모든 서비스들을 인터넷이라고 볼 수 있습니다.
웹의 메소포타미아 
http://info.cern.ch/
웹 호스팅
웹 서버

>  웹서버 운영하기
아파치, Nginx
how to install apache http server os