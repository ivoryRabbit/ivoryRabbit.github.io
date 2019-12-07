---
layout: post
title:  "Discrete Geometry"
date:   2019-03-07 13:45:45 + 0000
categories: - 수학
author: ivoryRabbit
comments: true
tag: - descrete geometry
---

안녕하세요?

이번에 제 지도교수이신 Andreas Holmsen 교수님과 논문 하나를 제출하게 되었습니다.

석사 졸업과 함께 처음이자 마지막으로 수학 분야에서 논문 출판을 경험하는 기회를 갖게 되어 기분이 오묘하네요. 논문은 이스라엘 수학 저널에 제출한 상태이며, [arxiv][arxiv]에서 찾아보실 수 있습니다.

Discrete Geometry는 많은 사람들, 특히 수학자들에게도 생소한 분야인데, 수학자 [Paul Erdős][Erdos]의 뒤를 이어 연구되고 있는 조합론의 한 분야라고 생각하시면 되겠습니다. 제가 공부하면서 사용했던 수학은 주로 조합론, 그래프이론, 선형대수학, 위상수학 정도였습니다.

논문의 내용은 Hadwiger-Debrunner의 (p,q)-problem입니다. 굉장히 조합적으로 기술된(combinatorial statement) 이 문제는 arbitrary dimensional Euclidean space에서 Alon과 Kleitman에 의해 1992년에 증명되어 이제는 (p,q)-theorem으로 불리게 되었습니다.

문제가 조합적으로 기술된 것에 비해, 증명은 Euclidean space의 다양한 성질을 사용하게 됩니다.
- Linear independence (dimension)
- Lexicographic order

제 연구 목표는 dimension을 Radon number라고 불리는 불변량(invariant)로 대체하면서 동시에 lexicographic order을 사용하지 않은, purely combinatorial proof를 찾는 것이었습니다.

결과적으로 (p,q)-problem의 중간단계인 'colorful Helly theorem'을 ['Radon number'][Radon]와 ['Stirling number of the second kind'][Stirling]를 이용하여 증명하는데 성공하였고, 다른 연구 결과들과 함께 (p,q)-theorem까지 도달할 수 있었습니다.


[arxiv]: https://arxiv.org/abs/1903.01068
[Erdos]: https://en.wikipedia.org/wiki/Paul_Erd%C5%91s
[Radon]: https://en.wikipedia.org/wiki/Radon%27s_theorem
[Stirling]: https://en.wikipedia.org/wiki/Stirling_numbers_of_the_second_kind

{% if site.disqus-shortname %}{% include disqus.html %}{% endif %}
