---
permalink: /projects/project2
collection: projects
# category: manuscripts
title: "宇树G1机器人 (130cm, 35kg) 抛接重物"
author_profile: true
---

- - - - - - - - - - -

目标
======
相比于抛接小质量物体（运动学问题），大质量物体（动力学问题）更需要机器人全身协同发力，来克服电机力矩输出的限制。这是帮助机器人理解力和学习使用力的重要任务。

- - - - - - - - - - -

挑战
======
+ **结合locomotion与manipulation任务**，难以开发一个统一的框架来同时保证行走与操作的稳定性。
+ **长序列规划与控制任务**，难以在短期奖励与长期奖励之间取得平衡。
+ **任务切换指标设计**，难以设计有效的指标函数来实现任务切换。

- - - - - - - - - - -

贡献
======
+ 一个单阶段强化学习框架，同时完成物体抓取与投掷。
+ 设计了合适的指标函数，实现从抓取任务到投掷任务的切换。

- - - - - - - - - - -

Isaacgym训练过程
======
<figure>
<img src="/files/project2/1.gif" alt="Figure" width="640">
<figcaption>Figure 1: 站立</figcaption>
</figure>

<figure>
<img src="/files/project2/2.gif" alt="Figure" width="640">
<figcaption>Figure 2: 拿住</figcaption>
</figure>

<figure>
<img src="/files/project2/4.gif" alt="Figure" width="640">
<figcaption>Figure 3: 接住</figcaption>
</figure>

<figure>
<img src="/files/project2/4.gif" alt="Figure" width="640">
<figcaption>Figure 4: 接和抛</figcaption>
</figure>

- - - - - - - - - - -

Mujoco部署结果
======
<div style="display:flex; justify-content:center; gap:20px;">
<figure style="max-width:240px; text-align:center;">
    <img src="/files/project2/6.gif" alt="Figure" style="width:100%; height:auto;">
    <figcaption>Figure 5: 站立</figcaption>
</figure>

<figure style="max-width:240px; text-align:center;">
    <img src="/files/project2/7.gif" alt="Figure" style="width:100%; height:auto;">
    <figcaption>Figure 6: 拿住</figcaption>
</figure>

<figure style="max-width:240px; text-align:center;">
    <img src="/files/project2/8.gif" alt="Figure" style="width:100%; height:auto;">
    <figcaption>Figure 7: 接住</figcaption>
</figure>

<figure style="max-width:240px; text-align:center;">
    <img src="/files/project2/5.gif" alt="Figure" style="width:100%; height:auto;">
    <figcaption>Figure 8: 接和抛</figcaption>
</figure>
</div>