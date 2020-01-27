---
layout: post
title: "Tidyverse and Pandas"
date: 2020-01-15 23:05:59
author: ivoryRabbit
categories: 개발
comments: true
tag: 파이프연산자
---

## Tidyverse

R **tidyverse** 라이브러리를 사용하면서 파이프연산자(%>%)를 이용하는 것이 많은 장점을 갖고 있다는 것을 느꼈다. 코드가 직관적이고 보기 좋을뿐만아니라, 하나의 코드블럭만으로 데이터 핸들링부터 시각화가 가능하기 때문에 불필요하게 많은 변수들을 생성할 필요가 없었기 때문이다. 

Python **pandas**에서도 이러한 장점을 유지하면서 나만의 개성있는 데이터 핸들링 코드를 짜고 싶은 바람에 검색해보다가 찾아낸 좋은 블로그가 있다.
- [https://stmorse.github.io/journal/tidyverse-style-pandas.html](https://stmorse.github.io/journal/tidyverse-style-pandas.html){: target="_blank" }

단순히 데이터 핸들링뿐만이 아닌, seaborn을 이용한 시각화까지 파이프연산자(.pipe)를 통해 우아하게 프로그래밍할 수 있다. 하지만 다른 자료들과 마찬가지로, 과도한 파이프연산자 사용을 지양하고 있으니 주의해야겠다.