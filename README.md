# 任务

工作初步确定为和文档相似度有关，应用层面的主要目的是文本去重。现在我们的金融语料中有很多内容相同描述不一样的文档，希望能找出来。初步的计划是先利用聚类算法初筛，再输入LSH（局部敏感哈希）。并且可以借助于word mover's distance、ESIM短文本匹配等方法。



## 文本相似度

### 1.TF-IDF+LSI

<https://www.jianshu.com/p/edf666d3995f>

#### 步骤：

1. jieba分词、stop-word
2. 词袋模型向量化文本
3. TF-IDF模型向量化文本（更好地反应文本内容）
4. LSI模型向量化文本（将文本向量降维到主题数量）
5. 计算相似度



### 2. WMD词移距离

<https://zhuanlan.zhihu.com/p/74899813>



## 文本聚类

<img src = "/Users/Lin/Desktop/intern2020/cluster_procudure.png" style="zoom:50%">

使用tf-idf或word2vec作为文本的特征，采用k-means或者DBSCAN进行聚类分析



### Text clustering and LDA

<https://towardsdatascience.com/a-friendly-introduction-to-text-clustering-fa996bcefd04>



## LSH

### LSH Intro

<https://www.cnblogs.com/fengfenggirl/p/lsh.html>

### More About LSH

<https://towardsdatascience.com/understanding-locality-sensitive-hashing-49f6d1f6134>

<https://www.cnblogs.com/wt869054461/p/8148940.html>

### Minhash, Simhash,Klongsent

<https://zhuanlan.zhihu.com/p/43640234>



