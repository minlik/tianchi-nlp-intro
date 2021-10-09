## Coggle 30 Days of ML（21年10月）

[文档地址](https://shimowendang.com/docs/XkpH6d8pHRgCtgV8/read)

| 任务名称                                        | 难度 | 所需技能             |
| ----------------------------------------------- | ---- | -------------------- |
| 报名比赛，下载比赛数据集并完成读取              | 低   | Pandas               |
| 对数据集字符进行可视化，统计标签和字符分布      | 中   | Pandas               |
| 使用 TFIDF 提取文本特征                         | 中   | Sklearn              |
| 使用 TFIDF 特征 和 线性模型完成训练和预测       | 中   | Sklearn              |
| 使用 TFIDF 特征 和 XGBoost 完成训练和预测       | 中   | Sklearn、XGBoost     |
| 学会训练 FastText、Word2Vec 词向量              | 中   | FastText、gensim     |
| 使用 Word2Vec 词向量，搭建 TextCNN 模型训练预测 | 高   | Pytorch              |
| 使用 Word2Vec 词向量，搭建 BILSTM 模型训练预测  | 高   | Pytorch              |
| 学会 Bert 基础，transformer 库基础使用          | 中   | Pytorch、transformer |
| 使用 Bert 在比赛数据集中完成预训练              | 高   | Pytorch、transformer |
| 使用 Bert 在比赛数据集上完成微调                | 高   | Pytorch、transformer |

**（10月5日）任务1：报名比赛，下载比赛数据集并完成读取**

- [x] 登录天池，可使用淘宝 & 支付宝登录，https://account.aliyun.com/login/login.htm

- [x] 下载比赛数据集，https://tianchi.aliyun.com/competition/entrance/531810/introduction

- [x] 读取比赛数据集，读取代码参考如下:

```python
import pandas as pd
train_df = pd.read_csv('train_set.csv', sep='\t', nrows=100)
train_df['word'] = train_df['text'].apply(lambda x: len(x.split(' ')))
```

**（10月5日）任务2：对数据集字符进行可视化，统计标签和字符分布**

- [x] 统计数据集中所有句子所包含字符的平均个数

- [x] 统计数据集中不同类别下句子平均字符的个数

- [x] 统计数据集中类别分布的规律

- [x] 统计数据集中不同类别下句子中最常见的5个字符

**（10月11日）任务3：使用 TFIDF 提取文本特征**

- [x] 学习 TFIDF 的原理

- [x] 学会使用 CountVectorizer

- [x] 学会使用 TfidfVectorizer

**（10月11日）任务4：使用 TFIDF 特征 和 线性模型完成训练和预测**

- [x] 使用 TFIDF 提取训练集和测试集特征

- [x] 使用线性模型（LR 等）完成模型的训练和预测

**（10月11日）任务5：使用 TFIDF 特征 和 XGBoost 完成训练和预测**

- [x] 使用 TFIDF 提取训练集和测试集特征

- [x] 使用 XGBoost 完成模型的训练和预测
