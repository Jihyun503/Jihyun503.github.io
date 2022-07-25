---
published: true
layout: post
title:  "[Selenium] 'WebDriver' object has no attribute 'find_element_by ...' 에러"
date: 2022-07-19
categories: Python Selenium

---

<br>

셀리니움을 이용하여 크롤링 하는 코드를 작성하던 중에 에러가 발생하였다.

```
'WebDriver' object has no attribute 'find_element_by_class_name'
```

검색해본 결과, 셀리니움 상위버전에서 나타나는 에러라는 걸 확인.

<br>

```
from selenium.webdriver.common.by import By
```

일단 위와 같이 import를 추가해준다.

find_element_by_ ... 라는 문법은 상위버전에서 에러가 난다.

>  `find_element("어떤 속성으로 추출할건지", "속성의 값")`

로 변경해서 사용해주면 되겠다.

<br>

내 에러로 예시를 들자면

```
#driver.find_element_by_class_name("test")
driver.find_element(By.CLASS_NAME, "test")
```

로 수정해주면 정상 동작한다. 

~~속성이라고 표현하는 게 맞는지 긴가민가하지만..~~

