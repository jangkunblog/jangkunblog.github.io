---
layout: post
lang: ko
title: 레이아웃 테이블에 WAI-ARIA presentation role 적용하기
permalink: /wp/using-wai-aria-presentation-role-to-layout-tables/
date:   2015-03-10
categories:
  - 웹접근성
tags:
  - 웹 접근성
  - WAI-ARIA
excerpt: 웹 표준이 국내 소개되면서 지금은 테이블을 활용해서 레이아웃을 만드는 일은 거의 없는 것으로 알고 있습니다. 하지만, 기존에 작업된 페이지의 유지보수나 어쩔 수 없이 레이아웃 테이블을 사용하는 경우가 종종 있는 것이 사실입니다. 이 경우 우리는 많은 죄책감(?)을 느끼게 됩니다. [...]
image:
  src: 'using-wai-aria-presentation-role-to-layout-tables.png'
views:
  - "44444"
---

웹 표준이 국내 소개되면서 지금은 테이블을 활용해서 레이아웃을 만드는 일은 거의 없는 것으로 알고 있습니다.  
하지만, 기존에 작업된 페이지의 유지보수나 어쩔 수 없이 레이아웃 테이블을 사용하는 경우가 종종 있는 것이 사실입니다.  
이 경우 우리는 많은 죄책감(?)을 느끼게 됩니다.

## WAI-ARIA, role="presentation"

웹 접근성을 보장하면서 레이아웃 테이블을 제공하기 위해서는 2가지를 체크하면 됩니다.

  1. 구조를 나타내는 요소(`caption`, `th` 등)나 구조를 나타내는 속성(`summary`, `scope` 등)을 사용하지 않는다.
  2. `table` 요소에 `role="presentation"`을 제공한다.

[WAI-ARIA](http://www.w3.org/TR/wai-aria/){: target="_blank" }의 `role="presentation"`은 해당 테이블의 의미(semantics)를 제거하게 된다.

예를 들어, 아래와 같이 레이아웃 테이블을 마크업한 경우,

~~~html
<table role="presentation">
	<tr>
		<td>나는 레이아웃 테이블이 싫어요.</td>
	<tr>
</table>
~~~

Accessibility tree에서는 아래와 같이 인식된다.

~~~html
<>
	<>
		<>나는 레이아웃 테이블이 싫어요.</>
	</>
</>
~~~

## Example

만만한게 청와대라서 청와대 사례를 보도록 하겠습니다.
  
현재 [청와대 메뉴 중 자문기구 및 소속위원회](http://www1.president.go.kr/cheongwadae/organization/commission.php){: target="_blank" }에는 아래와 같은 표가 제공되고 있습니다.

![청와대 자문기구 및 소속위원회 메뉴의 레이아웃 테이블 사례](/assets/img/2010/wai-aria-presentation-role-1.png){: .aligncenter}
*[청와대 자문기구 및 소속위원회 메뉴의 레이아웃 테이블 사례]*{: .aligncenter }

HTML은 아래와 같습니다.

~~~html
<h4 class="bg_pattern01">헌법상 자문기구</h4>
<table class="datatable" border="1" summary="헌법상 자문기구 표">
	<caption>헌법상 자문기구</caption>
	<colgroup>
		<col width="50%" />
		<col width="50%" />
	</colgroup>
	<tbody>
		<tr>
			<td><a href="http://www.nuac.go.kr/index.jsp" target="_blank" title="새창">민주평화통일자문회의</a></td>
			<td><a href="http://www.neac.go.kr" target="_blank" title="새창">국민경제자문회의</a></td>
		</tr>
		<tr class="crosscoloring">
			<td class="point_black"><a href="http://www.pacst.go.kr" target="_blank" title="새창">국가과학기술자문회의</a></td>
			<td  class="nobg"></td>
		</tr>
	</tbody>
</table>
~~~

사례를 보시면 누가봐도 레이아웃 테이블입니다.  
데이터에 대한 제목이 존재하지 않기 때문에 이를 데이터 테이블이라고 하기에는 무리가 있습니다.

이 경우, `role="presentation"`을 사용할 수 있습니다. 더불어 구조를 나타내는 요소 및 속성을 제거해주어야 합니다.

~~~html
<h4 class="bg_pattern01">헌법상 자문기구</h4>
<table role="presentation">
	<tr>
		<td><a href="http://www.nuac.go.kr/index.jsp" target="_blank" title="새창">민주평화통일자문회의</a></td>
		<td><a href="http://www.neac.go.kr" target="_blank" title="새창">국민경제자문회의</a></td>
	</tr>
	<tr>
		<td><a href="http://www.pacst.go.kr" target="_blank" title="새창">국가과학기술자문회의</a></td>
		<td></td>
	</tr>
</table>
~~~

물론 위 사례에 대한 가장 좋은 방법은 목록(`ul`)을 사용하는 것입니다. ^^

~~~html
<h4 class="bg_pattern01">헌법상 자문기구</h4>
<ul>
	<li><a href="http://www.nuac.go.kr/index.jsp" target="_blank" title="새창">민주평화통일자문회의</a></li>
	<li><a href="http://www.neac.go.kr" target="_blank" title="새창">국민경제자문회의</a></li>
	<li><a href="http://www.pacst.go.kr" target="_blank" title="새창">국가과학기술자문회의</a></li>
</ul>
~~~

## Test

sdfsdf

## 관련 정보