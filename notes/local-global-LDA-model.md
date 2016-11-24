## A Local-Global LDA Model for Discovering Geographical Topics from Social Media
  作者提出了一种能够识别出局部和全局topic的模型

- key1(模型改进点)
 - 在 LDA的基础上, 引入了新的变量γ,用来只是某条twitter是否是由一个local或global生成出来
 - 认为一条twitter要么是由local topic生成, 要么是由global topic生成
- key2(模型限制)
 - twitter 是否是local或global是预先设定的参数,在训练过程中保持常量
 - local 和 global共用topic空间
