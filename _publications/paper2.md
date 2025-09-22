---
permalink: /publications/paper2
collection: publications
category: manuscripts
title: "Event Imagination Model for Policy Learning"
# author_profile: true
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
我们提出了一个 两阶段 VLA 框架：
+ 第一阶段：从原始视频中抽取事件流，并训练模型去预测事件流的未来演化；这样能够把长时序的动态压缩成更易处理的表征，并且突出关键转变。
+ 第二阶段：结合语言指令与预测的事件流，用于指导动作规划，从而生成既有上下文感知又具备前瞻性的策略。

- - - - - - - - - - -

算法
======
<img src="/files/paper2/image.png" alt="Figure" width="640">

- - - - - - - - - - -

仿真实验
======
+ Stage 1
  + <img src="/files/paper2/4.png" alt="Figure 4" width="320"> --> <img src="/files/paper2/4.gif" alt="gif 4" width="240">
  + <img src="/files/paper2/3.png" alt="Figure 3" width="320"> --> <img src="/files/paper2/3.gif" alt="gif 3" width="240">
  + <img src="/files/paper2/2.png" alt="Figure 2" width="320"> --> <img src="/files/paper2/2.gif" alt="gif 2" width="240">
  + <img src="/files/paper2/1.png" alt="Figure 1" width="320"> --> <img src="/files/paper2/1.gif" alt="gif 1" width="240">

+ Stage 2
  + <img src="/files/paper2/4.png" alt="Figure 4" width="160"> + <img src="/files/paper2/4.gif" alt="gif 4" width="120"> --> actions ~ <img src="/files/paper2/video.gif" alt="gif 4" width="120">

