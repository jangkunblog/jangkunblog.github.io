---
id: 7
title: 워드프레스(WordPress) 설치하기
date: 2007-05-23T17:50:34+00:00
author: astar2
layout: post
guid: http://www.jangkunblog.com/wp/2007/10/02/7/
permalink: /wp/wordpress-easy-install/
0:
  - wpAjax8d62cb9c691c63dfff2e2d5380a36662dd6c8cb2418c6fbc430641346a705c0c150321f2a858f058c9df8480c5a2e513
1:
  - wpAjaxfc3a94754e7212d5bab7272fce988ee1cd8b49983e48a4e0816bee48dfa39800e31016874977cfc0eef954a09aabdba5
2:
  - wpAjax1c3f6174a4257583a693463369207baa3017f7214129a0f4367ca333c94388e238b13ffe0a422bfbf098763ef7ed25c1
views:
  - "36921"
dsq_thread_id:
  - "3584949436"
categories:
  - 워드프레스
tags:
  - wordpress
  - 설치
---
태터를 깔고 조금 사용해보다가 태터의 한계라고 해야하나 몇가지 불편한 점을 겪고 나서
  
후니님이 계속 강추하던 워드프레스(WordPress)를 설치하기로 결심했다.
  
한글버전이 없는 관계로 처음부터 이거 어렵겠는데 라고 생각을 하고 검색을 시작했다.
  
국내에도 많은 사용자층이 있다고 알고 있었는데, 웹상에서 설치에 대한 얘기가 별로 없었다.
  
태터나 뭐 이런건 설치법이 널려있는데, 이상했다.</span>

그런데!
  
그냥 한번 혼자 해보자고 설치를 시작해보니, 이유를 알아버렸다.
  
이유는&#8230;

**&#8220;너무 쉽다.&#8221;**

ㅋㅋㅋㅋ

그래도 얼마나 쉬운지 알려주기 위해 설치법을 적어볼까 한다.
  
설치법 이후에 플러그인과 테마에 대한 내 경험을 계속 써볼까 한다.
  
즐거운 포스팅이 될 것 같다.

### 1. 워드프레스 2.x 다운받기

<p style="text-align:center;">
  <a title="워드프레스 최신버전 다운로드" href="http://wordpress.org/latest.zip"><img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/01.gif" alt="wp 설치 이미지" /></a>
</p>

### 2. wp-config-sample.php 수정 및 파일명 변경

압축을 풀면 다음과 같은 파일들이 보입니다.

이 중에서 wp-config-sample.php 을 메모장에서 열고 약간의 수정을 해야하는데요.
  
DB\_NAME, DB\_USER, DB_PASSWORD, HOST 등을 개인계정에 맞게 적어주세요.

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/02.gif" alt="wp 설치 이미지" />
</p>

수정한 후에 저장하고 메모장을 닫는다.
  
그리고 wp-config-sample.php의 파일명을 <span style="color: #ff0000;"><strong>wp-config.php</strong></span>로 변경한다.

### 3. ftp로 올리기

이제 내 컴퓨터에서 해야할 일은 끝났구요.
  
현재 사용하고 있는 ftp 프로그램을 이용해서 계정에 올리시면 됩니다.
  
전 개인적으로 wp 라는 폴더를 만들고 그 안에 모든 파일들을 넣었습니다.

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/03.gif" alt="wp 설치 이미지" />
</p>

### 4. install 시작하기

자~ 이제 파일은 다 올렸으니 거의 끝나갑니다.
  
파일을 다 올린 이후 이제 install 을 할건데.
  
주소창에&#8230;

**<span style="color: #ff0000;">http://홈페이지 주소/wp(업로드한 폴더이름)/wp-admin/install.php</span>**

적고 엔터~

그럼 아래와 같은 시작화면이 나오게 됩니다.

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/04.gif" alt="wp 설치 이미지" />
</p>

아래 First Step >> 클릭~

### 5. First Step

Weblog title 과 Your e-mail 을 작성하고 Second Step >> 클릭~

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/05.gif" alt="wp 설치 이미지" />
</p>

### 6. Second Step

예!
  
이제 다 됐습니다. ㅋㅋㅋ
  
엄청 쉽죠?
  
물론 설치 후에 플러그인이나 테마 등에서 여러 난관(언어장벽 등 ㅋㅋ)을 만나게 되겠지만,
  
설치가 다 되니 기분이 엄청 좋더라구요.

이 단계에서 제일 중요한건 임의로 제시되는 비밀번호를 반드시 체크해야한다는 것입니다.
  
복사해놓으면 되겠지라는 안이한 생각은 금물&#8230;
  
저 한번 복사내용 날아가서 암담 ㅡ..ㅡ;
  
귀찮지만, 적거나 메모장에 남겨두면 깔끔합니다.

그런 다음 아래 적여진 **<span style="color: #ff0000;">wp-login.php 를 클릭</span>**해서 로그인 페이지로 가시면 됩니다.

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/06.gif" alt="wp 설치 이미지" />
</p>

### 7. 로그인

왠지 세련된 페이지가 나왔습니다.
  
멋있죠? ㅋㅋ
  
방금전에 적어두셨던 아이디와 비밀번호 기억하시죠?
  
그걸 적고 로그인!

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/07.gif" alt="wp 설치 이미지" />
</p>

### 8. 워드프레스 관리자

로그인을 하니 아래와 같은 관리자가 나왔습니다.
  
영어의 압박이 갈수록 심해집니다. 조심조심. ㅋㅋㅋ

<p style="text-align:center;">
  <img src="http://www.jangkunblog.com/wp/wp-content/uploads/2007/10/08.gif" alt="wp 설치 이미지" />
</p>

### 9. 비밀번호 및 개인정보 변경

아까 적어뒀다가 로그인한 비밀번호를 외운다는건 힘들겠죠.
  
바로 비밀번호를 변경해야합니다. 기억할 수 있는걸로.
  
그리고 그곳에서 여러 정보들도 넣어보세요~

상단 메뉴에서
  
User -> Edit
  
에서 수정하시면 됩니다.

<span style="color: #999999;">이것으로 워드프레스 설치하기 끝!<br /> 진짜 쉽죠?<br /> 겁내하시지 말고 그냥 설치하세요..<br /> 이제 더 어려운 것들 시작입니다.<br /> 저도 잘 모르는 부분이니 열심히 공부해서 또 적을께요~~</span>

<span style="color: #999999;">^^ </span>

## 최근(2011.02.25) 업데이트

워드프레스(WordPress) 설치하기 포스팅이 오래된 버젼이라 최근 버젼을 설치하는 방법을 별도로 포스팅하였습니다. 업데이트된 내용을 보시기 바랍니다. 

[워드프레스(WordPress) 설치하기 업데이트](http://www.jangkunblog.com/wp/wordpress-easy-install-2011-update/)

.