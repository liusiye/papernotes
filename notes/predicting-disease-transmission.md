## Predicting Disease Transmission from Geo-Tagged Micro-Blog Data

### key points
   作者利用tweet数据进行了潜在病人识别的应用，论文中关键点主要有两点:

- key1(tweet数据的筛选)
  - 首先人工标注构建小样本的数据集(数量5000),这些数据用来训练两个分类器:C1,C2, 其中C1focus on 避免将sick tweet识别为 normal tweet, C2 focus on 避免将normal tweet 识别为 sick tweet
  - 将(百万样本)大量数据通过C1、C2的分类器, 分别将C1、C2种top10%的数据筛出，这样就确保了这部分数据分别是sick 和 normal的数据集
  - 最后将上一步的数据用来训练C3分类器，C3做为最终分类器使用
- key2(CRF对病人的健康进行监控)
  - 将病人随时间变化的健康信息,及观测状态看成NER问题,用CRF解决
