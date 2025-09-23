---
permalink: /projects/project1
collection: projects
# category: manuscripts
title: "腾讯小五机器人 (170cm, 80kg) 步态规划与控制"
author_profile: true
---

- - - - - - - - - - -

足底建模
======

<div style="display:flex; justify-content:center; gap:20px;">
<figure style="max-width:240px; text-align:center;">
    <img src="/files/project1/0.jpg" alt="Figure" style="width:100%; height:auto;">
</figure>

<figure style="max-width:240px; text-align:center;">
    <img src="/files/project1/3.png" alt="Figure" style="width:100%; height:auto;">
</figure>

</div>

建模小五特殊足底和地面间的非线性接触，构建了基于Winkler 模型的数值求解器；小五轮足复合足底近似于高跟鞋结构，并与其他足底对比。

+ 平底鞋 / 镂空鞋 / 高跟鞋 鞋底CoP与脚踝力矩关系
  
    <figure>
    <img src="/files/project1/1.gif" alt="Figure" width="640">
    <figcaption>Figure 1: 平底鞋</figcaption>
    </figure>

    <figure>
    <img src="/files/project1/2.gif" alt="Figure" width="640">
    <figcaption>Figure 2: 镂空鞋</figcaption>
    </figure>

    <figure>
    <img src="/files/project1/4.gif" alt="Figure" width="640">
    <figcaption>Figure 3: 高跟鞋</figcaption>
    </figure>

+ 高跟鞋鞋底CoP与鞋跟震动幅度之间的关系
    <div style="display:flex; justify-content:center; gap:20px;">
    <figure style="max-width:240px; text-align:center;">
        <img src="/files/project1/5.png" alt="Figure" style="width:100%; height:auto;">
        <figcaption>Figure 4: 0.5mm震动</figcaption>
    </figure>

    <figure style="max-width:240px; text-align:center;">
        <img src="/files/project1/6.png" alt="Figure" style="width:100%; height:auto;">
        <figcaption>Figure 5: 1.0mm震动</figcaption>
    </figure>

    <figure style="max-width:240px; text-align:center;">
        <img src="/files/project1/7.png" alt="Figure" style="width:100%; height:auto;">
        <figcaption>Figure 5: 1.5mm震动</figcaption>
    </figure>
    </div>

- - - - - - - - - - -

功能实现
======
 + 足底力分配
    <figure>
    <img src="/files/project1/media2.gif" alt="Figure" width="640">
    </figure>

 + 机械臂末端轨迹跟随
    <figure>
    <img src="/files/project1/media3.gif" alt="Figure" width="640">
    </figure>

 + 步态规划
    <figure>
    <img src="/files/project1/media4.gif" alt="Figure" width="640">
    </figure>  

- - - - - - - - - - -

真机实验
======
 + 行走
    <figure>
    <img src="/files/project1/media5.gif" alt="Figure" width="640">
    </figure> 