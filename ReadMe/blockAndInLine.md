# Block Element & InLine Element

기본적으로 html은 태그 속성에 따라서 블락요소, 인라인요소 ,인라인블락요소로 나뉘어져 있습니다.

> 블락

![](https://blogfiles.pstatic.net/MjAxNzAxMzFfMTEw/MDAxNDg1Nzg4OTMyNjE4.PkD8jxV-EKFxFT5y0U0TZspSsKzX-CtFB0htUwGWUMgg.cfhf16MaXTUjJzncZfBeZUq4FDz0sbl0Waj5pcrUDH8g.PNG.lyhy0310/%EA%B7%B8%EB%A6%BC4.png)

면 같은 느낌 </br>
블락요소는 말 그대로 블라킹, 막는 역할을 해요. 난공블락?
한줄을 다 차지해요 욕심쟁이 컨텐츠 크기나 width가 라인을 다 차지 하지 않더라도 margin이 자동으로 채워져서 다른 요소들이 자신의 블락에 들어오지 못하게 막습니다 :D

블락요소들의 특징

1. width값이 정해지지 않았을 때는  부모의 컨텐츠 크기만큼 가진다.

1. height값이 주어지지 않았을 때는 자식의 height값을 따른다.
1. 노말 플로우상에서는한 줄을 다 차지(margin으로)
    (float나 absolute시킨 블락요소들은 또 컨텐츠 크기만큼만 차지하고 막는 성질이 없어진다.
      레이어 개념으로 떠 있으니까 막아야 될 필요성이 없어지나봐요 )
1. width,height값을 줄 수 있다

```
a{
background:red;

}
```

태그들의 기본성질이 어떤지 알아보려면 css에 배경색을 칠해보면 쉽게 알 수 있어요 </br>
한 줄 다 칠해지면 블락 , 컨텐츠 크기만큼만 칠해지면 inline요소겠지요:D

그리고 큰 단위들 레이아웃들을 결정짓는 </br>
div,heading,p,ul 등등  박스성질로 큼직하게 한 줄 차지할 녀석들은 어지간하면 블락요소 성질을 가지고 있어요 </br>
block성질을 가지고 있는 tag들 div, h1, p, ul, li 등</br>
inline성질을가지고 있는 태그들 a, span, img등등 </br>
[block_inline_element](http://www.w3schools.com/html/html_blocks.asp)

> 2.inline 요소 Text 성질

선 같은 느낌-----------------------------------------------------------------------------
말 그대로 라인 안에서 행동한다 글자요소 라고 생각하시면 될 것 같아요 width나 height 넓이를 가질 수 없습니다.
(line-height는 가지지만)

> 3.Inline block - SuperStar

1+1=3?

1,2번의 성질을 모두 쓸 수 있게 하기 위해서 탄생한 친구 inline block </br>
특히 텍스트 속성인 인라인 요소에  블락요소(width-height)등을 주고 싶을 때
많이 쓰입니다. inline요소를 </br>
블락요소로 바꾸면 한줄을 다 차지하려는 성질 때문에 레이아웃이 깨지는 상태가 발생하겠죠

반대의 경우에도 마찬가지이고요 , 기본 블락의 막는 성질을 없애고 정렬하고 싶을 때 등등 쓰임이 많은 유용한 요소입니다.