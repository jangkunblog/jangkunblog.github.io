---
layout: post
lang: ko
title: :hover 를 이용한 Rollover Menu 만들기
permalink: /wp/hover-rollover-menu/
date:   2007-10-18
categories:
  - CSS Tip
tags:
  - CSS
  - hover
  - rollover
excerpt: 얼마전에 윤석찬님이 번역해주신 ‘HTML 4와 HTML 5의 차이점‘ 이라는 글을 보고 HTML 5 가 상당히 재미있어질 것 같다는 생각을 했었다. 오늘 네이버 하코사 카페에 오랜만에 갔는데 HTML 5 에 관한 소식이 있어서 한번 가봤더니 ‘W3C Editor’s Draft‘ 라고 나와있었다. 오호라~ 솔직히 ‘Working Draft’와 ‘W3C Editor’s Draft’ 의 차이는 모르겠다. 어쨌든 확실한건 HTML 5에 대한 준비와 공부를 해야한다는 사실뿐이다. 당장은 아니지만, 이 짓을 업으로 살꺼라면 미리미리 준비해두는게 좋을듯하다.. ㅋㅋㅋ CSS3도 그렇고, 번역된 것이 없다보니 한계에 부딪히는 하루하루다. [...]
image: hover-rollover-menu.png
views:
  - "20402"
dsq_thread_id:
  - "3584961027"
---

괜찮았던 결과물들을 정리해보는 방향으로 설정했다.

Rollover(롤오버)메뉴를 만들때 기존에는 javascript의 도움을 받아왔다.  
난 개발자가 아니기 때문에 기존에 사용하는 사이트에서 긁어오거나 에디터에서 자동으로 생성되는 소스를 그대로 사용했던 기억이 있다.

[:hover를 이용한 Rollover Menu 예제](/study/css/ex/rollover/rollover.html){: target="_blank" }

그런데, CSS로 Rollover메뉴를 쉽게 만들 수 있는 방법을 아는 순간 경악했다.  
이런 간단한 방법이 있단 말인가! 왜 몰랐지.  
역시 공부를 해야해... 라며 자책했다.
  
소스? 어마어마하게 줄어든다. 게다가 전혀 모르는 소스가 아닌 아는 소스라는 사실!

#### Html

~~~html
<ul id="tab">  
    <li id="gi"><a href="#">채용정보</a></li>
    <li id="ht"><a href="#">헤드헌팅</a></li>
</ul>
~~~

#### CSS

~~~css
#tab {
	list-style:none;
}
#tab li {
	float:left;
}
#gi a {
	display:block;
	width:60px;
	height:25px;
	text-indent:-5000px;
	background:url(/css/ex/rollover/01.gif) no-repeat left top;
}
#ht a {
	display:block;
	width:60px;
	height:25px;
	text-indent:-5000px;
	background:url(/css/ex/rollover/02.gif) no-repeat left top;
}
#gi a:hover {
	background-position:0 -25px;
}
#ht a:hover {
	background-position:0 -25px;
}
~~~

위 방법은 html에서 메뉴를 이미지가 아닌 텍스트로 구성하고, 이미지 대체 기법으로 작업한 것이다.  
그냥 바로 메뉴 이미지를 넣고 해도 무방하다. (text-indent 삭제)

원리는 CSS의 :hover가상클래스를 이용한 방식이다.  
마우스 on상태와 over상태의 두 상황이미지를 하나로 만들고, 마우스 on시에 :hover가상클래스를 이용해 위치값을 변경해서 이미지가 바뀌게 하는 것이다.

![예제 1](/assets/img/2007/011.gif)

이 방식말고도 여러 방식들이 가능하고, IE에서는 버그(?)도 있다.
  
어쨌든 디자이너들은 이 방식으로 개발자한테 당당해지자!!!  
별것도 아닌걸 가지고 콧대세우는 개발자말이다...