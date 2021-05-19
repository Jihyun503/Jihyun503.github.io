---
layout: post
title:  "[Scrapyd] scrapyd 작업이 끝나지 않는 현상"
date: 2021-05-19
categories: Scrapyd Scrapy Selenium Python
---

<br>

scrapyd 실행 시 로그에는 Spider closed 라고 찍히는데, 웹 들어가서 확인해보면 finish가 안되있는 현상이 발생했다.

문제의 원인을 찾아본 결과, 셀리니움(selenium) 때문이라는 걸 알게 되었다.

(필자의 프로젝트는 scrapy와 selenium이 같이 사용됨.)

<br>

기존 코드에 driver.close() 해줬던 걸

```
driver.quit()
```

로 수정하니까 정상적으로 finish가 됨.