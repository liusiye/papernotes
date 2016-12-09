## Topic-Based-Chinese-Message-Sentiment-Analysis:-A-Multilayered-Analysis-System
  腾讯在2015中文主题情感分类任务上的模型 top1
 
- key1(分层模型)
  文章针对任务包含实体和事件两方面的情感分析. 模型主要分为3层, 首先是将微博分类为实体相关微博,事件相关微博; 第二层将提取出和实体或事件相关的微博; 第三层
 对微博中的情感进行分析
- key2(特征工程)
  文章中的特征主要采用N-gram Feature(50万), Feature Select Algorithm:(TF-IDF, X2-Test); PMI Feature 特别相关的特征; 情感词汇表
