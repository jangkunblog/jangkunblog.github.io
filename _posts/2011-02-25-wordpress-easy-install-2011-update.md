---
id: 1039
title: 워드프레스(WordPress) 설치하기 업데이트
date: 2011-02-25T13:28:29+00:00
author: astar2
excerpt: '4년 전에 포스팅한 워드프레스(WordPress) 설치하기라는 글이 있습니다. 크게 신경을 쓰지 않고 있었는데, 얼마전 우연히 트래픽을 좀 보다가 이 포스팅에 의외로 많은 분들이 접근하고 있다는 사실을 알게 되었습니다. 상당히 의외였고, 워낙 옛날 설치 방법이라 그대로 둬서는 안될 것 같아서 최신 버젼의 설치방법을 소개하는 글을 쓰려고 합니다. 순서는 기존 글과 동일하게 가도록 하겠습니다. 그럼 시작해볼까요~ WordPress Download 오랜만에 WordPress 사이트에 가보니 예전에 비해 훨씬 콘텐츠도 정리됐고, 디자인도 깔끔해졌네요. 상단 글로벌 메뉴의 우측 Download 를 클릭해서 들어가면 최신 버젼(2011.02.25. 현재 3.1) [...]'
layout: post
guid: http://www.jangkunblog.com/wp/?p=1039
permalink: /wp/wordpress-easy-install-2011-update/
views:
  - "21746"
dsq_thread_id:
  - "3584961508"
categories:
  - 워드프레스
tags:
  - wordpress
---
4년 전에 포스팅한 [워드프레스(WordPress) 설치하기](http://www.jangkunblog.com/wp/wordpress-easy-install/)라는 글이 있습니다.
  
크게 신경을 쓰지 않고 있었는데, 얼마전 우연히 트래픽을 좀 보다가 이 포스팅에 의외로 많은 분들이 접근하고 있다는 사실을 알게 되었습니다.

상당히 의외였고, 워낙 옛날 설치 방법이라 그대로 둬서는 안될 것 같아서 최신 버젼의 설치방법을 소개하는 글을 쓰려고 합니다. 순서는 기존 글과 동일하게 가도록 하겠습니다.
  
그럼 시작해볼까요~

## WordPress Download

오랜만에 [WordPress 사이트](http://wordpress.org/)에 가보니 예전에 비해 훨씬 콘텐츠도 정리됐고, 디자인도 깔끔해졌네요.

[<img class=" size-large wp-image-1047 aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Home-1024x780.png" alt="WordPress.org Homepage" width="600" />](http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Home.png)

상단 글로벌 메뉴의 우측 [Download](http://wordpress.org/download/) 를 클릭해서 들어가면 최신 버젼(2011.02.25. 현재 3.1)의 WordPress 설치파일을 내려받으실 수 있습니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/Safari.png" alt="WordPress Download" width="237" height="238" />

또는 <http://wordpress.org/latest.zip> 를 클릭하시면 언제나 최신 버젼을 내려받으실 수 있습니다.

## wp-config-sample.php 파일명 변경 및 수정

WordPress 최신 버젼을 내려받고, 로컬에서 압축을 풀어보면, 여러 개의 파일과 폴더가 보입니다.
  
그 중 **wp-config-sample.php** 파일을 찾아서 파일명을 **wp-config.php** 로 변경해야 합니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/wordpress.png" alt="WordPress folder" width="687" height="707" />

이제 파일명을 변경한 wp-config.php 파일을 [EditPlus](http://www.editplus.com/)나 메모장과 같은 에디터에서 열고 몇가지 항목을 수정해야 합니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/wp-config-edit-1.png" alt="wp-config.php 수정 화면-1" width="700" height="686" />

붉은 박스 안에 있는 내용들이 수정이 필요한 부분입니다.
  
해당 내용은 직접 확인하여 수정하시면 됩니다. 대부분 **DB\_NAME, DB\_USER, DB_PASSWORD** 정도를 자신의 정보로 변경합니다.

수정을 다 한 후 저장을 합니다. 이제 웹 서버에 올리고 설치할 일만 남았습니다.

## FTP File Upload

수정이 끝이 났다면, 이제 FTP를 통해 웹 서버로 파일을 업로드해야 합니다.
  
이때 주의해야할 점은 **블로그의 주소를 어떻게 정의할 것인지 먼저 결정**을 해야합니다.

아래에서 두 가지 방법을 설명하도록 하겠습니다.

  * **http://www.jangkunblog.com/**별도로 폴더를 만들지 않고, 웹 서버에 파일들만 선택해서 업로드
  * **http://www.jangkunblog.com/wp/**웹 서버에 wp라는 폴더를 만들고 파일들을 선택해서 업로드.
  
    이 때, 폴더명을 wp가 아닌 wordpress, blog 등으로 바꿔서 업로드해도 됩니다. 대신 주소도 같이 바뀌게 됩니다. (예 : http://www.jangkunblog.com/blog/)

대부분 두번째 방법을 사용해서 블로그를 관리하는 편입니다. 이유는 블로그와 상관없는 파일과 폴더 관리가 편하기 때문입니다. 또한 타 오픈소스(wiki 등)를 설치/관리하는 것 역시 편하기 때문입니다.
  
대신 이렇게 관리를 할 경우, 반드시 [웹 서버에 리다이렉션을 위한 파일을 만들어야만](http://www.jangkunblog.com/wp/wordpress-easy-install/comment-page-1/#comment-17) 블로그로 연결된다는 단점이 있습니다.

만약 WordPress만 사용할 거라면 첫번째 방법도 상관없습니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/html5css3.org_.png" alt="FTP Upload Sample" width="712" height="657" />

이제 웹 서버에 wp라는 폴더를 만들고, 그곳에 파일을 모두 업로드하였습니다.
  
(예제는 현재 제가 보유중인 [www.html5css3.org](http://www.html5css3.org/wp/)을 이용해서 설치해보고 있습니다.)

거의 끝나갑니다. ^^

## WordPress Install

웹 서버에 파일을 모두 올렸으니 이제 설치만 하면 됩니다.
  
설치라고 하니 뭔가 거창한 것 같은데, 한번 어떻게 진행되나 볼까요?

### Step.1

먼저 주소창에 자신의 블로그 주소와 폴더(없으면 생략)를 아래와 같은 양식으로 입력합니다.

> http://홈페이지 주소/wp(업로드한 폴더이름)/wp-admin/install.php

즉, 이렇게 주소창에 쓰시면 됩니다.

<blockquote style="font-weight: bold;">
  <p>
    http://www.html5css3.org/wp/wp-admin/install.php
  </p>
</blockquote>

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Installation.png" alt="WordPress Installation Step 1" width="700" />

이제 브라우저에서 설치화면을 확인할 수 있습니다.
  
입력이 필요한 **Site Title, Username, Password, E-mail**을 입력하고 하단의 &#8220;Install WordPress&#8221; 버튼을 클릭합니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Installation-End.png" alt="WordPress Installation End" width="700" />

놀라셨죠?
  
Step 1 에서 끝이 나버렸습니다. ^^
  
네. WordPress 설치가 끝이 난 것입니다.

설마라고 생각하지 말고, 정말 설치된건지 확인해볼까요?
  
주소창에 <http://www.html5css3.org/wp/> 라고 입력해 보겠습니다.

[<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/HTML5-CSS3-WordPress-site-1024x930.png" alt="HTML5 CSS3 WordPress site" width="700" />](http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/HTML5-CSS3-WordPress-site.png)

WordPress의 기본테마로 구성된 블로그가 만들어진 것을 확인할 수 있습니다.
  
설치가 정상적으로 완료되었습니다.

설치여부를 확인한 후, 이제 Step 1의 설치 성공 화면 하단에 있는 &#8220;Log In&#8221; 버튼을 클릭하고 관리자 화면으로 바로 가보겠습니다.

## WordPress Admin Login

install 시 작성했던 정보를 입력하고 로그인을 해보도록 하겠습니다.

<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Admin-Log-In.png" alt="WordPress Admin Log In" width="700" />

관리자 로그인 정보는 반드시 기억을 하고 있어야 합니다. 글을 쓸때도, 설정을 바꿀때도 로그인을 해야만 하기 때문에 절대 잊어버려서는 안됩니다.

로그인을 하면 관리자 화면을 확인할 수 있습니다.

[<img class=" aligncenter" src="http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Admin-Dashboard.png" alt="WordPress Admin Dashboard" width="700" />](http://www.jangkunblog.com/wp/wp-content/uploads/2011/02/WordPress-Admin-Dashboard.png)

WordPress 관리자 설정에 대한 내용은 다음 포스팅에서 이어서 하도록 하겠습니다.
  
그 전에 관리자 설정들을 하나하나 클릭해보면서 스스로 익혀보시기 바랍니다~

## 마무리하며

WordPress는 정말 강력한 툴입니다.
  
과거의 어떤 툴도 이렇게 간단히 사이트를 구축할 수는 없습니다.
  
또한 플러그인과 테마 커스텀 등과 같이 확장가능성이 무궁무진한 툴이기도 합니다.
  
국내에서는 여전히 큰 사용자 집단을 보유하고 있지는 않지만, 이를 알리는데 조금이나마 노력할까 합니다.

시간나는대로 WordPress 초보자들의 시각에서 WordPress를 뜯어보겠습니다. ^^