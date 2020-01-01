---
title: "Git submodule 사용하기"
date: 2020-01-01T20:46:11+09:00
draft: false

# post thumb
# image: "images/featured-post/hugo-logo.svg"

# meta description
description: "git usage"

# taxonomies
categories: 
  - "git"
tags:
  - "git" 
# post type
type: "post"
---
### 1.Git Submodule 사용하기
#### 1) 서브모듈 추가하기
main-mobule: git-main  
sub-module: git-sub  

```
# 메인저장소 clone
git clone <git-main 저장소 URL>
cd git-main 
# 서브모듈 추가
git submodule add <git-sub 저장소 URL> <저장 디렉토리>
# 서브모듈 push
git add <submodule>
git commit -m "메세지"
git push origin master
```

#### 2) 서브모듈이 포함된 저장소 내려받기
```
git clone <git-main 저장소 URL>
# submodule 디렉토리는 아직 비어있음
git submodule init
git submodule update
# submodule 디렉토리 내용이 내려옴
```


