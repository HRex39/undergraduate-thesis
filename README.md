# 基于深度强化学习的自动驾驶避障技术研究![](https://raw.githubusercontent.com/BITNP/BIThesis/main/assets/bithesis_badge_solid.svg?sanitize=true)

## 摘要
自动驾驶系统保证了快捷、安全、高效的驾驶体验，实现自动驾驶避障需要自动驾驶决策和控制系统的紧密配合。强化学习通过不断探索环境，自主学习复杂的控制模型，深度学习与强化学习相结合形成的深度强化学习方法可实现端到端的决策与控制，逐渐成为自动驾驶领域的研究热点。本文以实现端到端的自动驾驶决策器和控制器作为研究目标，围绕两种不同复杂度的仿真环境，针对DQN及其改进算法搭建神经网络模型开展了相关技术研究，主要研究内容如下：

（1）针对强化学习的相关算法选择，第2章通过对强化学习算法原理的分析，引出了适用于无模型的 Q-learning 算法和 DQN 算法，针对于DQN算法的不足和缺陷，介绍了Double DQN算法和Dueling DQN算法的原理，并对DQN及其改进算法的适用场景进行了分析。

（2）针对自动驾驶避障算法，第3章完成了自动驾驶决策器与控制器的算法设计。通过对两种仿真环境（Highway-Env、Metadrive）状态值、动作值与奖励函数的对比与分析，设计了DQN及其改进算法的网络结构及超参数，对自动驾驶决策器与控制器的学习过程进行分析，使其完成自动驾驶决策和控制两方面的任务要求。

（3）针对实验验证，第4章进行了两种仿真环境中决策器与控制器的实验，验证了提出的自动驾驶避障算法的可行性和有效性，并对具体的实验内容进行了设计，对最终的实验结果进行了详细的分析与改进。

实验结果表明，本文设计实现的基于DQN及其改进算法的自动驾驶决策器和控制器均满足实验要求，达到了预期的控制效果，能够有效提高自动驾驶车辆在决策和控制中的鲁棒性。对于较为简单的网络结构，DQN特别是Double DQN算法由于其改进的动作选择和评估方法，能够获得更加稳定有效的行为策略。本文的成果为自动驾驶决策器和控制器的研究提供了借鉴和参考，也为复杂动力学模型问题的解决提供了新的思路和方法。

## 项目结构

```
.
├── chapters
│   ├── 0_abstract.tex
│   ├── 1_chapter1.tex
│   ├── 2_chapter2.tex
│   ├── 3_chapter3.tex
│   └── 4_chapter4.tex
├── images
│   ├── bit_logo.png
│   ├── header.png
│   ├── chapter1
│   │   ├── Autodrive_structure.png
│   │   ├── DRL_structure.png
│   │   ├── EndtoEnd_structure.png
│   │   └── RL_structure.png
│   ├── chapter2
│   │   ├── DQN_model.png
│   │   ├── Dueling_DQN.png
│   │   ├── Experience_Replay.png
│   │   └── RL_struction.png
│   ├── chapter3
│   │   ├── highway_decision.png
│   │   ├── highway-env.png
│   │   ├── highway_forward.png
│   │   ├── metadrive_control.png
│   │   ├── metadrive_forward.png
│   │   └── metadrive.png
│   └── chapter4
│       ├── HighwayPic
│       ├── HighwayVideoSc
│       ├── MetadrivePic
│       └── MetadriveVideoSc
├── main.pdf
├── main.tex
├── misc
│   ├── 0_cover.tex
│   ├── 1_comment.pdf
│   ├── 1_mission.pdf
│   ├── 1_originality.pdf
│   ├── 1_originality.tex
│   ├── 2_toc.tex
│   ├── 3_conclusion.tex
│   ├── 4_reference.tex
│   ├── 5_appendix.tex
│   ├── 6_acknowledgements.tex
│   └── ref.bib
└── README.md
```

## 编译方式

```
-> xelatex
-> biber
-> xelatex
-> xelatex
```

## 鸣谢

北京理工大学  

此文件夹中包含了北京理工大学毕业设计（论文）的全部内容，有关模板的使用方法更为详细的介绍，请参考：[BIThesis Wiki - 本科生毕业论文：Graduation thesis](https://bithesis.bitnp.net/guide/3-templates/final-graduation-thesis)。

