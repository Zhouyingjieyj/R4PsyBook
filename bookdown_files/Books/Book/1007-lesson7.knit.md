---
editor_options: 
  markdown: 
    wrap: 72
---

# 第七讲：如何进行基本的数据分析: t-test和anova{#lesson-7}



## **语法实现**

### t检验
#### 理论基础
我们来讲讲t检验。最简单的是单样本t检验，它是一个样本的一系列数据，将其平均值与一个固定值进行比较。我们有两个假设，H0和H1，假设显著水平为0.05。NHST的逻辑是，首先假设H0为真，然后从H0统计模型中提取当前数据，计算概率。如果概率很低，我们认为它不太可能发生，拒绝假设H0。p值与假设水平进行比较时，我们假设H0为真。我们有三个选择，等于、大于或小于。如果不等于，那么是双样本检验，如果小于或大于，则为单样本检验。绍的是这些检验的不同类型。首先是单样本检验，当p值小于等于mu时，H0大于等于mu。另一种单样本检验是当H0大于等于mu时。

接下来是双样本检验，假设两个样本来自同一个集合。我们可以用p值或t值检验来比较两个样本之间的差异。如果数据是高度相关的，我们可以使用相关数据的t值检验。独立样本t值检验也是双样本检验，它是两对无相关的数据。我们可以使用R语言的函数来进行这些检验。有各种R语言函数可以用于t检验，这些函数包括在R-base基础包中。我们将会介绍Bruce R包，它是为心理学优化设计的，使用它更方便。
我们载入所需的包。BruceR包载入后会有一大串提示信息，包括载入的包、主要函数和网址等。我们使用相对路径读取之前的数据，可以查看前5行。
####解决问题




























