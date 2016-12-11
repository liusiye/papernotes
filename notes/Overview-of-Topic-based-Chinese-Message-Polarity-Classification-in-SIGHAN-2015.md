## Overview of Topic-based Chinese Message Polarity Classification in SIGHAN 2015
  这个比赛针对的是topic sentiment
- key1
 - 数据是按照topic筛选来的，由3人完成标注. 一致kappa系数0.88左右
 - 最好的模型是腾讯和哈工大研究院跑出来的
 - 25个topic, 共25000个微博句子
 - 在标注数据的过程中，如果对于同一个topic有两种情感，选择较强的那个情感
 - 在标注数据时, 用NTUSD2将neural句子筛除
 - 负面句子占比10.97%,和正面句子占比都存在这这方面的问题
