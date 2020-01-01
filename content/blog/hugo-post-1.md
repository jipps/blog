---
title: "Hugo로 블로그 만들기"
date: 2020-01-01T13:57:21+09:00
draft: false

# post thumb
image: "images/featured-post/hugo-logo.svg"

# meta description
description: "this is meta description"

# taxonomies
categories: 
  - "Blog"
tags:
  - "Hugo" 
# post type
type: "post"
---
> 참고:
> 1. [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)
> 2. [Hugo Hosting & Deploymeny - Host on GitHub](https://gohugo.io/hosting-and-deployment/hosting-on-github/)

# 1.Hugo Quick Start
### 1) Hugo 설치하기
> MacOS 기반 HomeBrew 이용 설치 가이드  
> 타 OS는 여기를 참고하세요. https://gohugo.io/getting-started/installing
```sh
brew install hugo
hugo version
```

### 2) 사이트 신규로 만들기
```
hugo new site blog
```

### 3) 테마 추가하기
> 추가할 테마: liva-hugo  
> Hugo 테마는 여기를 참고하세요.  https://themes.gohugo.io/
```
cd blog
git init
git submodule add https://github.com/themefisher/liva-hugo.git themes/liva-hugo 
```

themes/liva-hugo/exampleSite밑에 있는 config.toml참고하여 blog밑에 있는 config.toml을 수정한다.

### 4) Content 추가하기
Content 파일은 수동으로 추가하거나 hugo 명령어를 통해 추가가능하다.  
수동으로 파일생성시 ```content/<CATEGORY>/<FILE>.<FORMAT>``` 형태로 생성하고  
hugo 명령어로 생성시는 아래와 같이생성한다.   
```
hugo new posts/post-1.md
```

### 5) Hugo Server 시작하기
Content 파일은 수동으로 추가하거나 hugo 명령어를 통해 추가가능하다.  
수동으로 파일생성시 ```content/<CATEGORY>/<FILE>.<FORMAT>``` 형태로 생성하고  
hugo 명령어로 생성시는 아래와 같이생성한다.  

