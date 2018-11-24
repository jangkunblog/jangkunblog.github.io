---
layout: post
lang: ko
title: CSS Hover 를 이용한 깔끔한 페이징
permalink: /wp/css-hover-pagination/
date:   2008-02-15
categories:
  - CSS Tip
tags:
  - CSS
  - hover
  - pagination
excerpt: 웹디자이너로서 웹사이트 제작을 하다보면, 여러가지로 신경쓰이는 부분이 많습니다. 컬러, 폰트, UI, 가독성 등등. 대부분 눈에 많이 띄는 부분 위주로 디자인의 초점이 맞춰지고, 이것만 잘돼도 문제없이 디자인을 완료할 수 있습니다. 그러다보니 눈에 잘 띄지 않거나 큰 비중이 없는 부분은 대충 디자인을 잡게 되는 경우가 종종 있습니다. 그 부분때문에 특별히 큰 문제가 생기지 않기때문에 더욱 그랬던 것 [...]
image:
  src: 'css-hover-pagination.png'
views:
  - "60222"
dsq_thread_id:
  - "3584946118"
---

웹디자이너로서 웹사이트 제작을 하다보면, 여러가지로 신경쓰이는 부분이 많습니다.
  
컬러, 폰트, UI, 가독성 등등.
  
대부분 눈에 많이 띄는 부분 위주로 디자인의 초점이 맞춰지고, 이것만 잘돼도 문제없이 디자인을 완료할 수 있습니다.  
그러다보니 눈에 잘 띄지 않거나 큰 비중이 없는 부분은 대충 디자인을 잡게 되는 경우가 종종 있습니다.  
그 부분때문에 특별히 큰 문제가 생기지 않기때문에 더욱 그랬던 것 같습니다.

저에게 있어 기존에 크게 신경쓰지 않았던 곳 중에 하나가 바로 <del>'페이징'</del><ins>'pagination'</ins>입니다.  
(물론 저의 경우입니다. 대부분의 디자이너분들은 아닐거라 생각합니다. ^^)

![pagination 샘플](/assets/img/2008/csshover-1.png){: .aligncenter}
*[미리보기](/assets/sample/css-hover-pagination.html){: target="_blank" }*{: .aligncenter }

위와 같은 pagination 어떠세요?
  
[네이버](//cafeblog.search.naver.com/search.naver?where=post&sm=tab_nmr&query=hover){: target="_blank" }에서 쓰고 있는거랑 비슷하죠? [플리커](//www.flickr.com/photos/jangkunblog/){: target="_blank" }도 이런 스타일을 쓰고 있죠..
  
크게 디자인 요소를 넣지 않았지만, 깔끔하고, 발랄한 느낌을 가진 pagination이라는 느낌이 듭니다.

그럼 한번 이 pagination을 만들어볼까요?  
pagination작업시 HTML은 아래와 같이 간단합니다.

## HTML

~~~html
<ul>  
    <li><a href="#">1</a></li>  
    <li><a href="#">2</a></li>  
    <li><a href="#">3</a></li>  
    <li><a href="#">4</a></li>  
    <li><a href="#">5</a></li>  
    <li><a href="#">6</a></li>  
    <li><a href="#">7</a></li>  
    <li><a href="#">8</a></li>  
    <li><a href="#">9</a></li>  
    <li><a href="#">10</a></li>  
</ul>
~~~

이제 HTML은 손을 댈 곳이 없고, CSS로 평범한 숫자들의 목록을 이쁘게 만들어 볼까요?
  
CSS는 아래와 같습니다.

## CSS

~~~css
ul {
	list-style:none;
	float:left;
	display:inline;
}
ul li {
	float:left;
}
ul li a {
	float:left;
	padding:4px;
	margin-right:3px;
	width:15px;
	color:#000;
	font:bold 12px tahoma;
	border:1px solid #eee;
	text-align:center;
	text-decoration:none;
}
ul li a:hover, ul li a:focus {
	color:#fff;
	border:1px solid #f40;
	background-color:#f40;
}
~~~

간단하죠.  
물론 더 간단하게 예쁘게 만드실 수 있는 분들이 많을거에요. ^^

어쨌든 위내용을 정리해보면,

  1. 목록을 우선 `float` 시켜서 가로로 배열하고,
  2. 각 `li` 들의 `a` 값을 이용해서 width 값을 고정시키고,
  3. `a` 에 비활성화 상태의 스타일을 정의하고,
  4. `a`의 `hover` 선택자에서 활성화 상태의 스타일을 정의하면 끝!

이런 간단한 과정으로 밋밋한 pagination을 깔끔한 pagination으로 만드실 수 있습니다.

실제 웹사이트에서 사용할때는 '이전', '다음', '현재페이지' 등도 표현해야하는데, 이번 예제를 이해하시면 금방 적용하실 수 있어서 그 부분은 빼도록 하겠습니다.  
그리고, IE 5.5 에서도 동일하게 보이게 하기 위해 들어가는 CSS도 빼도록 하겠습니다.
  
그 부분은 [미리보기](/assets/sample/css-hover-pagination.html){: target="_blank" }에 담겨있습니다.  
(Mac 등에서는 확인을 못했습니다. T.T)

더 좋은 방법이나 문제점이 있으면, 답글 부탁드립니다~

## `display:inline-block`을 이용한 pagination 방법 <ins>(2009-07-09)</ins>

`float`을 사용했을 경우 page 수에 따라 가운데 정렬하는 부분에 어려움이 생깁니다.
  
항상 10개가 기본으로 나온다는 보장이 없기때문에 가운데 정렬을 기본으로 해야하는데, 이를 위해서 `display`속성의 값들 중에서 `inline-block`값을 사용해서 만들어보도록 하겠습니다.

> **inline-block :**  
> :  This value causes an element to generate a block box, which itself is flowed as a single inline box, similar to a replaced element. The inside of an inline-block is formatted as a block box, and the element itself is formatted as an inline replaced element.
> :  <W3C CSS 2.1 Specification (<//www.w3.org/TR/CSS21/visuren.html#propdef-display>)>

`display:inline-block`은 W3C의 CSS 2 명세에서는 없었고, [CSS 2.1 권고후보에서 추가된 값](//www.w3.org/TR/CSS21/visuren.html#propdef-display){: target="_blank" }으로 해당 요소를 block 박스로 만들지만, inline 요소와 같은 흐름을 가지게 하는 값입니다. 즉, inline 요소가 가질 수 없는 top(bottom) margin 과 top(bottom) padding, width를 가질 수 있게 됩니다.

HTML은 동일하고 CSS만 추가해보겠습니다.

~~~css
ul {
	text-align:center;
}
ul li {
	display:inline;
	vertical-align:middle;
}
ul li a {
	display:-moz-inline-stack;	/*FF2*/
	display:inline-block;
	vertical-align:top;
	padding:4px;
	margin-right:3px;
	width:15px !important;
	color:#000;
	font:bold 12px tahoma;
	border:1px solid #eee;
	text-align:center;
	text-decoration:none;
	width /**/:26px;	/*IE 5.5*/

}
ul li a.now {
	color:#fff;
	background-color:#f40;
	border:1px solid #f40;
}
ul li a:hover, ul li a:focus {
	color:#fff;
	border:1px solid #f40;
	background-color:#f40;
}
~~~

`display:inline-block`의 경우 Firefox 2에서 적용이 안되는 문제가 있어 `display:-moz-inline-stack;`를 별도로 제공해야합니다. 하지만, 회사마다 지원 브라우저의 범위가 있으므로, 저희처럼 Firefox 2에 대한 지원은 하지 않기로 한 곳은 없어도 무방합니다.
  
작업내용은 [미리보기](/assets/sample/css-hover-pagination.html){: target="_blank" }에서 확인하실 수 있습니다.  