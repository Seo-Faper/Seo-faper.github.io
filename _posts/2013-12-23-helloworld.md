---
layout: post
title: 깃허브 페이지 만들 때 팁
date: 2022-10-06 00:18:23
categories: ruby
short_description: 깃허브 블로그 만들 때 삽질한 기록
image_preview: https://raw.githubusercontent.com/Seo-Faper/cq_assets/master/heroes/cos_pr_17_17.png
---

# 블로그 만들 때 배포가 안될 시 (404)

자기가 커밋한 내용에 갈색깔 동그라미 누르면 특별하게 커밋의 진행과정을 볼 수 있는데
거기서 ruby의 어디 문법이 잘못되었는지 확인 해 보면 된다.

# _post에 쓴 글이 보이지 않을 때

`future: true` 를 _config.yml에 추가

# 자바스크립트가 jekyll에서 먹지 않을 시

`<script src="a.js"></scrpit>`를 선언 하고 그 안에 자바스크립트를 넣지 말고
아래에 새로운 `<script></script>` 태그를 만들고 그 안에서 스크립트를 짤 것  