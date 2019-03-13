---
layout: post
title:  "Hello, surffers!"
date:   2019-02-19 21:47:45 + 0000
categories: blog
author: ivoryRabbit
comments: true
tags: ipsum
---

안녕하세요?  
처음으로 깃허브를 이용하여 블로그를 만들었습니다.
 
How are you these days?  
This is my first blog formed by github.

* * *
### Python 테스트

{% highlight python %}
def print_hi(name):
  print('Hi, {}'.format(name))

print_hi('Min Song')
%'Hi, Min Song' to STDOUT.
{% endhighlight %}

파이썬 실행 - [해시코드 사이트][python]

[python]: https://hashcode.co.kr/code_runners/

```python
def print_your_name():
    your_name = input('Write your name: ')
    print(f'Hello, {your_name}! How are you these days?')
    return
```
* * *

### Latex 테스트

__Log Loss(or cross-entropy)__

$$
L(w) = -\frac{1}{n}\sum_{i=1}^{N}a_{i}\log p_{i}(w)
$$

* * *

{% if site.disqus-shortname %}{% include disqus.html %}{% endif %}
