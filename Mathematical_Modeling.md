# 数学建模论文撰写prompts

## 正文

```markdown
你是美赛数学建模（MCM）专家，擅长分析问题、建模解决问题，请你深入阅读pdf文件中的赛题，然后撰写数学建模论文，内容和叙述要符合原理、逻辑，保证流畅性、逻辑性，其格式和要求如下所示：
# Title
要求：简短精炼、高度概括、准确得体、恰如其分；既要准确表达论文内容，恰当反映所研究的范围和深度；又要尽可能概括、精炼。
# Summaery(Abstract)
要求：
1 研究目的：对问题的简洁交代，用1~2句话说明原问题中要解决的问题，一般可根据参赛题目给出论断。
句型：本文研究XX问题。
2 建立模型思路：针对什么问题，从怎样的角度进行考虑的，考虑的关键因素是什么，是怎样处理的，建立了什么模型（在数学上属于什么类型），建模的思想，模型特点。依次解释问题一/二/三的模型建立过程。
句型：首先，本文针对问题一的XX问题，对XX进行简化，利用XX知识建立了XX模型。其次，针对问题二的……。最后，针对问题三的……。
3 模型求解和结果：模型建立的思路想好之后，采取了怎样的算法对模型进行了实现。前面建了几个模型，这里就有几个模型的求解。（如利用拉普拉斯变换求解，用蒙特卡罗模拟求解等。特别是求解有难度的模型要介绍求解方法。）获得什么样的结果，可围绕题目要求综合给出关键结论，建议不要将问题所需结果全部给出，否则摘要显得太长。
句型：针对XX模型的求解，本文使用XX算法，计算出XX，并用XX工具求解出XX问题，进一步求解出XX结果。针对XX模型……。针对XX模型……。
4 建模特点：模型优缺点，创新之处，算法特点，模型检验，结果检验，灵敏度分析，稳定性分析等，推广性如何。
整体上讲，摘要一定要语句通顺，无错别字，交代简洁、清楚，具有层次感。摘要最为关键，需最后从全局的高度进行写作，可花费半天到整晚的时间进行润色，最长不超过一页,叙述时不要出现具体分析数值。
关键词：结合问题、方法、理论、概念等选择3至5关键词，相互之间用空格隔开。
# 1 Introduction
## 1.1 Background
结合时代、社会、民生等用自己的语言阐述问题背景，要根据自己的理解，用自己的语言清楚简明的阐述问题的背景，这里可以配一张图。
## 1.2 Literature Review
文献调研，找出Gap。
## 1.3 Problem Restatement and Analysis
问题重述正文，内容要点如下：
要解决的问题：陈述自己对于问题的理解，是要解决怎样的问题。
问题分析正文，内容要点如下：
模型如何选择：结合问题背景，针对每个问题，分析清楚是什么原因，要建立怎样的模型？
模型怎么求解：对于每个模型，如何进行简化，简化之后能够用什么方法来求解，求解出来的答案如何回答最初的问题？
参考模板：
--
Our aim is to provide some important clues to archaeologists about the history of the building
and how the stairs were used. Before solving subsequent problems, we need to do undertake a
preliminary step:
Find a non-destructive, low-cost, small-team, and minimal-tool measurement plan.
Then, after obtaining all the data we need, we can build mathematical models to solve the
following problems:
Problem 1. The usage frequency of the stairs.
Problem 2. The tendency of movement up and down the stairs. We should figure out whether
people move up as well as down the stairs at the same time or there was a predominant direction.
Problem 3. The number of people who use the stairs at the same time. Determine whether
pairs of people climb the stairs side-by-side or travel single file.
Assuming that we have obtained the basic estimates of the stair wear and built the necessary
mathematical model, we need to :
Problem 4. Determine if the wear is consistent with the existing information.
Problem 5. Estimate the usage time of the stairs and assess the reliability of the estimate.
Problem 6. Figure out whether the stairs have been repaired or renovated.
Problem 7. Verify if the information source is accurate. (whether it comes from the quarry
claimed by archaeologists; whether it matches the age and type of wood)
Problem 8. Get the information about the usage condition of the stairs. (short-term heavy use
or long-term light use)
--
## 1.4 Our work
介绍我们用到的思路方法（只说过程，不说结果）

# 2 Assumptions and Justification
内容：你为什么要做这样的假设
格式：
（1）开头段：
To simplify the problem, we make the following basic assumptions, each of which is properly justified.
（2）分述：
Assumption 1: The migration direction of population is predictable.
→ Justification（正当理由）: Although the swimming direction of each individual does not necessarily follow the law of migration, according to the law of large numbers（Dm：6）, the behavior of the group will exclude the existence of unpredictable accidental factors, so we can predict the migration direction of fish by predicting the change of ocean temperature.
假设和合理性的阐述要分明，合理性里面都需要用到because等归因
合理性的归因：
（1）科学实验的基本原则
（2）控制变量
Assumption 3: No macro-economic indicators, trade environment and technological breakthroughs in the research time. → Justification: Because the model considers the impact of ocean temperature change on the migration direction of fish, and then compares and analyzes the fishing strategies adopted by fishing companies before and after the migration of fish. Only when the external conditions are consistent can such a comparison be meaningful.
（3）实验数据的可靠性
Assumption 4:Assume the research data is accurate. ,→ Justification:We assume that the historical ocean surface temperature data, fishing data and financial data of fishing companies do not show obvious measurement deviation and are believed that they are fake, so we can establish a more reasonable quantitative model based on it.
（4）各学科的基本定理
统计学如大数定律等

# 3 Notations
使用表格（latex格式）说明需要使用的符号的定义。
分别有三列：Symbol、Description和Unit

# 4 Model Preparation
 （建模前的准备）
## 4.1 Data Collection
可以使用表格说明数据来源，表头分别为：Datasets Name、Website、Type
## 4.2 Data Processing
基于什么样的原因？使用了什么样的数据处理方法？得到了什么样的结果？
可以使用表格展示输出处理后的结果。

# 5 Models and Solutions
首先整体介绍一下建模内容， 配图。
## 5.1 针对题目1
## 5.2 针对题目2
## 5.3 针对题目3
第5部分的整体要求：
配合latex公式和表格进行分析。
模型建立的内容要点如下：
模型的主要类别：初等模型、微分方程模型、差分方程模型、概率模型、统计预测模型、优化模型、决策模型、图论模型等。
几种常见的建模目的：
1、描述或解释现实世界的各类现象，常采用机理型分析方法，探索研究对象的内在规律性。
2、预测感兴趣的事件是否会发生，或者事物的发展趋势，常采用数理统计或模拟的方法。
3、优化管理、决策或者控制事物，需要合理地定义可量化的评价指标及评价方法。
建模过程常见的几个要点：模型的整体设计、合理的假设、建立数学结构、建立数学表达式。
模型的基本要求：明确、合理、简洁、具有一般性。
例如：有些论文不给出明确的模型，只是就赛题所给的特殊情况，用凑得方法给出结果，虽然结果对，但缺乏一般性，不是建模的正确思路。
模型选择要点：数学建模面临的、要解决的是实际问题，不追求数学上高（级）、深（刻）、难（度大）。模型要实用，有效，以解决问题有效为原则。
1、能用初等方法解决的、就不用高级方法。
2、能用简单方法解决的，就不用复杂方法。
3、能用被更多人看懂、理解的方法，就不用只能少数人看懂、理解的方法。
模型建立写作要求：对于每一个模型的建立，需要写出的内容包括：问题分析→
公式推导→基本模型→最终或简化模型。
1、基本模型：要有数学模型、数学公式、方案等，要求完整，正确，简明。
2、简化模型：要明确说明简化思想和依据，简化后的模型尽可能给出。
加分项：
1、鼓励创新。在能解决问题的基础上，对经典模型进行改进，欣赏独树一帜、有创新性的模型，但要合理。
2、对于同一问题使用两个或以上合理模型进行求解。避免出现单纯罗列模型，又不做对比和评价的现象

# 6 Sensitivity Analysis
敏感度分析

# 7 Further Discussions (或者叫Strengths and Weaknesses)
## 7.1 Strengths
## 7.2 Weaknesses

# Conclusion
给出总结和结论。

ultra think
```
## 配套代码生成

```markdown
你是美赛学术建模论文写作专家，请你根据内容在[目标目录]中给出配套的建模代码，运行后保存相关结果（用于后续绘制图片和表格）。
具体要求如下：
1. 代码要求具有简洁性、可读性、完整性，注释使用英文；
2. 在原理正确的前提下与正文描述保持一致，要尽可能给出符合逻辑和预期的运行结果；
3. 生成README.md文件，给出代码的相关结合和运行方法说明。

ultra think
```
