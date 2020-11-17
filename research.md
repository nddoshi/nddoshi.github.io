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

<img src="/assets/img/ilqr-primitives.png" alt="hddp" align=left width="250" height="250" hspace="20"> 
We are interested in developing a framework for closed-loop execution of contact-rich pose-to-pose manipulation tasks. Planning and control of these tasks is challenging as they are often hybrid, underactuated, and stochastic. Our long-term goal is to develop a framework that can plan a trajectory from any initial condition, recover from large perturbations, and re-plan the mode sequence in real-time (~20 Hz).

Our current approach uses Differential Dynamic Programming (DDP) to plan a trajectory over a finite horizon, consider a small number of contact switches, and generate a stabilizing controller. Combining our approach with efficient mechanics representations enables planning of plan pose-to-pose trajectories from most initia configurations in reasonable time (one to five seconds) for two planar manipulation primitives: pushing and pivoting. A key insight is that while ability to select and switch contact locations is key to the success of these primitives, only one to two contact location switches are needed to converge from most initial configurations.

Next steps include improving the speed and scalability (e.g., consider more hybrid switches) of our approach.

#### Relevant Work: 

**IROS 2021 Workshop:** Pivoting an unkown object about an environmental contact. [[Abstract]](https://wvrtc.com/iros2020/contributed-abstracts/doshi.pdf), [[Video]](https://wvrtc.com/iros2020/contributed-abstracts.shtml#) <br>
**IROS 2021 Workshop:** Hybrid iLQR for manipulation with fixed environmental contacts. [[Abstract]](https://drive.google.com/file/d/1U4rOjIZ4KvS9X7MZOA6VnEBE9bek4FCR/view) <br> 
**ICRA 2020:** Hybrid DDP for Planar Manipulation Primitives. [[Publication]](https://ieeexplore.ieee.org/document/9197414), [[Video]](https://www.youtube.com/watch?v=YGSe4cUfq6Q&feature=youtu.be&ab_channel=MCubeLabMIT) <br>

<!-- ########################## Entry 1 ############################# -->
---

<h3 style="text-align:center;"> Switchable adhesion for robot end-effectors </h3>

One of the challenges 

#### Relevant Work  

**IROS 2020:** PnuGrip: An active two-phase gripper for dexterous manipulation. [[Publication]](http://ras.papercept.net/images/temp/IROS/files/1356.pdf), [[Video]]() <br>
**Science 2018:**  Climbing with a quadrupedal microrobot using electroadhesion. [[Publication]](https://robotics.sciencemag.org/content/3/25/eaau3038), [[Video]](https://www.youtube.com/watch?v=hPqFJ_lwHjY&ab_channel=MicroroboticsLab) <br>

<!-- ########################## Entry 2 ############################# -->
---

<h3 style="text-align:center;"> Trajectory optimization for legged microrobots</h3>

blah blah blah blah 

#### Relevant Work  

**IJRR 2019:** Contact-implicit trajectory optimization using variational integrators. [[Publication]](https://journals.sagepub.com/doi/full/10.1177/0278364919849235)<br>
**RSS 2018:** Contact-implicit trajectory optimization for a quadrupedal microrobot. [[Publication]](http://www.roboticsproceedings.org/rss14/p41.pdf), [[Video]](https://www.youtube.com/watch?v=fg5MiyJ7dXw&ab_channel=HarvardAgileRoboticsLab) <br>

<!-- ########################## Entry 3 ############################# -->
---

<h3 style="text-align:center;"> Computationally efficient control for legged microrobots </h3>

blah blah blah blah 

#### Relevant Work  

**Bio&Bio 2019:** Locomotion at multiple stride frequencies using proprioceptive feedback. [[Publication]](https://journals.sagepub.com/doi/full/10.1177/0278364919849235) <br>
**ICRA 2017:** Phase control for a legged microrobot operating at resonance. [[Publication]](https://ieeexplore.ieee.org/document/7989704) <br>

<!-- ########################## Entry 3 ############################# -->
---

<h3 style="text-align:center;"> Design of flexure-based microrobots </h3>

blah blah blah blah 

#### Relevant Work  



**IROS 2015:** Model driven design for flexure-based microrobots. [[Publication]](https://ieeexplore.ieee.org/document/7353959) <br>
**Science 2018:** The milliDelta. [[Publications]](https://robotics.sciencemag.org/content/3/14/eaar3018), [[Video]](https://www.youtube.com/watch?v=rHUnqYDgUFY) <br>




