---
layout: post
title:  "[Scrapyd] scrapyd 스케줄 등록"
date: 2021-05-09
categories: Scrapyd Scrapy Python

---

<br>

필자는 windows 환경에서 프로젝트를 진행하고 있다.

 curl 명령어를 위해서 *Cmder* 라는 프로그램을 이용했다.

<br>

<h3>스케줄 등록</h3>

```
curl http://localhost:6800/schedule.json -d project=project명 -d spider=spider명
```

<br>

아래처럼 화면에 출력되면 스케줄이 등록된거다.

![image](https://user-images.githubusercontent.com/42509019/117577195-bc890480-b123-11eb-9950-bb62f69ba165.png)

<br>

<h3>스케줄 삭제</h3>

```
curl http://localhost:6800/cancel.json -d project=project명 -d job=jobid
```



위 명령어를 입력 후 확인해보면 스케줄이 삭제된 걸 알 수 있다.

<br>