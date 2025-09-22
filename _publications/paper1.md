---
permalink: /publications/paper1
collection: publications
category: manuscripts
title: "Contact Estimation for Humanoid Robots via Diffusion Policy"
author_profile: true
# date: 2009-10-01
# venue: 'Journal 1'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
# paperurl: 'http://academicpages.github.io/files/paper1.pdf'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

还未挂到arxiv上，算法和文章还需一段时间才能开源。

- - - - - - - - - - -

概述
======
+ 在没有触觉和力学传感器的情况下，首次低成本地实现人形机器人表面交互过程中的接触估计。用强化学习增强算法在外力干扰下的鲁棒性，采集全身电机抖动等数据，利用流匹配推理接触点和冲量。

算法
======
+ 略

仿真实验
======
 + 在台阶静止站立状态，能感知任意躯干的接触
<img src="/files/paper1/figure1.gif" alt="Figure 3" width="640">

 + 在斜面静止站立状态，能感知任意躯干的接触
<img src="/files/paper1/figure2.gif" alt="Figure 3" width="640">

 + 在动态行走的过程中，能感知任意躯干的接触 (好像gif有点不清晰)
<img src="/files/paper1/figure3.gif" alt="Figure 3" width="640">

- - - - - - - - - - -

真机实验
======
 + 无需遥控，用任意肢体的接触唤醒机器人
<img src="/files/paper1/videos1.gif" alt="Figure 3" width="640">

 + 无需遥控，用任意肢体的接触给机器人发指令
   + 静止时，敲击任意关节，接触力的方向就是速度命令的方向
   + 运动中，朝运动的反向敲击任意关节，机器人停止运动
   + 静止时，连续两次敲击机器人，机器人向后转180度
<img src="/files/paper1/videos2.gif" alt="Figure 3" width="640">

 + 无需遥控，机器人感知任意肢体的碰撞实现主动安全
<img src="/files/paper1/videos3.gif" alt="Figure 3" width="640">