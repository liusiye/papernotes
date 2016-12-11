## A Joint Model for Chinese Microblog Sentiment Analysis
  文章是sighan中的第二名
- key1
 - SVM 特征n-gram n-pos 和情感词
 - 情感词可能需要进行扩充, 文章中有提到refer
 - 用CNN进行情感分析, 有提到refer
 - CNN主要用了max-time-polling, 但是具体如何训练没有详细说明, 但是有相关文献,可以继续查看
 - topic体现在先对句子进行分类, 判断句子是否时topic相关的句子. 方法是: 将某个topic下的常见单词聚集出来, 用这些单词进行topic的分类
