---
layout: post
lang: ko
title: Github Pages에 Custom Domain 설정하고 DNS 세팅하기
permalink: /wp/using-custom-domain-and-dns-with-github-pages/
date:   2018-12-05
categories:
  - Git
tags:
  - Git
  - Github
  - Github-pages
excerpt: fff [...]
image:
  src: 'using-custom-domain-and-dns-with-github-pages.png'
views:
  - "0"
---

나는 [미리내](https://www.mireene.com/){: target="_blank" }에서 호스팅과 도메인 관리를 하고 있다. 따라서 내 글은 미리내 기준이다. 

## DNS 세팅하기

Github 문서와 블로그들을 둘러보고 DNS 세팅을 따라 했고, 다음날 도메인이 연결되어 큰 문제 없는 줄 알았다.  
하지만, 다음날 Github에서 메일로 수정해야할 부분을 아래와 같이 친절히 알려주었다.

### A records

더 자세히 등록하면 좋겠지하면서 DNS A record에 `www` 서브도메인도 모두 IP를 등록했었다.  
하지만, Github 메일에서는 아래 4개의 IP를 `www`와 같은 **서브도메인 없이 등록**해야한다고 한다.

* 185.199.108.153
* 185.199.109.153
* 185.199.110.153
* 185.199.111.153

![미리내 내 DNS 관리에서 A 레코드 수정](/assets/img/2018/201812_github_dns_1.png){: .aligncenter}
*[미리내 내 DNS 관리에서 A 레코드 수정]*{: .aligncenter }

### CNAME record

CNAME도 도메인 둘 다 등록했는데, Github에서 `www` 서브 도메인을 붙여서 하나의 CNAME만을 등록하라고 했다.  
이때 CNAME의 종착지는 Github Repository 주소를 작성한다.

* jangkunblog.github.io

![미리내 내 DNS 관리에서 CNAME 수정](/assets/img/2018/201812_github_dns_2.png){: .aligncenter}
*[미리내 내 DNS 관리에서 CNAME 수정]*{: .aligncenter }

