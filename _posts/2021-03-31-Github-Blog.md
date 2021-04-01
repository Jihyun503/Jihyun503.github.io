---
layout: post
title:  "Github Blog 만들기"
date: 2021-03-31
categories: Git Jekyll Ruby
---

<br>

공부한 내용 정리나, 발생했던 에러에 대한 해결책을 기록해놓기 위해서 Github Blog를 만들어야겠다는 생각이 들었다. 

<h2>그리하여 ✨깃허브 블로그 만들기 대작전 ~!✨</h2>
<br>

우선적으로 깃허브에 레포지터리를 {username}.github.io 라는 이름으로 만든다.

![image](https://user-images.githubusercontent.com/42509019/113163050-c3963a80-927a-11eb-916a-1d852d2086e6.png)

<br>

레포지터리가 잘 만들어진 걸 확인한 후에 작업할 폴더를 하나 만들고 clone을 받는다.

```
git clone 복사한 레포지터리 주소
```

<br>

원격저장소와 연결이 됐으면 다음 단계로 넘어간다. 블로그의 테마를 골라야하는데, 지킬테마가 상당히 다양하기 때문에 고르는 재미가 쏠쏠했다. 아래의 링크들을 참고해서 선택하면 될 거 같다.

- [http://jekyllthemes.org/](http://jekyllthemes.org/)

- [https://jekyllthemes.io/free](https://jekyllthemes.io/free)

- [http://themes.jekyllrc.org/](http://themes.jekyllrc.org/)

(필자가 선택한 테마는 [https://github.com/samarsault/plainwhite-jekyll](https://github.com/samarsault/plainwhite-jekyll))

<br>

테마를 골랐으면 다운 받는다.

![image](https://user-images.githubusercontent.com/42509019/113311629-79798b80-9344-11eb-986d-8d39e3876357.png)

Downloda ZIP !



다운 받은 폴더를 열어서 모든 파일을 복사, 원격 저장소와 연결시킨 폴더로 붙여넣기 해준다.

<br>

이제 루비를 다운 받아야한다.

[https://rubyinstaller.org/downloads/](https://rubyinstaller.org/downloads/)



![image](https://user-images.githubusercontent.com/42509019/113312936-be51f200-9345-11eb-9b7f-d15f20fd8502.png)

필자는 2.7.2 버전을 다운 받았다. 다운로드하여 설치까지 완료하자.

<br>

```
gem install jekyll bundler
bundle install
```

루비가 다 설치 되었다면 cmd창을 열어서 원격저장소 경로로 이동한다.

그리고 위 명령어를 입력하면 설치가 완료될 것이다.

<br>

```
bundle exec jekyll serve
```

![image](https://user-images.githubusercontent.com/42509019/113317938-e4c65c00-934a-11eb-9cc5-36b98e6d740d.png)

이제 http://127.0.0.1:4000 를 접속하면 내가 다운 받은 테마와 같은 웹페이지가 뜨는 걸 확인 할 수 있다. github에 푸시하기 전에 로컬에서 작업하고 확인할 수 있는 환경이 구성되었다.

<br>

이제 파일들을 내가 원하는 스타일에 맞춰서 커스터마이징한 후 깃헙에 푸시하면 블로그 완성!

<br>

