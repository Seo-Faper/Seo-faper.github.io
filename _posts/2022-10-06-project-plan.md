---
layout: post
title: 프로젝트 계획서 (롤스타브 투게더)
date: 2022-10-06 00:18:23
author: seo-faper
categories: ruby
short_description: 돈스타브 투게더 모드를 만들어 보고 싶어짐
image_preview: https://raw.githubusercontent.com/Seo-Faper/cq_assets/master/heroes/cos_pr_17_23.png
---

## 롤 보이스를 돈투에 넣어 보면 재밌지 않을까! 
---

### 구상 

플레이어가 사망 시 사망한 플레이어와 죽인 몬스터의 초상화 뜨면서 롤 음성이 나오는 것

외국 유저가 많은 것을 감안해 영어로 통일

첫 번째 플레이어가 사망하면 `First Blood`

그 이후에 플레이어 사망 시 `Enemy Slain`

플레이어 부활 하기 전에 또 다른 플레이어가 죽을 시 `Dobule-Triple-quadr-penta-kill`

팬타킬 이후엔 그냥 `Enemy Slain`

모든 플레이어가 사망하면 `Ace`

플레이어가 부활 하고 자신을 죽인 몹에게 복수하면 `Shut down`

### 사용 기술 스택

Lua 스크립트

tex Editor <a herf="https://ko.overleaf.com/" target='_blank' >(link)</a>

### 목표 개발 기간 

~ 2022-12-31

### 세부 개발 계획


#### 자료 검색

- 돈스타브 투게더 플레이어 사망 시 발생하는 이벤트 확인
- 채팅 메세지에 로그를 지울 수 있는 방법 찾기
- 채팅 메세지에 `~가 ~에 의해 끔찍한 유령이 되었습니다.` 라는 메세지가 뜬다는 점, 이것은 서버 모드 단에서 한글패치 한 사례를 보아 충분히 편집 가능, 방법을 모를 뿐 불가능한건 아님
- 특정한 좌표에 이미지를 띄우는 방법 찾기
- 사망 시 중앙 상단에 롤 적 처지 이미지를 띄워야함 

#### 리소스 확보

- 롤 적 처치 시 뜨는 모양 누끼딴 이미지 필요 (초상화만 비워둔 이미지)
- 돈스타브 캐릭터 초상화
- 돈스타브 몬스터 초상화

<img src="https://raw.githubusercontent.com/Seo-Faper/seo-faper.github.io/main/img/23.JPG" width="100%">
대충 이런 느낌

### 2022-10-13 중간 점검

- 기본적인 돈스타브 투게더 모드 구조 확인 

- 비슷한 UI를 건드는 모드 4건 정도 찾아놈
- 왼쪽 하단이나 오른쪽 하단에 새로운 임의의 이미지 버튼을 만드는 모드 발견
- 그 이미지를 중앙 상단으로 올리는 방법을 찾아야함

- 사망 시 메세지를 바꾸는 모드 찾아야함
