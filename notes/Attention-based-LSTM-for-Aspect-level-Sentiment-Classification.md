## Attention-based LSTM for Aspect-level Sentiment Classification
  今年的情感分析的层面相比于句子更进一步，深入到句子观点层面(例如:这家餐馆的服务很好,但是菜不怎么样. 涉及服务、食物两方面)

- key1
 - 模型主要是生成了[d,N]的Aspect embedding Matrix，其中d表示维度，N表示涉及的Aspect数目. 其中这个矩阵不是由word embedding构成的，而是训练得到的
 - 加入了Attention Model, 1 直接在句子和aspect进行权重计算 2 或者是将aspect加入word embedding 再进行attention计算
 - 训练数据量: 2000条对应一个aspect, 数据量较小, 但是依然能够训练出相对(稳定)的模型
