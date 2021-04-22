---
layout: post
title:  "[Anaconda] conda 명령어"
date: 2021-04-22
categories: Anaconda
---

<br>

내가 편하게 보기 위해서 정리하는 conda 명령어

<br>

가상환경 리스트 조회

```
conda env list
```

가상환경 생성

```
conda create -n 가상환경 이름
```

가상환경 복사

```
conda create --clone 복사할 가상환경 이름 -n 만들 가상환경 이름
```

가상환경 활성화

```
conda activate 가상환경 이름
```

가상환경 비활성화

```
conda deactivate
```

가상환경 삭제

```
conda env remove -n 가상환경 이름
```

