---
title: "Git 기본 명령어"
date: 2020-01-04T10:31:11+09:00
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
### 1.Git 이용 초간단 과정
#### 1) Remote repository 생성
> [Github](https://github.com/) 또는 [Bitbucket](https://bitbucket.org/)에서 repository 생성
#### 2) Local 개발 환경 연결
> Git 서버와 Local 개발 환경을 동기화하는 방법은 2가지가 있다.  
> * git clone을 통해 git 서버 Contents를 내려받으면서 local git 환경 자동 세팅  
> * local에서 git 초기화를 한 후 remote 서버와 연결한느 방법
#### 3) git clone 이용하기
```
git clone <저장소URL>
```
#### 4) git init을 이용 저장소 연결하기
```
# local repository 생성
git init
# remote repository 연결
git remote add origin <저장소 URL>
```
#### 5) 파일 추가
```
git add <file>
git commit -m "<메세지>"
git push --set-upstream origin master
(--set-upstream = -u, default )
```
#### 6) 파일 가져오기
```
git pull [--allow-unrelated-histories]
```
* git push할때 fatal:refusing to merge unrelated histories 오류 발생할때 --allow-unrelated-histories 옵션을 추가한다.
* 서로 관련 기록이 없는 이질적인 두 프로젝트를 병합할때 git에서는 기본적으로 오류가 발생하는데 이것을 허용해 주는 것이다.

