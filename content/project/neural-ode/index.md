---
title: "Neural ODE for Planar Pushing Dynamics"
image: "neural-ode.gif"
summary: "基于 Neural ODE 的平面推块动力学建模与闭环控制"
tags: ["Neural ODE", "Robotics", "Control"]
---
[For more detail. You can download my project report here.](./ROB498_Project.pdf)
## 项目简介
本项目利用 **Neural ODE** 来建模机器人平面推块的动力学，  
并结合 MPPI 控制器实现闭环推方块到目标位姿的控制。
![这是图片的描述文字，可以为空](./animation.gif)


## 我的工作
- 设计并实现 Neural ODE 模型结构（ODEFunc 与求解器）  
- 系统调优超参数（积分方法、步长、网络深度/宽度、学习率）  
- 训练单步与多步模型，并与残差网络对比  
- 将模型集成进 MPPI 控制器，完成仿真闭环控制实验  

## 成果
- 验证误差显著低于基线模型  
- 多步预测精度更高，尤其在角度预测上优势明显  
- 成功完成 Franka Panda 推方块任务的闭环控制  
