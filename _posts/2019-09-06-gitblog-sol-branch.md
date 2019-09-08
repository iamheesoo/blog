---
layout: post
cover: 'assets/images/cover4.jpg'
navigation: True
title: "[Github블로그] 블로그에 코드 적용이 안될 때, 프로젝트 주소 페이지는 브랜치 체크"
date: 2019-09-06 19:33:00
tags: github blog
subclass: 'post tag-test tag-content'
logo: 'assets/images/ghost.png'
author: casper
categories: casper
---
미루고 미루던 유저네임을 변경했다.

덕분에 블로그 css가 또 망가졌다. ~~나 광광울어~~

F12로 블로그를 체크해보니 경로주소가 자꾸 이상한 곳을 가리키고 ~~난 분명히 baseurl 바꿨는데~~ config.yml에 정보를 가져다 쓰지 않고 갓 fork할 때 본 초기 블로그 모습을 보여줬다.

몇 시간의 구글링 결과 branch가 잘못되었음을 확인하였다.

프로젝트 주소 페이지의 경우(USERNAME.github.io/repo) push할 때 gh-page 브랜치를 이용해야한다.
~~왜때문인지는 이해하지 못했다. 그리고 유저네임 바꾸기 전에는 master로 잘 해왔는데 이제와서 안되는 것도 이상하다.~~

아무튼 <span style="color:red">해결 방법</span>은 너무 간단해서 화가 났다^.^

**setting에서 브랜치를 마스터로만 바꿔주면 된다!**

![190906_1](./assets/images/190906_1.png)
레파지토리의 setting을 클릭 후

![190906_2](./assets/images/190906_2.png)
아래로 스크롤을 내려서 gh-pages branch를 master로 바꿔주면 된다.

후...이제 css깨지는 건 해결했고 카테고리가 왜 안되는지 찾아야한다. 아무것도 건드린게 없는데 왜 404인지 정말 모르겠다. 울고 싶다...