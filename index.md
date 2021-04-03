# PlasticineLab: A Soft-Body Manipulation Benchmark with Differential Physics

[Zhiao Huang](https://sites.google.com/view/zhiao-huang), [Yuanming Hu](https://yuanming.taichi.graphics/), [Tao Du](https://people.csail.mit.edu/taodu/), [Siyuan Zhou](https://openreview.net/profile?id=~Siyuan_Zhou2), [Hao Su](https://cseweb.ucsd.edu/~haosu/), [Joshua B. Tenenbaum](http://web.mit.edu/cocosci/josh.html), [Chuang Gan](https://people.csail.mit.edu/ganchuang/)

## Abstract

![Alt Text](intro.jpg)

Simulated virtual environments serve as one of the main driving forces behind developing and evaluating skill learning algorithms. However, existing environments typically only simulate rigid body physics. Additionally, the simulation process usually does not provide gradients that might be useful for planning and control optimizations. We introduce a new differentiable physics benchmark called PasticineLab, which includes a diverse collection of soft body manipulation tasks. In each task, the agent uses manipulators to deform the plasticine into a desired configuration. The underlying physics engine supports differentiable elastic and plastic deformation using the DiffTaichi system, posing many underexplored challenges to robotic agents. We evaluate several existing RL methods and gradient-based methods on this benchmark. Experimental results suggest that 1) RL-based approaches struggle to solve most of the tasks efficiently; 2) gradient based approaches, by optimizing open-loop control sequences with the built-in differentiable physics engine, can rapidly find a solution within tens of iterations, but still fall short on multi-stage tasks that require long-term planning. We expect that PlasticineLab will encourage the development of novel algorithms that combine differentiable physics and model-based RL for more complex physics-based skill learning tasks. PlasticineLab will be made publicly available. 


## Tasks
![Alt Text](tasks.jpg)


## Examples

### Move
![Alt Text](Move3D-v1.gif)

### TripleMove
![Alt Text](TripleMove3D-v1.gif)

### Rope
![Alt Text](Rope3D-v1.gif)

### Writer
![Alt Text](Writer3D-v1.gif)

### Chopsticks
![Alt Text](Chopsticks3D-v1.gif)

### Torus
![Alt Text](Torus3D-v1.gif)

### Pinch
![Alt Text](Pinch3D-v2.gif)

### Table
![Alt Text](Table3D-v2.gif)

### Assembly
![Alt Text](Assembly3D-v1.gif)

### RollingPin
![Alt Text](Rollingbin3D-v1.gif)

## Paper
[PlasticineLab: A Soft-Body Manipulation Benchmark with Differentiable Physics](https://openreview.net/forum?id=xCcdBRQEDW)

[Zhiao Huang](https://sites.google.com/view/zhiao-huang), [Yuanming Hu](https://yuanming.taichi.graphics/), [Tao Du](https://people.csail.mit.edu/taodu/), [Siyuan Zhou](https://openreview.net/profile?id=~Siyuan_Zhou2), [Hao Su](https://cseweb.ucsd.edu/~haosu/), [Joshua B. Tenenbaum](http://web.mit.edu/cocosci/josh.html), [Chuang Gan](https://people.csail.mit.edu/ganchuang/)

[[paper](https://openreview.net/pdf?id=xCcdBRQEDW)][[code](https://github.com/hzaskywalker/PlasticineLab)][[bibtex](plb.bib)]


## Related Publications
**A moving least squares material point method with displacement discontinuity and two-way rigid body coupling**
Yuanming Hu, Yu Fang, Ziheng Ge, Ziyin Qu, Yixin Zhu, Andre Pradhana, and Chenfanfu Jiang
ACM Transactions on Graphics (TOG)

**Chainqueen: A real-time differentiable physical simulator for soft robotics**
Yuanming Hu, Jiancheng Liu, Andrew Spielberg, Joshua B Tenenbaum, William T Freeman, Jiajun Wu, Daniela Rus, and Wojciech Matusik
In 2019 International Conference on Robotics and Automation (ICRA)

**Difftaichi: Differentiable programming for physical simulation**
Yuanming Hu, Luke Anderson, Tzu-Mao Li, Qi Sun, Nathan Carr, Jonathan Ragan-Kelley, and Fredo Durand
ICLR, 2020.
