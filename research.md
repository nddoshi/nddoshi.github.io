---
layout: default
title: Research
# classes: wide
---
<h1 style="text-align:center;"> Research </h1>

My research is broadly focused on developing technologies that allow robots to make purposeful and reliable contact with the world. Within this area I work both on developing algorithms for model-based planning and control and the design of robot end-effectors (e.g., robot hands and feet). Moreover, I study contact in the context of both robot locomotion and manipulation, and for robots of various sizes. 

<!-- ########################## Entry 0 ############################# -->
--- 

<h3 style="text-align:center;"> Planning and control of manipulation primitives </h3>

<img src="/assets/img/hddp_primitives-1.png" alt="hddp" align=left width="400" hspace="20"> 
Manipulation primitives can be used to simplify the planning of contact-rich manipulation. I am developing more closed-loop 

I am developing a framework for closed-loop execution of these hybrid manipulation primitives. Planning and control of these tasks is challenging as they are often hybrid, underactuated, and stochastic. Our long-term goal is to develop a framework that can plan a trajectory from any initial condition, recover from large perturbations, and re-plan the mode sequence in real-time (~20 Hz).

Our current approach uses Differential Dynamic Programming (DDP) to plan a trajectory over a finite horizon, consider a small number of contact switches, and generate a stabilizing controller. Combining our approach with efficient mechanics representations enables planning of plan pose-to-pose trajectories from most initia configurations in reasonable time (one to five seconds) for two planar manipulation primitives: pushing and pivoting. A key insight is that while ability to select and switch contact locations is key to the success of these primitives, only one to two contact location switches are needed to converge from most initial configurations.

Next steps include improving the speed and scalability (e.g., consider more hybrid switches) of our approach.

#### Relevant Work: 
**ICRA 2020:** Hybrid DDP for Planar Manipulation Primitives. [[Publication]](https://ieeexplore.ieee.org/document/9197414), [[Video]](https://www.youtube.com/watch?v=YGSe4cUfq6Q&feature=youtu.be&ab_channel=MCubeLabMIT) <br>
**IROS 2021 Workshop:** Hybrid iLQR for manipulation with fixed environmental contacts. [[Abstract]](./assets/pdfs/Robotic_In_Situ_Workshop.pdf), [[Video]](./assets/vids/DoshiNeel_iLQR_Primitivesc.mp4) <br> 
**IROS 2021 Workshop:** Pivoting an unkown object about an environmental contact. [[Abstract]](./assets/pdfs/Fail_to_Grasp_Workshop.pdf) <br>

<!-- ########################## Entry 1 ############################# -->
---

<h3 style="text-align:center;"> Switchable adhesion for robot end-effectors </h3>

<img src="/assets/img/Seb_EA.png" alt="hddp" align=left width="400" hspace="20"> 


#### Relevant Work:
**Science 2018:**  Climbing with a quadrupedal microrobot using electroadhesion. [[Publication]](https://robotics.sciencemag.org/content/3/25/eaau3038), [[Video]](https://www.youtube.com/watch?v=hPqFJ_lwHjY&ab_channel=MicroroboticsLab) <br>
**IROS 2020:** PnuGrip: An active two-phase gripper for dexterous manipulation. [[Publication]](http://ras.papercept.net/images/temp/IROS/files/1356.pdf), [[Video]]() <br>


<!-- ########################## Entry 2 ############################# -->
---

<h3 style="text-align:center;"> Trajectory optimization for legged microrobots</h3>

<img src="/assets/img/Intro-Fig_increasedexposure-1.png" alt="hddp" align=left width="400" hspace="20"> 
Planning locomotion strategies for legged microrobots is challenging due to their complex morphology and discontinuous contact interactions with the environment. We developed a framework for systematically modeling, planning, and controlling legged microrobots. This involved building a three-dimensional dynamic
model of a 1.43 g quadrupedal microrobot and developing variational contact-implicit trajectory optimization methods to generate feasible whole-body locomotion plans for this robot. Our method is used to plan periodic gaits at multiple stride frequencies and on various surfaces. These gaits achieve high per-cycle velocities, including a maximum of 10.87 mm/cycle, which is 33% faster than previously measured for this robot. Furthermore, we plan and execute a vertical jump of 9.96 mm, which is 78% of the robot’s body height.

#### Relevant Work: 
**RSS 2018:** Contact-implicit trajectory optimization for a quadrupedal microrobot. [[Publication]](http://www.roboticsproceedings.org/rss14/p41.pdf), [[Video]](https://www.youtube.com/watch?v=fg5MiyJ7dXw&ab_channel=HarvardAgileRoboticsLab) <br>
**IJRR 2019:** Contact-implicit trajectory optimization using variational integrators. [[Publication]](https://journals.sagepub.com/doi/full/10.1177/0278364919849235)<br>


<!-- ########################## Entry 3 ############################# -->
---

<h3 style="text-align:center;"> Computationally efficient control for legged microrobots </h3>

<img src="/assets/img/bio_bio-1.png" alt="hddp" align=left width="400" hspace="20"> 
Limitations in actuation, sensing, and computation have forced small legged robots to rely on mechanically mediated leg trajectories for effective locomotion. Advances in manufacturing, however, have enabled the development of  small legged robote capable of operation at multiple stride frequencies using multi-degree-of-freedom leg trajectories. Proprioceptive sensing and control is key to extending the capabilities of these robots to a broad range of operating conditions. 

[ICRA 2017]

[Bio&Bio 2019] Here we use concomitant sensing for piezoelectric actuation with a computationally efficient framework for estimation and control of leg trajectories on a quadrupedal microrobot. We demonstrate accurate position estimation and control during locomotion across a wide range of stride frequencies. This capability enables the exploration of two bio-inspired parametricleg trajectories designed to reduce leg slip and increase locomotion performance (e.g., speed, cost-of-transport, etc.).  Using this approach, we demonstrate hig performance locomotion at stride frequencies where the robot’s natural dynamics result in poor open-loop locomotion.

#### Relevant Work:
**ICRA 2017:** Phase control for a legged microrobot operating at resonance. [[Publication]](https://ieeexplore.ieee.org/document/7989704) <br>
**Bio&Bio 2019:** Locomotion at multiple stride frequencies using proprioceptive feedback. [[Publication]](https://iopscience.iop.org/article/10.1088/1748-3190/ab295b) <br>

<!-- ########################## Entry 4 ############################# -->
---

<h3 style="text-align:center;"> Design of flexure-based microrobots </h3>



Advances in laminate-based manufacturing has enabled the development of highly articulated insect-scale robots. It  is, however, difficult to characterize and model the performance of these robots due to a poor understanding of the mechanics of their joints (compliant flexures) and actuators (piezoelectric bimorphs). 

<img src="/assets/img/figS1_spherical_five_bar.png" alt="hddp" align=left width="300" hspace="20"> 
[IROS 2015] Here we develop a lumped-parameter mechanics-model of the compliant flexures, and use this to build a model of the Harvard Ambulatory MicroRobot (HAMR) transmission. This model is then used to redesign the transmission for improved performance. This model-based redesign results in a 266% increase in the work done by the foot when compared to a previous version of HAMR, and leads to a payload capacity of 2.9g, which is about twice the robot's mass and a 114% increase.

<img src="/assets/img/Delta1.png" alt="hddp" align=left width="300" hspace="20"> 
[Science 2018] The improved understanding of the actuators and compliant flexures was used to inform the design 

#### Relevant Work: 
**IROS 2015:** Model driven design for flexure-based microrobots. [[Publication]](https://ieeexplore.ieee.org/document/7353959) <br>
**Science 2018:** The milliDelta. [[Publications]](https://robotics.sciencemag.org/content/3/14/eaar3018), [[Video]](https://www.youtube.com/watch?v=rHUnqYDgUFY) <br>




