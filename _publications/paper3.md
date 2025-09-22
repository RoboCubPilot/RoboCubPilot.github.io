---
permalink: /publications/paper3
collection: publications
category: manuscripts
title: "[Secure State Estimation of Cyber-Physical Systems via Gaussian Bernoulli Mixture Model](https://arxiv.org/pdf/2411.09956)"
author_profile: true
# date: 2009-10-01
# venue: 'Journal 1'
slidesurl: 'https://arxiv.org/pdf/2411.09956'
paperurl: 'https://arxiv.org/pdf/2411.09956'
citation: ''
---

这篇文章是我关于控制理论的结尾之作，自认为做的蛮不错的，在我博士阶段研究的控制问题上达到了sota。在这之后转做机器人了，但机器人交互问题的关键思路，都孕育在这篇文章中。

概述
======
文章研究了一个基本控制问题。当观测不完美可靠，应该直接用滤波，还是找到并且除去那些不可靠的观测。如果是后者（聪明的系统显然应该有判断力），该如何去推断哪些观测不可靠，又该如何利用不完美的观测来估计状态。文章的结论是：推理不可靠观测和估计最优状态这两个问题耦合在一起，观测信息既包含环境也包含系统状态，整个问题既连续又离散，求解过程既要解耦也要解码。

- - - - - - - - - - -

问题描述
======
<img src="/files/paper3/image.png" alt="Figure" width="640">

- - - - - - - - - - -

扰动表征 / 核心问题 / 算法
======
都直接看paper吧。

- - - - - - - - - - -

实验结果
======
  + 直接用贝叶斯估计推理出了不可靠的观测，而不是依赖傻乎乎的鲁邦估计
    <img src="/files/paper3/1.png" alt="Figure" width="640">
  + 在所有强度的扰动下，我们的算法 (GBS) 估计精度和推理正确性几乎都达到了sota
    <img src="/files/paper3/2.png" alt="Figure" width="640">  