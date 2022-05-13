---
layout: post
title: NLP 공부
subtitle: Natural Language Processing
cover-img: /assets/NLP-img/cover.png
<!-- thumbnail-img: https://gpigp.github.io/taehyun/assets/post2-img/marmoset.jpg -->
tags: [NLP, Pytorch]

published: true
---

NLP
============================
<br>
<h6> one-hot Encoding with scikit learn </h6>
``` python
from sklearn.feature_extraction.text import CountVectorizer

corpus              = ["Natural Language Processing"]
one_hot_vectorizing = CounterVectorizer(binary=True)
ohe                 = one_hot_vectorizing.fit_transform(corpus).toarray()
voca                = one_hot_vectorizing.get_feature_names()
```
<br>

<h6> TF : Term Frequency </h6>
one-hot representation들의 합
<br><br>

<h6> IDF : Inverse Document Frequency </h6>
흔한 토큰의 점수는 낮추고, 드문 토큰의 점수를 높임
~~~ python
from sklearn.feature_extraction.text import TfidfVectorizer

corpus    = ["Natural Language Processing"]
tfidf_vec = TfidfVectorizer()
tfidf     = tfidf_vec.fit_transform(corpus).toarray()
~~~
<br>

<h6> (_) 밑줄의 의미 </h6>
fill_(), normal_() 등과 같은 in-place 메소드는 새로운 객체를 생성하는게 아닌 현재값을 변경해준다.
<br><br>

<h6> tensor type 변환 </h6>
~~~ python
x  = torch.rand(2,3,4) # [2,3,4] -> [3,4]가 2개
x1 = x.view(2,-1)      # [2,12]
x2 = x.transpose(0,2)  # [4,3,2] -> [2,3]가 4개
x3 = x.permute(2,1,0)  # [4,3,2]
~~~
<br>
<span style="color: #2D3748; background-color: #fff5b1">2022.05.12.wrote</span>
<br>






