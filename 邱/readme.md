# 大模型推理


## 最近阅读

1. #### MathAttack: Attacking Large Language Models Towards Math Solving Ability 
出处：AAAI 2024

作者：西交利物浦大学

发布时间：2023年9月3日

原文：https://arxiv.org/pdf/2309.01686

简介：提出了一个用来生成问题文本对抗样本的方法。不是针对prompt，而是针对问题进行词替换的方法。然后用这个对抗样本生成办法生成了一个对抗样本数据集，并且这些对抗样本可以拿来作为prompt来提高模型鲁棒性。

博客：https://blog.csdn.net/weixin_74095289/article/details/139510694?csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22139510694%22%2C%22source%22%3A%22weixin_74095289%22%7D

2. #### BADCHAIN: BACKDOOR CHAIN-OF-THOUGHT PROMPTING FOR LARGE LANGUAGE MODELS
出处：	Accepted to ICLR2024

作者： Zhen Xiang, Fengqing Jiang, Zidi Xiong, Bhaskar Ramasubramanian, Radha Poovendran, Bo Li

发布时间：20 Jan 2024

原文： https://arxiv.org/abs/2401.12242

简介：在本文中，我们提出了BadChain，这是第一个使用COT提示的针对LLM的后门攻击，它不需要访问训练集或模型详细信息。我们展示了BadChain对两个COT策略和四个LLM在六个基准推理任务上的有效性，并对这种有效性提供了解释。此外，我们进行了广泛的消融研究，以说明BadChain的设计选择可以很容易地通过少量的实例来确定。最后，我们提出了两种后门防御方法，并证明了它们对BadChain的无效性。因此，BadChain仍然是LLMs的重要威胁，需要在未来开发更有效的防御方法。

博客：https://blog.csdn.net/weixin_74095289/article/details/139511980?spm=1001.2014.3001.5501


## 综述
### 大模型prompt
1. #### Reasoning with Language Model Prompting: A Survey
出处：	ACL 2023, 24 pages, add references of theoretical analysis

发布时间：Fri, 28 Jan 2022 

作者：Shuofei Qiao, Yixin Ou, Ningyu Zhang, Xiang Chen, Yunzhi Yao, Shumin Deng, Chuanqi Tan, Fei Huang, Huajun Chen

原文：https://arxiv.org/abs/2212.09597

简介：
关于大模型推理提示的一些技术,用分类法分的很清楚。主要分为策略增强推理和知识增强推理。本文全面综述了语言模型推理的前沿研究提示。我们通过比较和总结来介绍研究工作，并提供系统资源来帮助初学者。我们还讨论了出现这种推理能力的潜在原因，并强调了未来的研究方向

博客：https://blog.csdn.net/weixin_74095289/article/details/139243074?spm=1001.2014.3001.5502

2. #### Exploring the Reasoning Abilities of Multimodal Large Language Models (MLLMs): A Comprehensive Survey on Emerging Trends in Multimodal Reasoning
出处：Computation and Language (cs.CL); Artificial Intelligence (cs.AI)

时间：Wed, 10 Jan 2024

作者：Yiqi Wang, Wentao Chen, Xiaotian Han, Xudong Lin, Haiteng Zhao, Yongfei Liu, Bohan Zhai, Jianbo Yuan, Quanzeng You, Hongxia Yang

简介：具有抽象推理能力的强人工智能（Strong AI）或通用人工智能（AGI）是下一代人工智能的目标。大型语言模型 (LLM) 的最新进展以及新兴的多模态大型语言模型 (MLLM) 领域在各种多模态任务和应用程序中展示了令人印象深刻的功能。特别是，各种 MLLM 都具有不同的模型架构、训练数据和训练阶段，已在广泛的 MLLM 基准上进行了评估。这些研究在不同程度上揭示了 MLLM 当前能力的不同方面。然而，MLLM 的推理能力尚未得到系统研究。在本次调查中，我们全面回顾了现有的多模态推理评估协议，对 MLLM 的前沿进行了分类和说明，介绍了 MLLM 在推理密集型任务中应用的最新趋势，最后讨论了当前的实践和未来的方向。我们相信我们的调查为多模态推理这一重要主题奠定了坚实的基础并阐明了清楚了


博客：https://blog.csdn.net/weixin_74095289/article/details/139013490?spm=1001.2014.3001.5502

## 技术
### 对抗样本
1. #### MathAttack: Attacking Large Language Models Towards Math Solving Ability 
出处：AAAI 2024

作者：西交利物浦大学

发布时间：2023年9月3日

原文：https://arxiv.org/pdf/2309.01686

简介：提出了一个用来生成问题文本对抗样本的方法。不是针对prompt，而是针对问题进行词替换的方法。然后用这个对抗样本生成办法生成了一个对抗样本数据集，并且这些对抗样本可以拿来作为prompt来提高模型鲁棒性。

博客：https://blog.csdn.net/weixin_74095289/article/details/139510694?csdn_share_tail=%7B%22type%22%3A%22blog%22%2C%22rType%22%3A%22article%22%2C%22rId%22%3A%22139510694%22%2C%22source%22%3A%22weixin_74095289%22%7D

### 大模型推理能力增强
1. #### Chain-of-Thought Prompting Elicits Reasoning in Large Language Models
出处：proceedings.neurips.cc

作者：J Wei, X Wang, D Schuurmans, M Bosma, F Xia, E Chi, QV Le, D Zhou

发布时间：Fri, 28 Jan 2022 

简介：COT思维链技术

博客：https://blog.csdn.net/weixin_74095289/article/details/139247231?spm=1001.2014.3001.5502


#### Self-consistency Improves Chain Of Thought Reasoning in Language Models引用

COT的自我一致性（有点类似于ensemble）

2. #### Large Language Models are Versatile Decomposers: Decomposing Evidence and Questions for Table-based
出处：SIGIR 2023

作者：Yunhu Ye, Binyuan Hui, Min Yang, Binhua Li, Fei Huang, Yongbin Li

发布时间：Tue, 31 Jan 2023

原文： https://arxiv.org/abs/2301.13808
简介：

表格推理很重要：1、对于NLU（自然语言理解）和IR（信息检索）很重要 2、对于下游任务例如FV（基于表格的事实验证）和QA很重要

表格推理难：原因是包括了非结构化文本，半结构化表格

解决的历史过程：
1、综合执行语言和表进行交互，例如sql

不足：忽略了表格内文本块的语义

2、最近基于表格的预训练模型
不足：
1、这些模型需要对大量基于特定任务的下游数据集进行微调在处理具有未见过的推理类型的新数据集时难以获得出色的性能
2、破坏了模型的上下文能力

3、对于预训练模型，不进行微调而是上下文学习引起关注

现在LLM在文本推理上厉害，但是对表格推理还没怎么研究，但是LLM对表格推理有一下技术挑战：

1、大表格困难 原因：有很多行和列，难以直接对所有表内容进行编码，而且会有大量不相干信息。例如现在不能扩展到30行以上

2、 将复杂问题分解为更简单的子问题可以有效促进LLM的多步推理（Huang et al., 2022；Dua et al., 2022；Chen et al., 2022）。然而，利用思维链提示直接分解复杂问题（Wei et al., 2022）很容易陷入幻觉困境（Ji et al., 2022），模型可能会生成包含信息的误导性子问题(这些子问题和证据不符合)。

综上，作者提出要一个可靠的基于表格的复杂问题分解方法
所以作者提出
探索了上下文学习 来分解问题和表格的方法----DATER

博客： https://blog.csdn.net/weixin_74095289/article/details/139014779?spm=1001.2014.3001.5502


3. #### Large Language Models are Visual Reasoning Coordinators
出处：Part of Advances in Neural Information Processing Systems 36 (NeurIPS 2023) 

时间：2023

作者： Liangyu Chen, Bo Li, Sheng Shen, Jingkang Yang, Chunyuan Li, Kurt Keutzer, Trevor Darrell, Ziwei Liu

原文： https://proceedings.neurips.cc/paper_files/paper/2023/hash/ddfe6bae7b869e819f842753009b94ad-Abstract-Conference.html


简介：用一个LLM作为两个VLM之间的沟通桥梁，来提高大模型推理能力


博客：https://blog.csdn.net/weixin_74095289/article/details/139014353?spm=1001.2014.3001.5502








## 多模态






## 分析



## benchmark

### 自动化
1. #### Understanding Social Reasoning in Language Models with Language Models
出处：proceedings.neurips.cc


时间：2023

作者：Kanishk Gandhi, Jan-Philipp Fraenken, Tobias Gerstenberg, Noah Goodman

原文：https://proceedings.neurips.cc/paper_files/paper/2023/hash/2b9efb085d3829a2aadffab63ba206de-Abstract-Datasets_and_Benchmarks.html

简介：随着大型语言模型（LLM）越来越多地融入我们的日常生活，了解它们理解人类心理状态的能力对于确保有效的交互变得至关重要。然而，尽管最近尝试评估LLM的心智理论 (ToM) 推理能力，但这些模型与人类心智理论 (ToM) 的一致性程度仍然是一个微妙的探索话题。这主要是由于两个不同的挑战：（1）以前的评估结果不一致，（2）对现有评估方法有效性的担忧。为了应对这些挑战，我们提出了一个新颖的框架，通过填充因果模板来程序化地生成对LLM的评估。使用我们的框架，我们为LLM创建了一个新的社会推理基准 (BigToM)，其中包含 25 个对照和 5,000 个模型编写的评估。我们发现，人类参与者对我们基准的质量评价高于以前的众包评估，并且与专家撰写的评估相当。使用 BigToM，我们评估了各种LLM的社会推理能力，并将模型表现与人类表现进行比较。我们的结果表明，GPT4 具有反映人类推理模式的 ToM 功能，尽管不太可靠，而其他LLM则不太行

所以作者反复用few shot prompt提示去利用LLM的推理能力生成了一个关于TOM的数据集命名为bigTOM


博客：https://blog.csdn.net/weixin_74095289/article/details/139014683?spm=1001.2014.3001.5502