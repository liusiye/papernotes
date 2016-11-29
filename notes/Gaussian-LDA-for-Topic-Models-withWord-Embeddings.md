## Gaussian LDA for Topic Models withWord Embeddings
  这篇文章主要讲述了如何使用word embedding来替代原有LDA model中的word
- key1
 - 文章采用word embedding来代替原有的word, 认为文章是由一系列word embedding构成的
 - 因此topic 的表现形式也与之前的狄利克雷分布不同, 采用了高斯分布作为topic的先验模型, 这样topic一方面语义一致，另一方面可以表示word embedding的分布
 - 文章中的计算方法没有细看
 
[[github_link]](https://github.com/rajarshd/Gaussian_LDA)
