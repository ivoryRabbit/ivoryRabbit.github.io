---
layout: post
title:  "NIMS 산업수학"
date:   2019-02-24 15:38:45 + 0000
categories: 개발
comments: true
author : ivoryRabbit
tag: NIMS 
---
 
안녕하세요?  
깃허브를 통해 두번째로 만나뵙게 되었습니다.
 
제 4회 NIMS 산업수학 아카데미에 참석하여  
산업수학 문제해결에 필요한 데이터 분석을 공부하고 있습니다.
 
개발환경은 Python - Jupyter Lab이며,  
문제해결 및 데이터 분석에 사용할 모듈들을 conda 가상환경에 설치하였습니다.
 
그런데 저의 conda 가상환경에는 Jupyter Lab이 실행되지 않더군요.
 
<center><img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%841.png?raw=true" width="1080"></center>


보다시피 계속해서 다음과 같은 메세지가 뜹니다:  
__'jupyter'은(는) 내부 또는 외부 명령, 실행할 수 있는 프로그램, 또는
배치 파일이 아닙니다.__

왜 안될까 뒤적거리다가 힌트를 찾아내었습니다. 

<center><img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%842.png?raw=true" width="1080"></center>

제가 사용하는 Directory는 다음과 같은데,  

```
C:\Users\이동규
```
이 사용자 폴더의 한글 이름이 유니코드로 잘못변환되어 에러가 난다고 추측하였습니다. 
 
제가 생각해낸 해결방법은 administrator 계정을 NIMS 세미나 기간동안에만 활성화 시켜, 그곳에서 conda 가상환경을 설치 및 사용하는 것입니다.

1. 먼저 cmd를 실행시킨 후, 다음 명령어를 입력합니다. 

```
net user administrator /active:yes
```
<center><img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%843.png?raw=true" width="1080"></center>

2. 그러면 administrator 계정이 활성화되는데, window키+x를 눌러 로그아웃하면 administrator로 접속할 수 있습니다.  

3. conda를 이용하여 가상환경을 설치한 후, Jupyter Lab을 실행시켜보면 앞의 오류가 사라집니다.

<img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%844.png?raw=true" width="1080" >
<img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%845.png?raw=true" width="1080" >

4. Jupyter Lab에서 가상환경에 설치한 모듈들을 실행시켜보면, 잘 작동하는 것을 확인할 수 있습니다.

<img src="https://github.com/ivoryRabbit/ivoryRabbit.github.io/blob/master/assets/20190224/%EC%82%AC%EC%A7%846.png?raw=true" width="1080" >

5. administrator를 비활성화시키고 싶다면 yes -> no로 바꾸어줍니다.
```
net user administrator /active:no
```


* * *
__Reference__ 

* <a href="https://pinkwink.kr/1097" target="_blank"> conda 가상환경에서 jupyter 설치 </a>

* <a href="https://answers.microsoft.com/ko-kr/windows/forum/windows_10-security/window-10-%EC%82%AC%EC%9A%A9%EC%9E%90/fe12dc88-2705-42fd-a76b-674dbe3a0808" target="_blank"> 사용자 폴더 이름이 한글일 때 </a>

* <a href="https://ahribori.com/article/5a03bcfd6c9eef13d882e29a" target="_blank"> 마크다운 이미지 관련 참조 </a> 

* <a href="https://blog.ayukawa.kr/archives/1290 target=_blank"> 마크다운 문법 참조 </a>

* * *

[제 4회 NIMS 산업수학 아카데미][NIMS] 참석

[NIMS]: https://www.nims.re.kr/scholarship/post/seminar/33128

* * *

{% if site.disqus-shortname %}{% include disqus.html %}{% endif %}
