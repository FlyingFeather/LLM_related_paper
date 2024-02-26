# Text2SQL

## Datasets
### source datasets-EN
- WikiSQL [[paper](https://arxiv.org/pdf/1709.00103.pdf)] [[code](https://github.com/salesforce/WikiSQL)] [[dataset](https://github.com/salesforce/WikiSQL)]
一个大型的语义解析数据集，由80,654个自然语句表述和24,241张表格的sql标注构成。WikiSQL中每一个问句的查询范围仅限于同一张表，不包含排序、分组、子查询等复杂操作。
- Spider [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider)] [[dataset](https://yale-lily.github.io/spider)]
- SParC [[paper](https://arxiv.org/pdf/1906.02285.pdf)] [[code](https://github.com/taoyds/sparc)] [[dataset](https://drive.google.com/uc?export=download&id=1Uu7NMHTR1tdQw1t7bAuM7OPU4LElVKfg)]
- CSpider [[paper](https://arxiv.org/pdf/1909.13293.pdf)] [[code](https://github.com/taolusi/chisp)] [[dataset](https://drive.google.com/drive/folders/1TxCUq1ydPuBdDdHF3MkHT-8zixluQuLa?usp=sharing)]
- CoSQL [[paper](https://arxiv.org/pdf/1909.05378.pdf)] [[code](https://yale-lily.github.io/cosql)] [[dataset](https://yale-lily.github.io/cosql)]
是一个用于构建跨域对话文本到sql系统的语料库。它是Spider和SParC任务的对话版本。CoSQL由30k+回合和10k+带注释的SQL查询组成，这些查询来自Wizard-of-Oz的3k个对话集合，查询了跨越138个领域的200个复杂数据库。每个对话都模拟了一个真实的DB查询场景，其中一个工作人员作为用户探索数据库，一个SQL专家使用SQL检索答案，澄清模棱两可的问题，或者以其他方式通知。

- DuSQL [[paper](https://aclanthology.org/2020.emnlp-main.562.pdf)] [[dataset](https://www.luge.ai/#/luge/dataDetail?id=13)]
- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase)] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
一个跨领域多轮交互text2sql中文数据集，包含5459个多轮问题组成的列表，一共17940个<query, SQL>二元组，涉及280个不同领域的数据库。

- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)] [[dataset](https://bird-bench.github.io/)]
数据集是一个英文的大规模跨领域文本到SQL基准测试，特别关注大型数据库内容。该数据集包含12,751对文本到SQL数据对和95个数据库，总大小为33.4GB，跨越37个职业领域。BIRD-SQL数据集通过探索三个额外的挑战，即处理大规模和混乱的数据库值、外部知识推理和优化SQL执行效率，缩小了文本到SQL研究与实际应用之间的差距。

### source datasets-CN
- [DuSQL-中文多表SQL解析数据集](https://www.luge.ai/#/luge/dataDetail?id=13)
DuSQL是一个面向实际应用的数据集，包含200个数据库，覆盖了164个领域，问题覆盖了匹配、计算、推理等实际应用中常见形式。该数据集更贴近真实应用场景，要求模型领域无关、问题无关，且具备计算推理等能力。Text-to-SQL任务的输入为数据库D和自然语言问题Q，输出为对应的SQL查询语句Y。在DuSQL数据集中，每一条样本是由数据库D、自然语言问题Q、SQL查询语句Y构成的一个三元组 (D, Q, Y )，其中，数据库由若干张表格构成，表格之间通过外键连接。


- [NL2SQL-中文单表SQL解析数据集](https://www.luge.ai/#/luge/dataDetail?id=12)
NL2SQL是一个多领域的简单数据集，其主要包含匹配类型问题。该数据集主要验证模型的泛化能力，其要求模型具有较强的领域泛化能力、问题泛化能力。


- [Cspider-中英文多表SQL解析数据集](https://www.luge.ai/#/luge/dataDetail?id=11)
CSpider是一个多语言数据集，其问题以中文表达，数据库以英文存储，这种双语模式在实际应用中也非常常见，尤其是数据库引擎对中文支持不好的情况下。该数据集要求模型领域无关、问题无关，且能够实现多语言匹配。

- 百度整理的数据
https://www.modb.pro/db/495086
https://zhuanlan.zhihu.com/p/349797233

### preprocess datasest
- sql-create-context [[dataset](https://huggingface.co/datasets/b-mc2/sql-create-context)]
This dataset builds from WikiSQL and Spider.

- NSText2SQL [[dataset](https://huggingface.co/datasets/NumbersStation/NSText2SQL)]

## 比赛
- [千言数据集：语义解析](https://aistudio.baidu.com/competition/detail/47/0/leaderboard)


## Papers

### Survey

### in-context learning methods
- (DAIL-SQL) Text-to-SQL Empowered by Large Language Models: A Benchmark Evaluation
- (2023-nips-DIN-SQL) DIN-SQL: Decomposed In-Context Learning of Text-to-SQL with Self-Correction
- C3: Zero-shot Text-to-SQL with ChatGPT


### LLM-based models
- 


### traditional models
