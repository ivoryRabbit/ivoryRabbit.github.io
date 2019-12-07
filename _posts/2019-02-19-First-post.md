---
layout: post
title:  "Hello, world!"
date:   2019-02-19 21:47:45 + 0000
categories: - 일상
author: ivoryRabbit
comments: true
tags: - blog
---

안녕하세요?  
처음으로 깃허브를 이용하여 블로그를 만들었습니다.
 
How are you these days?  
This is my first blog written by github.

* * *
### Python 테스트

{% highlight python %}
def print_hi(name):
  print('Hi, {}'.format(name))

print_hi('Min Song')
{% endhighlight %}

~~~
박스 테스트
abc
~~~

파이썬 실행 - [해시코드 사이트][python]

[python]: https://hashcode.co.kr/code_runners/

```python
def print_your_name():
    your_name = input('Write your name: ')
    print(f'Hello, {your_name}! How are you these days?')
    return
```

* * *


### Table 테스트

언어 | 세부내용(패키지) | 용도
:-- | :-- | --:
`Python` | numpy / scipy / scikit-learn / tensorflow / keras | 머신러닝
`R` | stringr / tidyr / **dplyr** / ggplot2 / survival | 전처리 및 시각화
`SQL` | **_오라클_** | 
`LaTex` | **Overleaf.com** | 문서 작성


* * *
### Latex 테스트

__Log Loss(or cross-entropy)__

$$
L(w) = -\frac{1}{N}\sum_{i=1}^{N}a_{i}\log p_{i}(w)
$$

* * *

{% if site.disqus-shortname %}{% include disqus.html %}{% endif %}
