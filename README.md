# Architecture
 是项目整个架构的文档仓库，用于整合现有的所有技术、规划现有项目。

## 项目概况

目前技术的整合接近尾声，我们将在这一步之上开始整合。

### 项目划分

#### Fantasy Studio

【代号】Studio，是所有技术的整合,我们会把所有实验得到的改进都加入FantasyStudio，并且FantasyStudio将会享受到所有研究产出。

#### Morisa

【代号】Morisa，用于提供项目中所有使用到的模型和算法

#### UI

用于为所有项目提供界面和视图架构支持。



# 研究项目

## 1.结构化与非结构化数据在文字创作的应用

这个项目用于研究以下内容：

1. 如何在非结构化的文本内容中提取结构化数据
2. 如何利用结构化数据帮助我们创作文字创作

### 项目背景

我们希望在创作文学作品中，能够获得创作智能。帮助我们快速编写一个文字创作的作品。

### 项目进度概况

首先我们遇到的最大的难点是，我们并没有精力和时间，完全将深度学习和机器学习应用到结构化和非结构化数据的提取任务当中，其次我们需要考虑的是，面对参差不齐的机器配置，我们如何将算法落地。这两项难题一直困扰我们许久，因为缺少时间、经济、精力、技术，我们很难让深度学习帮助我们将这个想法落地。所以我们只能另辟蹊径！现在最核心的突破点就是利用创作的三种状态（概念态、设计态、最终态）来提取结构化数据，并利用结构化数据指导我们的创作。

### 项目的答疑

#### 为什么我们非要折腾结构化数据的提取？

这其实是我们一直在坚持的一个核心技术，叫做创作智能，我们希望我们在创作的过程中，能够不断的收获到创作的启发。但是创作智能这个技术，现在是没有落地的技术和产品来给我们做参考的，都是摸着石头过河前进。我们在有限的人力物力财力目前顺利的推进到了第一阶段，也就是弱创作智能。这是非常有限的智能，我们依赖用户的反馈，用户的数据，全部由用户编写的内容来生成有限的内容。虽然能做到的事情非常有限，但是推动了我整个创作智能项目计划的前进。

#### 什么是创作智能？

谁不想在自己写东西的时候，碰到什么难题就有人帮助我们解决？灵感枯竭的时候，给我们一个想法？不知道自己的人设长什么样子的时候，给自己一个概念图？这就是创作智能，这种创作智能，我目前只在以下几处地方看到过预览的实现：

1. Visual Studio 根据深度学习实现的IntelliCode，能够总结用户当前的行为，对将来要做的行为进行预测
2. PowerPoint 根据页面形状自动推荐布局的设计灵感