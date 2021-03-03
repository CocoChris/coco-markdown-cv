---
layout: cv
title: Wode "Nimo" Ni
email:
  url: mailto:woden@cs.cmu.edu
  text: woden@cs.cmu.edu
homepage:
  url: http://cs.cmu.edu/~woden
  text: cs.cmu.edu/~woden
phone:
  '18217195632'
---

# Wode **Ni**

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

### **宾夕法尼亚州立大学&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;统计系 - 机器学习方向** `2020.6 -`

研究实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;研究方向是机器学习算法在基因组学中的应用<br>

### **爱奇艺（上海）&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;智能平台部 - 大数据服务组** `2018.5 - 2020.5`

算法工程师&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责各项大数据服务系统的开发工作，建设一体化、实时化的运维数仓，开发DataOps大数据资源审计平台，并将机器学习算法应用于项目开发中，建立一套集成智能报警、智能诊断、聊天机器人的AIOPS智能运维系统<br>

### **百度（北京）&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;推荐技术平台部** `2017.12 - 2018.4`

研发实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责手机百度的feed流推荐策略和模型研究，开发推荐系统的指标监控和数据分析模块<br>

### **天风证券&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;信息技术部** `2017.6 - 2017.11`

研发实习生&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;主要负责证券交易流水的数据分析系统的设计与开发<br>

## 项目经历
### **运维数仓与大数据资源审计平台的设计与开发** `爱奇艺 (2019 - 2020)`
- 搭建一体化、灵活可配置的大数据资源审计平台，实现对存储资源、计算资源、服务指标等多数据源的数据采集引擎，打通离线与实时链路，建立多层血缘结构的运维数仓，对外提供实时查询、报警配置、数据分析、资源与任务优化建议等多项服务，大大提高运维同学的工作效率，节省资源采购成本<br>
  - zheshiyigexiaoceshine
- 传统的数据采集会对集群造成压力，为了解决这一难点，我设计了先同步再采集的方案，并且保证每次同步只在standby的namenode上进行，大大减轻了集群的压力，同时，还设计了通过对比远端和本地的文件大小来判断日志是否发生回滚的机制，保证了数据的准确性<br>
- 实时链路开发过程中有两个主要难点，一个是如何尽量做到实时，减少延迟，对此我将存储资源数据以目录树的形式存储在内存中，加快了数据的更新和读取，使数据延时控制在5分钟以内；第二点，如何尽量节省目录树所占的存储空间，对此我优化了目录树模型，将路径名进行十六进制编码后存储，使占用内存从100+G节省到40G左右<br>
- 运维数仓的搭建初期，由于数仓结构过于扁平化，无法进行复杂指标的关联分析，为了解决这一难点，我设计了多层的数仓结构，通过对元数据层的数据进行关联、拆分，生成满足不同需求的中间层，并记录层与层、表与表之间的血缘关系，方便了数据的追踪，也方便了运维同学自定义指标进行查询<br>
- Java/Scala/Shell/Spark/Hive/HBase/ActiveMQ/Kafka/Flink/Springboot/Vue/JavaScript/MySQL/Redis<br>
### **AIOPS智能报警与故障诊断系统的设计与开发** `爱奇艺 (2019)`
### **Chatbot智能运维机器人的设计与开发** `爱奇艺 (2018)`
### **机器学习在基因组学中的应用** `宾夕法尼亚州立大学 (2020 - 2021)`
## Honors & Awards

CHI'20 Best Paper Honourable Mention Award `CMU, 2020` <br>
Phi Beta Kappa `Dickinson, 2018` <br>
Excellence in Computer Science Award `Columbia, 2018` <br>
Travel Award PL Mentoring Workshop (PLMW) `SPLASH, 2018` <br>
Tau Beta Pi, Engineering Honor Society `Columbia, 2017` <br>
Computer Science Departmental Honors `Dickinson, 2016` <br>
Pi Mu Epsilon, Mathematics Honor Society `Dickinson, 2016` <br>
Upsilon Pi Epsilon, Computer Science Honor Society `Dickinson, 2016` <br>
Alpha Lambda Delta, First year Honor Society `Dickinson, 2013`<br>
John Montgomery Scholarship `Dickinson, 2013` <br>

---

## Teaching

Teaching Assistant, **Programming Languages and Translators (COMS 4115)** `Columbia, 2017 - 2018` <br>
Teaching Assistant, **Introduction to Java II (COMP 132)** `Dickinson, 2016` <br>
Peer Tutor, **Data Structures and Problem Solving (COMP 232)** `Dickinson, 2016` <br>
Computer Lab Consultant `Dickinson, 2014 - 2016` <br>


## Service

Reviewer `CHI 2021`
Research Experiences for Undergraduates in Software Engineering Admission Committee `CMU, 2019 - 2020`

## Publications

### [**Penrose: From Mathematical Notation to Beautiful Diagrams**](http://penrose.ink/media/Penrose_SIGGRAPH2020.pdf)
Katherine Ye, **Wode Ni**, Max Krieger, Dor Ma'ayan, Joshua Sunshine, Jonathan Aldrich, and Keenan Crane.<br> 
_ACM Transactions on Graphics (SIGGRAPH'20)._<br>
[[PDF](http://penrose.ink/media/Penrose_SIGGRAPH2020.pdf)]
[[BibTeX]({{ page.homepage.url }}/assets/siggraph20-penrose.txt)]
[[www](http://penrose.ink/siggraph20.html)]
[[repo](https://github.com/penrose/penrose)]

### [**How Domain Experts Create Conceptual Diagrams and Implications for Tool Design**]({{ page.homepage.url }}/assets/chi-20-natural-diagramming.pdf)

Dor Ma'ayan\*, **Wode Ni\***, Katherine Ye, Chinmay Kulkarni, and Joshua Sunshine.<br>
<i class="fas fa-award"></i> <strong>Best Paper Honourable Mention</strong><br>
_In Proceedings of the 2020 CHI Conference on Human Factors in Computing Systems (CHI'20)._<br>
[[PDF]({{ page.homepage.url }}/assets/chi-20-natural-diagramming.pdf)]
[[BibTeX]({{ page.homepage.url }}/assets/chi-20-natural-diagramming.txt)]

### [**Defining Visual Narratives for Mathematics Declaratively**](http://plateau-workshop.org/assets/papers-2019/9.pdf)

Max Krieger, **Wode Ni**, and Joshua Sunshine.<br>
_Evaluation and Usability of Programming Languages and Tools (PLATEAU 2019), co-located with UIST._<br>
[[PDF](http://plateau-workshop.org/assets/papers-2019/9.pdf)]
[[slides]({ page.homepage.url }}/aassets/plateau-19-presentation.pdf)]

### [**Designing Declarative Language Tutorials: a Guided and Individualized Approach**](http://plateau-workshop.org/assets/papers-2019/2.pdf)

Anael Kuperwajs Cohen, **Wode Ni**, and Joshua Sunshine.<br>
_Evaluation and Usability of Programming Languages and Tools (PLATEAU 2019), co-located with UIST._<br>
[[PDF](http://plateau-workshop.org/assets/papers-2019/2.pdf)]
[[slides]({{ page.homepage.url }}/assets/plateau-19-presentation.pdf)]

### [**Substance and Style: domain-specific languages for mathematical diagrams**](https://2017.splashcon.org/event/dsldi-2017-substance-and-style-domain-specific-languages-for-mathematical-diagrams)

**Wode Ni\***, Katherine Ye\*, Joshua Sunshine, Jonathan Aldrich, and Keenan Crane.<br> _Domain-Specific Language Design and Implementation (DSLDI 2017), co-located with SPLASH._ <br>
[[PDF]({{ page.homepage.url }}/assets/dsldi.pdf)]
[[slides]({{ page.homepage.url }}/assets/dsldi-presentation.pdf)]
[[www](http://penrose.ink)]
[[repo](https://github.com/penrose/penrose)]

---

### [**Whiteboard Scanning Using Super-Resolution**](http://scholar.dickinson.edu/student_honors/221/)

**Wode Ni**.<br> _Dickinson College Honors Theses. Paper 221._<br>
[[PDF]({{ page.homepage.url }}/assets/superres.pdf)]

<!-- ### Footer

Last updated: May 2013 -->
