---
layout: post
lang: ko
title:  Sublime Text에서 CSS 작업시 콜론 뒤에 자동으로 생기는 공간 없애기
permalink: /wp/how-to-remove-space-after-a-colon-in-css-with-sublime-text/
date:  2015-04-29
categories:
  - Sublime Text
tags:
  - CSS
  - Sublime Text
excerpt: Sublime Text의 CSS 속성 뒤의 공간에 대한 Sublime Text의 기본적인 처리방법은 아래와 같이 속성(property)을 자동완성에서 선택하면 콜론(:)뒤에 한 칸 여백이 생깁니다. 저희 회사는 이 여백을 사용하지 않고 있습니다. 어떤 분은 실서버에 반영할 때 자동으로 날리면 된다고 하시는 분들도 있지만, 저희는 아직 그런거 안합니다. 어쨌든 계속 신경쓰여서 혹시나 하고 검색해봤더니 여러 방법들이 있었습니다. PackageResourceViewer라는 플러그인을 설치하고 수정하는 방법도 있지만, 윈도우즈 탐색기를 통해서 접근하는게 더 쉽습니다. 단, 기본적으로 ‘폴더 옵션’에서 ‘숨김 파일, 폴더 및 드라이브 표시’가 설정되어 있어야 합니다. 위 경로대로 가면 css_completions.py라는 파일이 있고, 이를 에디터에서 열면 190번째
image:
  src: 'how-to-remove-space-after-a-colon-in-css-with-sublime-text.png'
views:
  - "12791"
dsq_thread_id:
  - "3722192709"
---

저는 컴퓨터 포맷 전에 프로그램 세팅을 백업하는 것을 자주 까먹는 편입니다.  
그러다보니 매번 포맷 후 각종 설정을 다시 하는 것도 일인 것 같습니다.  
특히 Sublime Text 세팅은 여간 귀찮은게 아닙니다. ㅜㅜ

대부분 잘 알고 있는 팁이겠지만, 기억저장할겸 간혹 포스팅 할 예정입니다.

[주의] 아래 내용은 회사마다 코딩 컨벤션이 다르기 때문에 저희 회사랑 룰이 같을 경우에만 해당되는 내용입니다.

## Sublime Text의 CSS 속성 뒤의 공간

Sublime Text의 기본적인 처리방법은 아래와 같이 속성(property)을 자동완성에서 선택하면 콜론(:)뒤에 한 칸 여백이 생깁니다.

``` css
.class {
	float: left;
}
```

저희 회사는 이 여백을 사용하지 않고 있습니다.  
어떤 분은 실서버에 반영할 때 자동으로 날리면 된다고 하시는 분들도 있지만, 저희는 아직 그런거 안합니다. ㅜㅜ

어쨌든 계속 신경쓰여서 혹시나 하고 검색해봤더니 여러 방법들이 있었습니다.

## [Windows 7] Sublime Text의 css_completions.py 수정하기

PackageResourceViewer라는 플러그인을 설치하고 수정하는 방법도 있지만, 윈도우즈 탐색기를 통해서 접근하는게 더 쉽습니다.  
단, 기본적으로 '폴더 옵션'에서 '숨김 파일, 폴더 및 드라이브 표시'가 설정되어 있어야 합니다.

![sublime-text-css-completions-py](/assets/img/2015/sublime-text-css-completions-py.png){: .aligncenter}

윈도우즈 탐색기에서 아래와 같은 순서로 탐색을 해야 합니다.

  1. 로컬 디스크(C드라이브)
  2. 사용자
  3. 사용자 계정 ID (난 jangkunblog임)
  4. AppData
  5. Roaming
  6. Sublime Text 3
  7. Packages
  8. CSS

CSS 폴더에 css_completions.py라는 파일이 있고, 이를 에디터에서 열면 190번째 줄에 아래와 같이 작성되어 있습니다.

``` html
.append((p, p + ": "))
```

여기에서 콜론 뒤의 공간을 삭제합니다.

``` html
l.append((p, p + ":"))
```

파일을 저장하고, Sublime Text를 재실행하면 이제 끝!

``` css
.class {
	float:left;
}
```

이제 잘 되네요~

즐 코딩~