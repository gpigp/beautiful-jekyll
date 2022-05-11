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

<h6> one-hot vector with scikit learn </h6>
```python
from sklearn.feature_extraction.text import CountVectorizer

corpus = ["Natural Language Processing"]
one_hot_vectorizing = CounterVectorizer(binary=True)
ohe = one_hot_vectorizing.fit_transform(corpus).toarray()
voca = one_hot_vectorizing.get_feature_names()
```
<br>

<h6> TF : Term Frequency </h6>
문장에서의 one-hot representation들의 합
