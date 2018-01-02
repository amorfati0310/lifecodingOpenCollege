# CSS

> CSS의 등장

CSS의미 Cascading(폭포같은, 연속적인 ) Style Sheet

```

* {
 box-sizing: border-box;
}
a {
    color: inherit;
}
.wrapper: {
    background-color: #eee;
}

이렇게 선택자들을 계속 중첩해서 내려가는 , 마치 폭포수 같은 구조라고 하는데 사용하다 보니 이 의미가 조금 와닿네요

```

기존에 있는 html 을 확장해서 Style을 추가하는 형식이였지만,</br>
스타일의 다양성 및 재사용성을 위해서 CSS의 필요성을 느끼게 됩니다.

> 한계 😖

1. 정보성을 지니지 않음, 디자인적인 요소만 가지는 태그들.
1. 스타일과 html이 섞여있으면 변동이 어려움

*  html에서 주석처리 하는 방법 ```<!--  --> ```
텍스트에디터에서는 각 파일 형식들에 맞춰서 커맨드+/을 누르면 주석 구문이 나옵니다.

> 혁명적 변화 

CSS 사용방법 3가지

1. CSS inline
1. head위에 Style tag안에서
1. 외부 css파일로

우선순위는 밖으로 멀어질수록 멀어진다. inline style 속성으로 넣는 것이 가장 강하고, 다음 style tag안에 다음 외부 css파일로

> 검색 구글링

css text property

> CSS 선택자를 스스로 알아내는 방법 

중요한 개념

1. 효과
1. 선택자
   
선택자는 크게 elmeent, class, id 가 있는데 대체로 모든 style guide들이 class 로 선택하는 것을 권장합니다.
그런데 우선은 여러가지 선택자들을 다 써봅시다.
id는 하나 밖에 없는 특수한 경우 주로 사용합니다.!

> 박스모델
> 그리드
> 반응형 디자인
> CSS 코드의 재사용


참고문헌
[CSS_tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
[CSS_udacity_style_guide](https://udacity.github.io/frontend-nanodegree-styleguide/css.html)