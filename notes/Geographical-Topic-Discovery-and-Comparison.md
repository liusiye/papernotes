## Geographical topic discovery and comparison
  较为早的一篇关于geographical topic的文章,整篇文章难度较高，文章中主要抓住两个问题：geographical topic [analyze] and [compare]

- key1(location-driven model)
 - 该模型首先对文档按照地点进行聚类，聚类方法采用GMM(高斯混合模型),这个对于任何一个具体location而言，可以计算出相应其属于某个地区的概率
 - 接着每个地区对应于一个topic，再由topic生成文档
- key2(text-driven model)
 - 该模型是直接对某个既有模型(NetPLSA)的使用，在计算Loss的过程中，引入regularization项，该项含义是计算相邻位置的文档的主题相似性
- key3(LGTA model)
 - 该模型认为文档的生成方式首先是:确定地区r~R, 这反映了不同地区文档数目的不同
 - 在确定地区后，每个地区存在不同的主题分布，确定主题
 - 接着确定下主题中的字
- key4(summary)
 - key1和key3都能够反推出地点的主题分布，因此能够进行比较(这里的地点与区域是有区别的)。但文章中对于key2的解释难以认同
 - 总的来说文章整体思想和2016年那篇文章的思路基本相同，但同时也说明了单纯topic model的能力可能会比较有限，需要考察neural network等方法进行的改造，
 同时需要了解下基本的EM算法思路
