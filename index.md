---
layout: cv
title: Xingxin Liu
email:
  url: mailto:191384643@qq.com
  text: 191384643@qq.com
homepage:
  url: https://github.com/CocoChris
  text: https://github.com/CocoChris
phone:
  '182-1719-5632'
username:
  text: '刘星鑫'
age:
  '28'
wechat:
  'sznznted'
---

<!-- # Xingxin **Liu** -->

<!--
include contact information from the front matter
Supported arguments:
    - homepage: url, text
    - phone
    - email
-->

{% include cv-contact.html %}

## 教育背景

### **上海交通大学&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;硕士&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;图像处理专业&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;GPA：3.7/4.3（20%）** `2015.9 - 2018.3`

### **上海交通大学&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;本科&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;电气工程专业&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;GPA：2.81/3.3（5%）** `2011.9 - 2015.6`

## 工作经历

### [**宾夕法尼亚州立大学&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;统计系 - 机器学习方向**]() `2020.6 -`

研究实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;研究方向是机器学习算法在基因组学中的应用<br>

### [**爱奇艺（上海）&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;智能平台部 - 大数据服务组**]() `2018.5 - 2020.5`

算法工程师&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责各项大数据服务系统的开发工作，建设一体化、实时化的运维数仓，开发DataOps大数据资源审计平台，并将机器学习算法应用于项目开发中，建立一套集成智能报警、智能诊断、聊天机器人的AIOPS智能运维系统<br>

### [**百度（北京）&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;推荐技术平台部**]() `2017.12 - 2018.4`

研发实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责手机百度的feed流推荐策略和模型研究，开发推荐系统的指标监控和数据分析模块<br>

### [**天风证券&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;信息技术部**]() `2017.6 - 2017.11`

研发实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责证券交易流水的数据分析系统的设计与开发<br>

## 专业技能

熟练掌握Java / Python / R / C++等编程语言，熟练掌握Springboot项目开发<br>
熟悉Hadoop生态系统，熟悉Spark编程，熟悉MySQL / Redis等数据库，熟悉Linux操作<br>
熟悉机器学习、NLP、图像处理算法<br>
了解前端开发，掌握Vue / JavaScript / HTML编程<br>

## 项目经历

### [**运维数仓与大数据资源审计平台的设计与开发**]() `爱奇艺 (2019 - 2020)`

- 搭建一体化、灵活可配置的大数据资源审计平台，实现对存储资源、计算资源、服务指标等多数据源的数据采集引擎，打通离线与实时链路，建立多层血缘结构的运维数仓，对外提供实时查询、报警配置、数据分析、资源与任务优化建议等多项服务，大大提高运维同学的工作效率，节省资源采购成本<br>
- 传统的数据采集会对集群造成压力，为了解决这一难点，我设计了先同步再采集的方案，并且保证每次同步只在standby的namenode上进行，大大减轻了集群的压力，同时，还设计了通过对比远端和本地的文件大小来判断日志是否发生回滚的机制，保证了数据的准确性<br>
- 实时链路开发过程中有两个主要难点，一个是如何尽量做到实时，减少延迟，对此我将存储资源数据以目录树的形式存储在内存中，加快了数据的更新和读取，使数据延时控制在5分钟以内；第二点，如何尽量节省目录树所占的存储空间，对此我优化了目录树模型，将路径名进行十六进制编码后存储，使占用内存从100+G节省到40G左右<br>
- 运维数仓的搭建初期，由于数仓结构过于扁平化，无法进行复杂指标的关联分析，为了解决这一难点，我设计了多层的数仓结构，通过对元数据层的数据进行关联、拆分，生成满足不同需求的中间层，并记录层与层、表与表之间的血缘关系，方便了数据的追踪，也方便了运维同学自定义指标进行查询<br>
- Java&ensp;/&ensp;Scala&ensp;/&ensp;Shell&ensp;/&ensp;Spark&ensp;/&ensp;Hive&ensp;/&ensp;HBase&ensp;/&ensp;ActiveMQ&ensp;/&ensp;Kafka&ensp;/&ensp;Flink&ensp;/&ensp;Springboot&ensp;/&ensp;Vue&ensp;/&ensp;JavaScript&ensp;/&ensp;MySQL&ensp;/&ensp;Redis<br>

### [**AIOPS智能报警与故障诊断系统的设计与开发**]() `爱奇艺 (2019)`
- 将各服务的海量报警经过故障自愈、报警聚合等模块后聚合成有效报警，并提供故障诊断、报警可视化统计等功能，大大减少报警数量，提高运维同学的工作效率<br>
- 为了方便服务的接入，实现了可插拔式的报警规则的灵活化配置，便于规则的修改、增删，系统陆续接入了Hadoop/中间件/数据库等服务，并将报警数量减少了97%以上<br>
- 针对故障原因复杂、难定位的难点，设计了基于混合决策数模型的故障诊断模块，相比于传统的逐项排查的方式，大大缩短了故障定位所需的时间<br>
- Java&ensp;/&ensp;Springboot&ensp;/&ensp;ActiveMQ&ensp;/&ensp;MySQL&ensp;/&ensp;Redis<br>

### [**Chatbot智能运维机器人的设计与开发**]() `爱奇艺 (2018)`
- 开发线上聊天机器人，提供各项云服务的QA、提交工单、查询监控等功能<br>
- 项目初期使用Baidu-Unit作为意图识别引擎，但识别效果受限于语料库，针对落地场景的特殊性，设计了基于意图打分的识别模型，通过爬虫爬取训练数据，基于用户反馈对模型进行学习，提高了识别的准确率<br>
- 基于SimHash算法进行文本去重，基于word2vec算法进行文本识别<br>
- Java&ensp;/&ensp;Python&ensp;/&ensp;C++&ensp;/&ensp;Springboot&ensp;/&ensp;MySQL&ensp;/&ensp;NLP<br>

### [**机器学习在基因组学中的应用**]() `宾夕法尼亚州立大学 (2020 - 2021)`
- 将机器学习算法应用于基因数据融合，进行样本分类、特征预测等<br>
- 采用CCA（canonical correlation analysis）算法进行数据降维，消除batch effect<br>
- 采用OT（optimal transport）算法进行最优分类<br>
- 采用MNN（mutual nearest neighbors）算法进行数据融合<br>
- R&ensp;/&ensp;Python&ensp;/&ensp;Matlab<br>

## 获奖经历

上海交通大学A等奖学金 `2016.9` <br>
上海交通大学优秀毕业生 `2015.6` <br>
上海交通大学C等奖学金 `2012.9` <br>

## 论文专利

### [**CT-ultrasound registration for electromagnetic navigation of cardiac intervention**](https://ieeexplore.ieee.org/abstract/document/8302189) `CISP-BMEI (IEEE 2018)`
### [**Surgical navigation simulation method based on electromagnetic positioning technology and intraoperative image guidance**]() `CN108420529A (2018)`

<!-- ### Footer

Last updated: May 2013 -->
