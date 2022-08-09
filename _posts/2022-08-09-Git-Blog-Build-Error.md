---
layout: post
title:  "Git Blog 포스팅 커밋시 빌드 에러"
date: 2022-08-09
categories: Git Jekyll
---

<br>

한동안 깃 블로그에 글이 제대로 올라가지 않아 골머리 썩였다. 

확인해보니 빌드 과정에서 에러가 발생한 것이었다.

```
The plainwhite theme could not be found. (Jekyll::Errors::MissingDependencyException)
```

저기서 'Plainwhite' 는 내가 사용한 테마명이다.

<br>

찾아본 결과 _config.yml 을 수정하면 된다고 한다.

```
#theme: plainwhite
```

원 코드에 주석 하나 추가해서 다시 커밋해주었다.

이제 귀신 같이 에러가 안남!