---
id: 56
title: :hover 를 이용한 Rollover Menu 만들기
date: 2007-10-18T15:46:42+00:00
author: astar2
layout: post
guid: http://www.jangkunblog.com/wp/2007/10/18/56/
permalink: /wp/hover-rollover-menu/
0:
  - wpAjax4d4ef584cc002b85d20d5d362bdc26910169ce3258ae54365878d5cb08c5ac04cbe8abc5752d767001922ce5b7abaf82
views:
  - "20402"
dsq_thread_id:
  - "3584961027"
categories:
  - CSS Tip
tags:
  - CSS
  - hover
  - rollover
---
처음 블로그를 만들고 멋진 글을 남겨야한다는 압박에 보다시피 글을 쓰는 횟수가 저조하다.
  
점점 스스로 좁아지고 블로그가 의미가 없어진다는 느낌을 받는 순간.
  
보여주기 위한 블로그가 아닌 스스로 공부할 수 있는 블로그를 만들어보자는 생각을 했다.
  
그래서 쉽지만, 괜찮았던 결과물들을 정리해보는 방향으로 설정했다.
  
혹시 유치한 예제들을 만나면 그냥 읽지 않아도 된다. ㅋㅋ



Rollover(롤오버)메뉴를 만들때 기존에는 javascript의 도움을 받아왔다.
  
난 개발자가 아니기 때문에 기존에 사용하는 사이트에서 긁어오거나 에디터에서 자동으로 생성되는 소스를 그대로 사용했던 기억이 있다.
  
그런데, CSS로 Rollover메뉴를 쉽게 만들 수 있는 방법을 아는 순간 경악했다.
  
이런 간단한 방법이 있단 말인가! 왜 몰랐지.
  
역시 공부를 해야해&#8230;. 라며 자책했다.
  
소스? 어마어마하게 줄어든다. 게다가 전혀 모르는 소스가 아닌 아는 소스라는 사실!

#### Html

<pre name="code" class="html">&lt;ul id="tab"&gt;
	&lt;li id="gi"&gt;&lt;a href="#"&gt;채용정보&lt;/a&gt;&lt;/li&gt;
	&lt;li id="ht"&gt;&lt;a href="#"&gt;헤드헌팅&lt;/a&gt;&lt;/li&gt;
&lt;/ul&gt;</pre>

#### CSS

<pre name="code" class="css">#tab {
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
	background:url(/cssdic/ex/rollover/01.gif) no-repeat left top;
}
#ht a {
	display:block;
	width:60px;
	height:25px;
	text-indent:-5000px;
	background:url(/cssdic/ex/rollover/02.gif) no-repeat left top;
}
#gi a:hover {
	background-position:0 -25px;
}
#ht a:hover {
	background-position:0 -25px;
}</pre>

위 방법은 html에서 메뉴를 이미지가 아닌 텍스트로 구성하고, 이미지 대체 기법으로 작업한 것이다.
  
그냥 바로 메뉴 이미지를 넣고 해도 무방하다. (text-indent 삭제)

원리는 CSS의 :hover가상클래스를 이용한 방식이다.
  
마우스 on상태와 over상태의 두 상황이미지를 하나로 만들고,
  
마우스 on시에 :hover가상클래스를 이용해 위치값을 변경해서 이미지가 바뀌게 하는 것이다.

![예제 1](http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/011.gif)

이 방식말고도 여러 방식들이 가능하고, IE에서는 버그(?)도 있다.
  
버그 관련해서는 따로 포스팅 할 기회가 있을 것 같다.

어쨌든 디자이너들은 이 방식으로 개발자한테 당당해지자!!!
  
별것도 아닌걸 가지고 콧대세우는 개발자말이다&#8230;&#8230;..