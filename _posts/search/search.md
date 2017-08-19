# search
核心点:索引的构造、搜索查询、基础排序

通用搜索(非结构化 文档)、垂直搜索(结构化较多)

## 数据结构
倒排（原理)、正排、
(实现) 哈希表、跳跃表、B+数

## 索引构建     

- 全量索引 增量索引
- 内存构建索引
- 磁盘构建索引
- 索引加载技术，全内存加载，MMAP加载(搜索、推荐、广告系统或所有大数据的查询系统中较为广泛常见)
现在后端开发，一般遇到瓶颈都会用redis内存数据库来抗压抗并发。而还有一种方式就是使用MMAP的方式，它对内存的要求很小。

## 搜索查询
- 倒排查询
- 正排过滤(电商中非常重要)
- 交集、并集、bitmap、内存控制

## 完整实现
- 网络模型
- 索引构建模块
- 搜索查询模块
- 提供搜索服务
- golang网络模型

## 搜索相关性排序
- 中文分词（初步涉及）
- 搜索词的相关性排序(TF-IDF)
- 其他维度排序(点击，收藏，销量......)

## 分布式和搜索周边应用
分布式模型
相关搜索和搜索提示
query分析（通用->基于统计、垂直领域->结果集），自然语言处理
搜索和推荐，搜索和广告

数据库并不能够

