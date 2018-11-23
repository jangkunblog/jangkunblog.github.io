---
layout: post
lang: ko
title: Skip Navigation(건너뛰기 링크, 스킵 네비게이션)은 Quick Link가 아닙니다.
permalink: /wp/skip-navigation-is-not-a-quick-link/
date:   2009-12-03
categories:
  - 웹접근성
tags:
  - skip-navigation
  - 건너뛰기링크
  - 웹 접근성
excerpt: 건너뛰기 링크(Skip Navigation)란? 건너뛰기 링크는 말 그대로 “링크”를 건너뛰기 위해 제공되는 메뉴를 의미합니다. 여기서 “링크”라는 것은 매 페이지마다 반복적으로 제공되는 링크를 말하며, 건너뛰기 링크는 이를 건너뛰어 바로 본문으로 포커스를 이동할 수 있게 해주는 역할을 하게 됩니다. 비장애인의 경우 화면에 출력된 내용을 시각적으로 정확히 인지할 수 있고, 화면에서 원하는 영역으로 바로 시선을 옮길 수 있습니다. 하지만, 장애인의 경우에는 화면에 출력된 내용을 시각적으로 볼 수 없기 때문에 특정 행동, 즉 Tab키나 방향키로 콘텐츠들을 지나가거나 보조 기기의 단축키 등을 이용 [...]
image: skip-navigation-is-not-a-quick-link.png
views:
  - "71519"
---

## 건너뛰기 링크(Skip Navigation)란?

건너뛰기 링크는 말 그대로 '링크'를 건너뛰기 위해 제공되는 메뉴를 의미합니다. 여기서 '링크'라는 것은 매 페이지마다 반복적으로 제공되는 링크를 말하며, 건너뛰기 링크는 이를 건너뛰어 바로 본문으로 포커스를 이동할 수 있게 해주는 역할을 하게 됩니다.

![웹 접근성 연구소에 제공된 건너뛰기 링크 (skip navigation)](/assets/img/2009/skip_navigation_wah1.gif){: .aligncenter}
*[웹 접근성 연구소의 건너뛰기 링크 사례](http://www.wah.or.kr){: target="_blank" }*{: .aligncenter }

**비장애인**의 경우 화면에 출력된 내용을 시각적으로 정확히 인지할 수 있고, 화면에서 원하는 영역으로 바로 시선을 옮길 수 있습니다. 하지만, **장애인**의 경우에는 화면에 출력된 내용을 시각적으로 볼 수 없기 때문에 특정 행동, 즉 Tab키나 방향키로 콘텐츠들을 지나가거나 보조 기기의 단축키 등을 이용해야 합니다.

비장애인은 큰 문제가 없지만, 장애인의 경우에는 해당 페이지의 주요 내용이 위치해있는 본문으로 이동하기 위해서는 대메뉴와 좌측 메뉴 등과 같이 반복적으로 제공되는 링크를 모두 거쳐가야만 합니다. 즉, Tab키/방향키을 반복적으로 눌러야하는 불필요한 행동을 해야하는 것입니다. 이는 웹 접근성(엄밀히 말하면 주 콘텐츠 접근성)을 저해하는 주요인이 됩니다.

그래서 사용자 특히 장애인이 반복적인 링크들로 인해 불편해 하지 않고, 원하는 영역 즉 '본문'으로 바로 이동할 수 있는 건너뛰기 링크를 반드시 제공해야만 합니다.

## 국내외 지침과 가이드라인

건너뛰기 링크는 국내외 다양한 웹 접근성 지침과 가이드라인에 대부분 포함되어 있습니다. 우선 어떤 내용으로 명시되어 있는지 몇가지 지침과 가이드라인을 살펴보도록 하겠습니다.

### WCAG 1.0 (Web Content Accessibility Guidelines 1.0, 1999년 05월 05일)

> **지침 13. 명확한 탐색 구조를 가져야 한다.**  
> :  13.6 관련된 링크들은 한데 묶어 두고, 웹 표시 장치가 그 모둠을 식별할 수 있도록 표시한다. 그리고, 웹 표시 장치가 사용자들에게 그런 기능을 제공하기 전까지는 모둠을 건너 뛸 수 있는 방법도 제시해 주어야 한다. [중요도 3]  
> :  * [http://gregshin.pe.kr/wcag/#gl-facilitate-navigation](http://gregshin.pe.kr/wcag/#gl-facilitate-navigation)

### IWCAG 1.0 (Internet Web Content Accessibility Guidelines 1.0, 2005년 12월 21일)

> **지침8. 웹콘텐츠는 반복적인 네비게이션(repetitive navigation link)를 뛰어넘어 페이지의 핵심부분으로 직접 이동할 수 있게 구성하여야 한다.**  
> :  ① 웹 콘텐츠상에 반복적 네비게이션 링크 객체가 포함되어 있으며 이 링크 객체가 콘텐츠의 핵심부분보다 먼저 읽어주도록 구성된 경우에 이들링크들의 읽기를 생략하고 직접 콘텐츠의 메인 부분으로 직접 이동할 수 있는 링크를 제공하여야 한다.  
> :  * [http://www.wah.or.kr/kwcag/wcag_guide_8.asp](http://www.wah.or.kr/kwcag/wcag_guide_8.asp)

### 웹 접근성 향상을 위한 국가표준 기술 가이드라인 (2009년 03월 17일)

> **9. 반복되는 링크를 건너뛸 수 있도록 건너뛰기 링크(Skip Navigation)를 제공해야 한다.**  
> :  반복적인 네비게이션 링크를 뛰어넘어 페이지의 핵심부분으로 직접 이동할 수 있도록 건너뛰기 링크를 제공해야 한다.   
> :  * [http://www.wah.or.kr/Guide/valuation.asp](http://www.wah.or.kr/Guide/valuation.asp)

### 미 재활법 508조 (Section 508. 1998년 08월 07일)

> **Section 1194.22 Web-based intranet and internet information and applications.**  
> :  (o) A method shall be provided that permits users to skip repetitive navigation links.
> 
> **1194.22조 웹 기반 인트라넷과 인터넷 정보 및 응용 프로그램**  
> :  (o) 반복적인 내비게이션 링크를 사용자가 건너뛸 수 있는 방법을 제공해야한다.  
> :  * [http://www.section508.gov/index.cfm?FuseAction=Content&ID=12#Web](http://www.section508.gov/index.cfm?FuseAction=Content&ID=12#Web)  
> :  * [http://www.access-board.gov/sec508/guide/1194.22.htm#(o)](http://www.access-board.gov/sec508/guide/1194.22.htm#(o))

## 적절한 사용방법

### 제공 위치

건너뛰기 링크는 웹 페이지 상단에서 반복되는 콘텐츠를 건너뛰는 것이므로, **건너뛰기 링크 이전에는 콘텐츠가 없어야 합니다.**  
즉, `<body>`가 시작하고 바로 나오는 것이 가장 적절합니다.

~~~html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="ko" lang="ko">
<head>
----------------------
</head>
<body>
<div class="skip-navigation">
	<p><a href="#content">메뉴 건너뛰기</a></p>
</div>

<div id="wrap">
	<h1><img src="logo.png" alt="OOO구청"></h1>
	<h2>대메뉴</h2>
	<ul>
		<li><a href="intro.html">구청소개</a>
		<li><a href="board.html">참여마당</a>
		----------------------
	</ul>
	----------------------

	<div id="content">
	----------------------

</body>
</html>
~~~

만약 건너뛰기 링크가 로고와 대메뉴 이후에 제공된다면 건너뛰기 링크로서의 역할을 제대로 하지 못하는 것입니다. 단순히 기업 로고 정도만 먼저 나오고 건너뛰기 링크를 제공하는 것이라면 크게 문제가 되지 않겠지만, 대메뉴 등이 건너뛰기 링크 이전에 제공되면 웹 접근성을 보장하는 웹사이트라고 말하기 어렵습니다.

### 제공 방법

건너뛰기 링크의 주 기능은 '반복되는 메뉴를 건너뛰고 본문으로 바로가는 기능'입니다. 즉, **링크는 '메뉴 건너뛰기'만 있으면 됩니다.**

특정 영역으로 바로 가는 링크들의 모음이 아니라, '현재 페이지의 본문으로 이동하는 것이 주 기능'이므로 이를 바로가기 메뉴(Quick Link)처럼 사용해서는 안됩니다. (아래 '잘못된 사례'에서 부연설명)

이때, 추가적으로 '대메뉴 바로가기'나 '퀵 메뉴 바로가기' 등을 제공하는 정도는 일정 부분 허용할 수 있다고 하더라도 아래 사례처럼 많은 링크를 제공하는 것은 피해야합니다.

'메뉴 건너뛰기'라는 명칭은 '콘텐츠 바로가기', '본문 바로가기' 등의 이름으로도 사용될 수 있습니다. 하지만, [링크가 이동되는 위치보다는 링크로 인해 건너뛰는 부분을 알려줄 수 있도록 링크명을 정하는 것이 더 적절하다](http://www.wah.or.kr/Example/wcag_valu.asp?cate=47){: target="_blank" }고 볼 수 있습니다.

## 잘못된 사례

건너뛰기 링크를 사용하는 여러 웹 사이트들을 분석해보면 몇가지 잘못된 사례들을 접하게 됩니다. 여기에서 '잘못된 사례'라는 단어는 웹을 사용하는 장애인 중 다수에게 불편함을 야기시키는 경우를 말합니다. 물론 특정 장애를 가진 분들에게 도움이 될 수 있다고도 볼 수 있지만, 이 포스트에서는 이를 잘못된 사례로 명시하겠습니다.

**[잘못된 사례 샘플 HTML]**{: .aligncenter}

~~~html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="ko" lang="ko">
<head>
----------------------

</head>
<body>

<div id="wrap">

	<div id="header">
		<h1><img src="logo.png" alt="OOO구청"></h1>
		<h2>대메뉴</h2>
		<ul>
			<li><a href="intro.html">구청소개</a>
			<li><a href="board.html">참여마당</a>
			----------------------
		</ul>

		<div class="skip-navigation">
			<ul>
				<li><a href="#gnb">대메뉴 바로가기</a></li>
				<li><a href="#notice">공지사항 바로가기</a></li>
				<li><a href="#news">뉴스 바로가기</a></li>
				<li><a href="#content">본문 바로가기</a></li>
				<li><a href="#briefing">국정브리핑 바로가기</a></li>
				<li><a href="#qna">질문답변 바로가기</a></li>
				<li><a href="#homepage">부서홈페이지 바로가기</a></li>
				<li><a href="#banner">배너모음 바로가기</a></li>
				<li><a href="#copyright">저작권 바로가기</a></li>
			</ul>
		</div>
	</div>

	<div id="content">
		----------------------

		<div class="skip-navigation">
			<ul>
				<li><a href="#gnb">대메뉴 바로가기</a></li>
				<li><a href="#notice">공지사항 바로가기</a></li>
				<li><a href="#news">뉴스 바로가기</a></li>
				<li><a href="#content">본문 바로가기</a></li>
				<li><a href="#briefing">국정브리핑 바로가기</a></li>
				<li><a href="#qna">질문답변 바로가기</a></li>
				<li><a href="#homepage">부서홈페이지 바로가기</a></li>
				<li><a href="#banner">배너모음 바로가기</a></li>
				<li><a href="#copyright">저작권 바로가기</a></li>
			</ul>
		</div>
	</div>

	<div id="footer">
		----------------------
	</div>

	<div class="skip-navigation">
		<ul>
			<li><a href="#gnb">대메뉴 바로가기</a></li>
			<li><a href="#notice">공지사항 바로가기</a></li>
			<li><a href="#news">뉴스 바로가기</a></li>
			<li><a href="#content">본문 바로가기</a></li>
			<li><a href="#briefing">국정브리핑 바로가기</a></li>
			<li><a href="#qna">질문답변 바로가기</a></li>
			<li><a href="#homepage">부서홈페이지 바로가기</a></li>
			<li><a href="#banner">배너모음 바로가기</a></li>
			<li><a href="#copyright">저작권 바로가기</a></li>
		</ul>
	</div>

</div>
</body>
</html>
~~~

### 잘못된 제공 위치

가장 적절한 건너뛰기 링크는 `<body>`가 시작하고 바로 제공하는 것입니다. 건너뛰기 링크는 문서에 접근했을 때 대메뉴나 하위메뉴와 같은 반복되는 링크를 건너뛰고 본문으로 바로 가는 역할을 하는 것입니다. 그렇기 때문에 대메뉴 등의 콘텐츠를 접하기 이전에 제공되어야 합니다.

그런데, 몇몇 웹 접근성 평가 단체에서 건너뛰기 링크의 위치를 위 HTML처럼 [시작지점], [중간지점], [끝지점] 등 여러 위치에 중복 제공하는 것을 권고하고 있습니다. 이런 **건너뛰기 링크의 중복 제공은 적절한 방법이 아닙니다.**

물론 건너뛰기 링크를 여러번 제공하려하는 의도를 이해하지 못하는 것은 아닙니다. 아마도 작업자는 이를 통해 장애인 사용자의 사용성을 높일 수 있다고 판단하고 귀찮고도 귀찮은 이 작업을 했을 것입니다. 아마도... 하지만, 작업자의 의도와는 달리 오히려 이는 사용성/접근성 모두 저해하는 결과를 낳습니다.

다시한번, **건너뛰기 링크는 문서의 처음에 한번만 제공할 것**을 권합니다.

### 잘못된 제공 방법

건너뛰기 링크의 주요 기능은 반복되는 메뉴를 건너뛰고 본문으로 바로가는 기능이라고 했습니다. 그런데, 위의 HTML을 보면 그 핵심을 파악하지 못하고 있다는 것을 알 수 있습니다.

위 사례는 건너뛰기 링크를 '바로가기 메뉴(Quick Link)'로 사용하는 사례로서 불필요한 콘텐츠(여러 개의 바로가기 메뉴들)를 제공하는 잘못된 방식입니다. 바로가기 메뉴는 건너뛰기 링크를 제공하라는 웹 접근성 지침과는 무관한 것으로 건너뛰기 링크라고 볼 수 없습니다. 또한 바로가기 메뉴 자체가 장애인 사용자들에게 키보드 클릭 '수'를 늘리는 원인이 될 수 있고, 이는 대메뉴 반복과 동일한 폐해를 낳게 됩니다.

이는 개발자의 입장에서도 제공된 링크가 이동이 가능한지 모두 테스트를 해야하는 부담을 안게 됩니다. 왜냐하면 이동할 지점이 없이 제공된 경우가 하나라도 있으면 오히려 웹 접근성이 떨어진다고 판단하기 때문입니다.

현재 페이지의 주요 콘텐츠 영역으로 이동하기 위해 이를 사용하는 것이라면, **제목(headings, `<h1>~<h6>`)**을 잘 사용하면 됩니다. 문서의 가장 기본이 되는 '제목(headings)'은 페이지를 구성하는 주요 콘텐츠에 `<h1>~<h6>`를 사용하여 계층구조를 만들게 됩니다.

문서의 구조를 제목(headings)을 통해 제공하게 되면, 보조기기 사용자들은 가장 먼저 제목만을 불러들여 문서의 구조를 파악하게 됩니다. 이후 사용자들은 제목(headings)을 통해 파악된 구조를 바탕으로 콘텐츠 중 원하는 위치의 콘텐츠로 이동하여 내용을 출력시킵니다. 이러한 장애환경을 작업자가 이해한다면 위와 같은 불필요한 제공방법을 선택하지 않을 것입니다.

다시 말씀드리지만, **건너뛰기 링크는 '메뉴 건너뛰기'만 있으면 됩니다.**

## UI

국내 웹 사이트에서 건너뛰기 링크는 통상 화면에서 보이지 않게 처리하는 편입니다.

하지만, 보조 기기를 통해 접근하는 사용자뿐 아니라, 모든 사용자들이 건너뛰기 링크를 이용할 수 있도록 화면상에 건너뛰기 링크를 노출시키는 것이 더 좋다고 개인적으로 생각합니다.

물론 마우스를 사용함에 있어서 큰 불편함이 없는 사용자들에게 해당 링크가 [공해가 될 수 있다는 의견](http://naradesign.net/open_content/lecture/wp/#section33){: target="_blank" }도 있고, 이를 [해결하기 위한 방법](http://naradesign.net/open_content/reference/navigation.html){: target="_blank" }도 제시되었지만, 비장애인이고 마우스 이용이 훨씬 편한 저도 스크롤을 내리는 것보다 건너뛰기 링크를 클릭하여 바로 콘텐츠로 이동하는 방법이 편할때가 있습니다. 이는 개인차가 있을 수 있을 것 같아서 논외로 하겠습니다.(의견은 댓글로 부탁드립니다.)

## 개발시 검수 방법

위에서도 언급했듯 웹 사이트 개발시 건너뛰기 링크는 일반적으로 화면에서 보이지 않게 처리하는 편입니다.

이를 구현하기 위해 사용하는 방법은 CSS를 활용하여 보이지 않게 처리하는 것입니다. 화면에 출력되지 않기 때문에 건너뛰기 링크는 보조기기가 없으면 해당 영역에 접근했는지 명확히 알 수가 없습니다. 사이트 오픈 이전에 이를 테스트하려면 개발방법을 역으로 이용하면 됩니다. 즉, CSS를 제거하면 됩니다.

### 스타일 제거

[Firefox](http://www.mozilla.or.kr){: target="_blank" } 사용자는 Firefox의 보기 메뉴에서 쉽게 CSS 즉, 스타일을 제거할 수 있습니다. 그리고, Internet Explorer 8 사용자는 '보기 > 스타일 > 스타일 없음'을 선택하거나, 개발자 도구(F12)를 클릭하고 '사용 안 함 > CSS'를 선택하면 됩니다.

![Firefox CSS disable](/assets/img/2009/jangkunblog_firefox_css_disable.gif){: .aligncenter}

또한 마크업 개발자라면 아마도 다들 설치했을 Firefox 부가기능인 [Web Developer Tool Bar](http://chrispederick.com/work/web-developer/){: target="_blank" }를 통해서도 쉽게 CSS를 제거할 수 있다. 사실 이것이 마크업 개발자들이 스타일을 제거하는데 가장 많이 사용하는 방법일 것이다. (단축키 : Ctrl + Shift + S)

![Web Developer Toolbar - Firefox CSS disable](/assets/img/2009/firefox_css_disable_wd.gif){: .aligncenter}

### 타겟 확인

스타일을 제거하면 검수자는 시각적으로 화면 상단에 위치한 건너뛰기 링크를 확인할 수 있습니다. 위에서도 언급했듯이 단순히 제공의 차원을 넘어서 사용가능한지 여부를 판단해야 합니다. 이 판단은 해당 링크를 클릭해보면 알 수 있습니다. 만약 클릭을 했는데도 이동하지 않는다면, 이는 제공하지 않는 것과 동일합니다.

반드시 검수자/개발자 등은 웹 사이트 개발시 해당 링크값이 존재하는지를 확인해야합니다.

![Skip Navigation Animation](/assets/img/2009/skip_navigation_animation.gif){: .aligncenter}

## 마무리하며

일반적으로 '스킵 네비게이션'이라고 부르는 건너뛰기 링크는 웹 접근성을 보장하는 웹 사이트를 이루는 중요한 항목입니다. 보다 웹을 쉽고 간편하게 사용할 수 있는 건너뛰기 링크를 작업시 늘 제공해주시길 개발자분들께 부탁드립니다.
  
단지 웹 접근성 평가를 위해 사용할 것이 아니라 이를 통해 혜택받을 수 있는 많은 분들을 위해 사용해야 한다는 점을 잊지 않았으면 좋겠습니다. 지금부터 제작되는 모든 웹 사이트에 건너뛰기 링크를 넣는다면 많은 분들에게 큰 도움이 될 것입니다.
  
내용과 생각이 다르거나 잘못된 부분이 있을 수 있습니다. 댓글로 의견을 남겨주시면 감사하겠습니다.

## 관련 외부 자료 (2010.02.18.추가)

제 글과 더불어 참고할만한 외부 자료 및 블로그 글들을 찾는대로 링크하도록 하겠습니다. 함께 보시면 더 좋을 것 같아서 추가하기로 했습니다. ^^

  * [HHS.gov - Skip Navigation (Accessibility/508)](http://www.hhs.gov/web/policies/skipnavigation.html){: target="_blank" }
  * [WebAIM - 'Skip Navigation' Links](http://www.webaim.org/techniques/skipnav/){: target="_blank" }
  * [JimThatcher.com - Skip Navigation Links](http://jimthatcher.com/skipnav.htm){: target="_blank" }
  * [Dive Into Accessibility - Day 11: Skipping over navigation links](http://diveintoaccessibility.org/day_11_skipping_over_navigation_links.html){: target="_blank" }