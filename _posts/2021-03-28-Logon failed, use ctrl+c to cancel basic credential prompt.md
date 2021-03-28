---

layout: post
title:  "[Git] Logon failed, use ctrl+c to cancel basic credential prompt"
date: 2021-03-28
categories: Git

---

<br>

오랜만에 git push 하려고 하니까 못보던 에러가 발생했다.

<br>

```python
Logon failed, use ctrl+c to cancel basic credential prompt
```

찾아본 결과, 깃 업데이트 문제였다.

<br>

```python
git update-git-for-windows
```

위 명령어를 입력하면 문제없이 푸시가 된다.