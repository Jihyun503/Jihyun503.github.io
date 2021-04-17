---
layout: post
title:  "[Scrapyd] scrapyd deploy"
date: 2021-04-17
categories: Scrapyd Scrapy Python
---

<br>

1. ```
   pip install scrapyd
   ```

   <br>

2. ```
   pip install scrapyd-client
   ```

   <br>

3. ```
   scrapyd
   ```

   위 명령어 입력해서 에러없이 잘 작동하면 O

4. 파이썬 동작 환경 폴더에서 scrapyd-deploy 파일 복사해서 스크래피 프로젝트 안에 붙여넣기

   (필자는 \anaconda3\Scripts 에 있었음)

5. scrapy.cfg 에 url 주석 제거

6. scrapyd를 실행한 상태에서 커맨드창에 

   ```
   scrapyd-deploy default -p 프로젝트명
   ```

   입력해서 별 이상없이 출력되면 일단은 성공

   ![KakaoTalk_20210416_155346087](https://user-images.githubusercontent.com/42509019/115101110-8f11c680-9f7c-11eb-9a17-8501fdff2293.png)