<center># PlasticineLab: A Soft-Body Manipulation Benchmark with Differential Physics

[Zhiao Huang](https://sites.google.com/view/zhiao-huang), [Yuanming Hu](https://yuanming.taichi.graphics/), [Tao Du](https://people.csail.mit.edu/taodu/), [Siyuan Zhou](https://openreview.net/profile?id=~Siyuan_Zhou2), [Hao Su](https://cseweb.ucsd.edu/~haosu/), [Joshua B. Tenenbaum](http://web.mit.edu/cocosci/josh.html), [Chuang Gan](https://people.csail.mit.edu/ganchuang/)
</center>
## Abstract

![Alt Text](intro.jpg)

Simulated virtual environments serve as one of the main driving forces behind developing and evaluating skill learning algorithms. However, existing environments typically only simulate rigid body physics. Additionally, the simulation process usually does not provide gradients that might be useful for planning and control optimizations. We introduce a new differentiable physics benchmark called PasticineLab, which includes a diverse collection of soft body manipulation tasks. In each task, the agent uses manipulators to deform the plasticine into a desired configuration. The underlying physics engine supports differentiable elastic and plastic deformation using the DiffTaichi system, posing many underexplored challenges to robotic agents. We evaluate several existing RL methods and gradient-based methods on this benchmark. Experimental results suggest that 1) RL-based approaches struggle to solve most of the tasks efficiently; 2) gradient based approaches, by optimizing open-loop control sequences with the built-in differentiable physics engine, can rapidly find a solution within tens of iterations, but still fall short on multi-stage tasks that require long-term planning. We expect that PlasticineLab will encourage the development of novel algorithms that combine differentiable physics and model-based RL for more complex physics-based skill learning tasks. PlasticineLab will be made publicly available. 


## Tasks and Reference Solutions
![Alt Text](tasks.jpg)

## Qualitative Results

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
[PlasticineLab: A Soft-Body Manipulation Benchmark with Differentiable Physics](https://openreview.net/forum?id=xCcdBRQEDW)\
Zhiao Huang, Yuanming Hu, Tao Du, Siyuan Zhou, Hao Su, Joshua B. Tenenbaum, Chuang Gan\
[[Paper](https://openreview.net/pdf?id=xCcdBRQEDW)][[Code](https://github.com/hzaskywalker/PlasticineLab)][[Bibtex](plb.bib)]


## Related Publications
**A moving least squares material point method with displacement discontinuity and two-way rigid body coupling**\
[Yuanming Hu](https://yuanming.taichi.graphics/), [Yu Fang](http://squarefk.com/), [Ziheng Ge](https://www.math.ucla.edu/~zihengge/), [Ziyin Qu](https://www.seas.upenn.edu/~ziyinq/), [Yixin Zhu](https://yzhu.io/), [Andre Pradhana](https://www.linkedin.com/in/andre-pradhana-93313428/), and [Chenfanfu Jiang](https://www.seas.upenn.edu/~cffjiang/)\
ACM Transactions on Graphics (TOG)

**Chainqueen: A real-time differentiable physical simulator for soft robotics**\
[Yuanming Hu](https://yuanming.taichi.graphics/), [Jiancheng Liu](https://scholar.google.com/citations?user=ReWNzl4AAAAJ&hl=en), [Andrew Spielberg](http://www.andrewspielberg.com/), [Joshua B. Tenenbaum](http://web.mit.edu/cocosci/josh.html), [William T Freeman](https://billf.mit.edu/), [Jiajun Wu](https://jiajunwu.com/), [Daniela Rus](http://danielarus.csail.mit.edu/), and [Wojciech Matusik](https://cdfg.csail.mit.edu/wojciech)\
In 2019 International Conference on Robotics and Automation (ICRA)

**Difftaichi: Differentiable programming for physical simulation**\
[Yuanming Hu](https://yuanming.taichi.graphics/), [Luke Anderson](https://people.csail.mit.edu/lukea/), [Tzu-Mao Li](https://people.csail.mit.edu/tzumao/), [Qi Sun](https://qisun.me/), [Nathan Carr](https://research.adobe.com/person/nathan-carr/), [Jonathan Ragan-Kelley](https://people.eecs.berkeley.edu/~jrk/), and [Fredo Durand](http://people.csail.mit.edu/fredo/)\
ICLR, 2020.
