---
layout: post
title: "[Python] SQLAlchemy"
date: 2021-04-30
categories: Python
---

<br>

원래 개발할 때 pymysql, pymssql 등 사용했었는데 통합적으로 쓸 수 있는 sqlalchemy를 사용하려고 시도 중이다.

<br>

```
pip install sqlalchemy
```

<br>

```
from sqlalchemy import create_engine

engine = create_engine('mssql+pymssql://username:password@host/database')
```

뒤에 database는 기재하지 않아도 된다. 그리고 만약 mysql을 사용하려면 mysql+pymysql로 변경해주면 되겠다.

<br>

```
rows = engine.execute(query)
```

따로 engine.connect() 를 하지 않고 execute를 하면 된다. (그 과정 속에 connect 가 됨.)