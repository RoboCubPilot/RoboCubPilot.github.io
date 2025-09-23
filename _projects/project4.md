---
permalink: /projects/project4
collection: projects
title: "宇树G1机器人 (130cm, 35kg) 不同地形站立平衡策略"
author_profile: true
---

- - - - - - - - - - -

目标
======
我们希望让机器人能够和人类一起玩“一二三木头人”的游戏。这不仅要求机器人能在任意地形上行走，还要能够在任意时刻切换到完全静止状态。不同于传统只需维持一种标准站姿的站立策略，本任务要求机器人具备在任意初始姿态下，都能稳定维持多样化站姿的能力。

- - - - - - - - - - -

挑战
======
+ **姿态多样性**：机器人不能依赖单一的“最佳站立姿态”，而是需要在复杂地形、不同身体关节状态下保持稳定。这显著增加了控制策略的复杂度。

+ **快速状态切换**：在游戏规则中，机器人必须能够从动态运动瞬间过渡到完全静止状态，要求控制器在毫秒级别内抑制动量、吸收冲击，并避免发生不稳定摆动。

+ **地形适应性**：不同地形（斜坡、台阶、软硬不均的地面）都会改变接触条件，机器人必须实时调整接触力分布与关节力矩，保证在任意支撑面上都能“冻结”姿态。

- - - - - - - - - - -

训练初始化
======
生成任意的机器人`base height`和机器人的双脚落脚点。根据这俩，用[dart](https://dartsim.github.io/dart/v6.11.1/index.html)反解相应的下肢关节IK，并且生成相应的地形，使得脚贴合在地形上，作为初始状态。

| 平地 | 台阶 |  斜坡 |
|--- | --- | --- |
| <img src="/files/project4/1.gif" width="200"> |<img src="/files/project4/2.gif" width="200"> | <img src="/files/project4/3.gif" width="200"> |

- - - - - - - - - - -

Issagym训练
======

| 平地 | 台阶 |  斜坡 |
|--- | --- | --- |
| <img src="/files/project4/4.gif" width="200"> |<img src="/files/project4/5.gif" width="200"> | <img src="/files/project4/6.gif" width="200"> |

- - - - - - - - - - -

Mujoco部署
======

| 平地 | 台阶 |  斜坡 |
|--- | --- | --- |
| <img src="/files/project4/7.gif" width="200"> |<img src="/files/project4/8.gif" width="200"> | <img src="/files/project4/9.gif" width="200"> |
