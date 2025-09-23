---
permalink: /projects/project3
collection: projects
title: "普渡D9机器人 (165cm, 65kg) 行走、奔跑"
author_profile: true
---

- - - - - - - - - - -

Pudu D9机器人参数
======
+ 外观图
    <figure>
        <img src="/files/project3/1.png" alt="Figure" width="640">
    </figure>

+ 结构图
    <figure>
        <img src="/files/project3/2.png" alt="Figure" width="640">
    </figure>

- - - - - - - - - - -

训练初始化
======
+ 生成初始姿态
    <figure>
        <img src="/files/project3/dataset.gif" alt="Figure" width="640">
    </figure>

+ 确定关节偏置

| Joint Name | Angle Limit | default_joint_angle | 
|---  | --- | --- | 
| {Left,Right}_Hip_Joint_Pitch  | [-0.9599, 1.5708] | 0.3 | 
| {Left,Right}_Knee_Joint_Pitch | [-1.5708, 0] | -0.7 | 
| {Left,Right}_Ankle_Joint_Pitch | [-0.4, 0.6] | 0.4 | 
| others | ... | 0 | 

+ 将base height放在`0.88m`处，给定`default_joint_angles`下的机器人站姿为
    <figure>
        <img src="/files/project3/3.png" alt="Figure" width="640">
    </figure>

+ 确定电机参数`stiffness`和`damping`
  
这两个参数和机器人结构和质量有关，我们参考宇树g1和h1机器人的定义，将pudu d9的关节电机参数定义为

| Joint Name | stiffness | damping | 
|---  | --- | --- | 
| Hip_Joint_Roll  | 200 | 2.5 | 
| Hip_Joint_Yaw | 200 | 2.5 | 
| Hip_Joint_Pitch | 200 | 2.5 | 
| Knee | 300 | 4 | 
| Ankle | 80 | 2.5 | 
| Waist_Joint_Yaw | 100 | 2.5 |

- - - - - - - - - - -

Isaaclab训练效果
======

+ 平地走
    <figure>
    <img src="/files/project3/media8.gif" alt="Figure" width="640">
    </figure>

+ 复杂地形走
    <figure>
    <img src="/files/project3/media10.gif" alt="Figure" width="640">
    </figure>

+ 跑步
    <figure>
    <img src="/files/project3/media9.gif" alt="Figure" width="640">
    </figure>