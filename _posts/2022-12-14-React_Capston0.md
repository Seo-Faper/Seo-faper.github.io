---
layout: post
title: _[React js]_ useState()에 대한 고찰
date: 2022-12-11 03:10:23
categories: react
short_description: 플젝 하면서 생긴 일
image_preview: https://raw.githubusercontent.com/Seo-Faper/cq_assets/master/heroes/cos_pr_17_17.png
---

> 백엔드가 json을 뿌려주면 프론트가 주워서 예쁘게 화면에 출력한다.

이게 정말 간단히 설명한 웹 서비스 동작방식이라고 생각한다. 

단순히 정보를 받기만 하면 `GET` 이고
서버에게 사용자의 정보를 담아서 결과를 받고 싶으면 `POST` 이다.

useState()는 쉽게 말하자면 특정 변수를 바꾸기 위해서 핸들링 하는 기능이다.
![](https://raw.githubusercontent.com/Seo-Faper/seo-faper.github.io/main/img/img1.JPG)
이런 컴포넌트가 있을 때, 실시간으로 사용자가 체크를 풀었다 걸었다 할 때 마다 서버에게 보내줄 json의 true, false도 바뀌어야 한다.
그 때 바로 useState()를 쓴다. 