---
layout: post
title: NLP 공부
subtitle: Natural Language Processing
cover-img: /assets/post2-img/indel_blue.jpg
thumbnail-img: https://gpigp.github.io/taehyun/assets/post2-img/marmoset.jpg
tags: [NLP, Pytorch]

published: true
---

NLP
============================
<br>
<h6> one-hot Encoding with scikit learn </h6>
```Python
from sklearn.feature_extraction.text import CountVectorizer

corpus = ["Natural Language Processing"]
one_hot_vectorizing = CounterVectorizer(binary=True)
ohe = one_hot_vectorizing.fit_transform(corpus).toarray()
voca = one_hot_vectorizing.get_feature_names()
```
<br>

<h6> TF : Term Frequency </h6>
one-hot representation들의 합
<br><br>

<h6> IDF : Inverse Document Frequency </h6>
흔한 토큰의 점수는 낮추고, 드문 토큰의 점수를 높임
```Python
from sklearn.feature_extraction.text import TfidfVectorizer

corpus = ["Natural Language Processing"]
tfidf_vec = TfidfVectorizer()
tfidf = tfidf_vec.fit_transform(corpus).toarray()
```
<br>

<h6> (_) 밑줄의 의미 </h6>
fill_(), normal_() 등과 같은 in-place 메소드는 새로운 객체를 생성하는게 아닌 현재값을 변경해준다.
<br><br>





