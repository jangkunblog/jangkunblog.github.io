---
layout: post
lang: ko
title: 워드프레스로 웹 접근성 칭찬받기
permalink: /wp/how-to-improve-wordpress-s-web-accessibility/
date:   2015-03-10
categories:
  - 워드프레스
  - 웹접근성
tags:
  - wordpress
  - 웹 접근성
excerpt: 얼마전 한국 워드프레스 사용자 모임에서 진행하는 ‘워드프레스 미트업 서울 2015‘에 참가하였습니다. 나름 오랫동안 워드프레스를 사용해오고 있지만, 막연하게 워드프레스가 웹 접근성을 상당히 고려하고 있다고만 알고 있었습니다. 하지만, 상당한 공헌자들의 노력들이 있었기에 가능한 일이었습니다. 노력의 질과 양을 보면서 많은걸 깨닫게 되는 계기가 되었습니다. 우선 워드프레스는 코어 뿐만 아니라 테마, 플러그인 등 전반적으로 웹 접근성을 높히기 위한 노력을 하고 있었습니다. 워드프레스 자체적으로 다양한 분야에 공헌할 수 있는 기회가 주어지는데, 접근성 또한 포함되어 있습니다.  특히, Accessibility Testing의 경우 배울 점들이 많았습니다. 체크리스트를 기반으로 각종 코어, 테마, 플러그인 등을 테스트하고 [...]
image: how-to-improve-wordpress-s-web-accessibility.png
views:
  - "12076"
youtubeId: lvb8SANYsUs
---

얼마전 한국 워드프레스 사용자 모임에서 진행하는 '[워드프레스 미트업 서울 2015](http://kopress.kr/wordcamp/camp/meetup-seoul-2015/)'에 참가하였습니다.

![워드프레스 뺏지](/assets/img/2015/wordpress_meetup_4.jpg){: .aligncenter}

예전부터 암암리에(?) 워드프레스 모임과 관계를 유지하던 차에 운영자이신 [천영민](http://082net.com/)님의 연락을 받고 바로 발표를 수락하였지만, 회사 서비스 런칭 때문에 바빠서 결국 발표자료는 당일날에야 완성이 되었습니다.  
게다가 감기가 심해져서 '타미플루'를 처방받기까지 하여 육체적으로나 정신적으로나 여간 부담이 되는 행사가 아닐 수 없었습니다.

(여담 : 082net의 천영민님은 제가 워드프레스로 블로그를 처음 만들 때 댓글로 계속 질문하면서 도움을 받았던 분입니다. 국내에서 워드프레스를 시작하게 되면 한번쯤은 천영민님의 블로그를 가게 되죠~ ^^)

## 워드프레스 미트업 서울 2015

행사는 금천구 현대아울렛 6층에 있는 G밸리 시민청이라는 곳에서 진행되었습니다.  
200명의 신청자가 모두 온건지 행사장이 발디딜 틈없이 꽉 차 있었습니다.

![워드프레스 미트업 서울 2015 프로그램](/assets/img/2015/wordpress_meetup_1.png){: .aligncenter}

솔직히 감기로 인해 정신이 오락가락해서 발표를 제대로 듣지는 못했습니다.  
'이장'이라는 닉네임을 쓰시는 [양석원](http://ejang.net/)님의 발표와 곧 장가가는 SEO계의 떠오르는 샛별 [전승엽](https://www.facebook.com/yubsdesign)님의 발표가 인상적이었습니다.  
([발표 자료](http://kopress.kr/wordcamp/meetup-seoul-2015/presentations/)와 [발표 영상](http://kopress.kr/wordcamp/meetup-seoul-2015/video/)을 꼭 보세요~)

(여담 : 이장님과 당일날 탁자를 두고 같이 앉아 있었는데, 인사를 못했습니다. 혹시 저를 기억 못하실까봐 겁나서... 몇 년만에 뵙는거라 소심한 저는 인사를 못했지요... ㅜㅜ )

## Make WordPress Accessible

나름 오랫동안 워드프레스를 사용해오고 있지만, 막연하게 워드프레스가 웹 접근성을 상당히 고려하고 있다고만 알고 있었습니다.  
하지만, 상당한 공헌자들의 노력들이 있었기에 가능한 일이었습니다.  
노력의 질과 양을 보면서 많은걸 깨닫게 되는 계기가 되었습니다.

우선 워드프레스는 코어 뿐만 아니라 테마, 플러그인 등 전반적으로 웹 접근성을 높히기 위한 노력을 하고 있었습니다.  
워드프레스 자체적으로 [다양한 분야에 공헌할 수 있는 기회](http://make.wordpress.org/)가 주어지는데, [접근성](http://make.wordpress.org/accessibility/) 또한 포함되어 있습니다.

> The Make WordPress Accessible team are volunteers who are working to ensure the continued improvement of accessibility within WordPress – both with the themes that power all WordPress websites, and within the admin screens used by site administrators.
> 
> <https://make.wordpress.org/accessibility/>

특히, Accessibility Testing의 경우 배울 점들이 많았습니다.  
체크리스트를 기반으로 각종 코어, 테마, 플러그인 등을 테스트하고 이를 리포팅하고 있습니다.  
모든 과정은 토론을 통해 더나은 결과물을 만들어내고 있었습니다.

[한국 웹 접근성 그룹](http://kwag.net)에서 비슷한 방식으로 국내 웹 사이트 평가를 진행하면 좋겠다고 생각했습니다.

위 URL에 가서 다양한 문서들과 활동 내역을 꼭 확인하길 권고드립니다.  
좋은 자료도 많고, 직접 참여할 수 있는 기회도 있습니다.

아래는 발표를 준비하면서 둘러봤던 사이트들입니다.

  * <https://make.wordpress.org/accessibility/>
  * <https://www.facebook.com/pages/WPAccessibility/412604585533085>
  * <https://developer.wordpress.org/themes/functionality/accessibility/>
  * <http://premium.wpmudev.org/blog/25-ways-to-make-your-wordpress-website-more-accessible/>
  * <https://www.joedolson.com/web-site-accessibility-services/>

## 워드프레스로 웹 접근성 칭찬받기

주로 워드프레스에 관심은 있지만 직접적으로 웹 접근성에 대해 잘 모르시는 분들이 많을 것이라고 예상했습니다.  
발표자료도 그래서 쉽게 준비하였습니다.

웹 접근성의 정의, 장애인의 웹 이용 등과 지침을 설명하는 것으로 시작하였습니다.  
이후 워드프레스 글 작성시 지켜야할 점, 워드프레스로 웹 개발시 신경써야할 부분 등을 예를 들어 설명하였습니다.  
발표 시간이 짧다보니 많은 사례를 준비하지 못했지만, 많은 분들이 공감해주셔서 상당히 즐거운 발표였습니다.

이번 행사를 준비하고 진행한 운영진 분들 모두 고생 많으셨습니다~  
좋은 자리 마련해주셔서 정말 고맙습니다~

### 발표 자료


[워드프레스로 웹 접근성 칭찬받기 (워드프레스 미트업) from Slideshare](www.slideshare.net/jangkunblog/ss-45248628)

### 발표 영상

{% include youtubePlayer.html id=page.youtubeId %}
*워드프레스로 웹 접근성 칭찬받기 발표영상*{: .aligncenter }

## 남는건 사진

어색하지만 찍힌 사진

## 마무리하며

최근 발표 내용을 적어두어야겠다고 생각해서 '억지로' 글 썼습니다.  
후기라고 하기에는 행사의 내용을 담지 못했으니 참가기 정도가 되겠네요...

겸사겸사 기존 블로그 디자인을 버렸습니다.

기본적인 테마는 Themegraphy를 기반으로 했으며, 상당히 많이 커스터마이징했습니다.  
글에 집중할 수 있게 글자 크기를 키우고 내용 외에는 아래로 배치하였습니다.  
폰트도 나눔고딕에서 명조 기반의 [제주 명조체(Jeju Myeongjo)](http://www.google.com/fonts/earlyaccess)를 사용하였습니다.