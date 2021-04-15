---
layout: post
title:  "[Scrapyd] deploy시 scrapyd-deploy 파일이 열리는 현상"
date: 2021-04-15
categories: Scrapyd Scrapy Python
---

<br>

scrapyd-deploy를 커맨드 창에 입력했는데 

<b>scrapyd-deploy</b> 파일이 오픈되는 현상이 나타났다.

<br>

서치해본 결과 그 파일(scrapyd-deploy)을 복사해서 스크래피 프로젝트 폴더에 붙여넣기 해주면 된다.



<br>

+) 추가적으로 아래와 같은 에러가 발생했었다.

```
scrapyd-deploy:23: ScrapyDeprecationWarning: Module `scrapy.utils.http` is deprecated, Please import from `w3lib.http` instead.
```

<br>

```
# from scrapy.utils.http import basic_auth_header
from w3lib.http import basic_auth_header
```

위와 같이 첫번째 줄 코드를 주석처리 해주고 두번째 줄 코드를 추가한다.