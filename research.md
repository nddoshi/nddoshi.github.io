---
layout: default
title: Research
# classes: wide
---
<h1 style="text-align:center;"> Research </h1>

 <font face="arial" color="black">
<p> My research is focused on developing synergistic mechanical and algorithmic solutions that allow robots to make <b>purposeful and reliable </b> with contact real-world objects and surfaces. To this end, I have predominantly focused on solving problems in robotic manipulation and locomotion, using techniques from dynamics/mechanics, control, optimization, mechanical design, and machine learning. </p>

<hr>
<!-- ########################## Entry 0 ############################# -->


<h3 style="text-align:center;"> Planning and executing contact-rich manipulation</h3>
<br>
A key challenge in manipulation is designing motions that react intelligently to unexpected perturbations and changes in the environment. My research uses  mechanics, trajectory optimization, and estimation/control theory to develop reactive manipulation primitives that can be sequenced to achieve complex motions.

<p>
    <img src="/assets/img/contact-config-regulation.png" alt="Rectangle_Balance" style="float:right;width:30%;" hspace="25"/>
</p>

<p> <b> ICRA 2022: Manipulation of unknown objects via contact configuration regulation. </b> We develoed an approach to robotic manipulation of unknown objects through regulation of the object’s contact configuration: the location, geometry, and mode of all contacts between the object, robot, and environment. A contact configuration constrains the forces and motions that can be applied to the object; however, synthesizing these constraints generally requires knowledge of the object’s pose and geometry. We develop an object-agnostic approach for estimation and control that circumvents this need. Our framework directly estimates a set of wrench and motion constraints which it uses to regulate the contact configuration. We use this to reactively manipulate unknown planar polygonal objects in the gravity plane. 
<a href="https:://nddoshi.github.io/assets/pdfs/doshi_icra2022.pdf" target="_blank"><b>[Publication]</b></a>
</p>


<p>
    <img src="/assets/img/hddp_primitives.png" alt="Rectangle_Balance" style="float:left;width:20%;" hspace="25" />
</p>
<p> <b> ICRA 2020: Hybrid DDP for planar manipulation primitives. </b> We use Hybrid Differential Dynamic Programming (HDDP) to plan pose-to-pose primtive manipulations by planning a trajectory over a finite horizon, considering a small number of contact switches, and generating a stabilizing controller. We can plan trajectories from most initial configurations in reasonable time (one to five seconds) for two planar manipulation primitives: pushing and pivoting. The success of our approach is contingent on the fact that while ability to select and switch contact locations is key to the success of these primitives, only one to two contact location switches are needed to converge from most initial configurations. 
<!-- <br> -->
<a href="https:://nddoshi.github.io/assets/pdfs/doshi_icra2020.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=YGSe4cUfq6Q&feature=youtu.be&ab_channel=MCubeLabMIT" target="_blank"><b> [Video]</b></a> 
</p>
<br>
<hr>

<!-- ########################## Entry 1 ############################# -->


<h3 style="text-align:center;"> Closed-loop locomotion
of centimeter-scale legged robots  </h3>
<br>
Planning locomotion strategies for centimeter-scale legged robots is challenging due to the limited availibity of on-board computation. In my work, I develop high fidelity robot models and high accuracy trajectory optimization techniques for offline planning of realistic locomotion plan that can be tracked with simple on-board controllers.

<br>

<p>
<img src="/assets/img/Intro-Fig_increasedexposure.png" alt="hamr-jump" style="float:left;width:40%;" hspace="10" vspace="10"/>
</p>
<p>
<b>RSS 2018, IJRR 2019: Contact-implicit trajectory optimization for a centimeter-scale quadrupedal robot. </b> We developed a framework for systematically modeling, planning, and controlling centimeter-scale legged robots. This involved building a three-dimensional dynamic model of a millmeter-scale quadruped and developing a second-order contact-implicit trajectory optimization method to generate feasible whole-body locomotion plans for this robot. Our method is used to plan periodic gaits at multiple stride frequencies and on various surfaces. These gaits achieve high per-cycle velocities, including a maximum of 10.87 mm/cycle, which is 33% faster than previously measured for this robot. We also plan and execute a vertical jump of 9.96 mm, which is 78% of the robot’s body height.
 <a href="https:://nddoshi.github.io/assets/pdfs/doshi_rss2018.pdf" target="_blank"><b>[RSS Publication]</b></a> 
<a href="https:://nddoshi.github.io/assets/pdfs/manchester_ijrr2019.pdf" target="_blank"><b>[IJRR Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=fg5MiyJ7dXw&ab_channel=HarvardAgileRoboticsLab" target="_blank"><b> [Video]</b></a>
</p>


<p>
<img src="/assets/img/bio_bio.png" alt="bio-bio" style="float:right;width:40%;" hspace="25" vspace="10"/> 
</p>
<p> <b> Bio&Bio 2019: Locomotion at multiple stride frequencies using proprioceptive feedback. </b> We use concomitant sensing for piezoelectric actuation with a computationally efficient framework for estimation and control of leg trajectories on a centimeter-scale quadrupedal robot. We demonstrate accurate position estimation and control during locomotion across a wide range of stride frequencies. This capability enables the exploration of two bio-inspired parametric leg trajectories designed to reduce leg-slip and increase locomotion performance. Our approach enables high performance locomotion at stride frequencies where the robot’s natural dynamics result in poor open-loop locomotion. 
 <a href="https:://nddoshi.github.io/assets/pdfs/doshi_biobio2019.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https:://nddoshi.github.io/assets/pdfs/doshi_biobio2019.pdf" target="_blank"><b> [Video]</b></a>

<br>
<hr>
<!-- ########################## Entry 2 ############################# -->


<h3 style="text-align:center;"> Switchable adhesion for robot end-effectors </h3>

<br>
Enforcing a sequence of planned motions can be challenging under model uncertainty and with limited sensing. My research uses switchable adhesion to enforce the planned contact-state (e.g., sticking versus sliding) during locomotion and manipulation.
<br>

<p>
<img src="/assets/img/pnugrip.png" alt="pnu-grip" style="float:right;width:40%;" hspace="25" />
</p>
<p> <b>IROS 2020: PnuGrip, an active two-phase gripper for dexterous manipulation. </b> We present the design of an active two-phase finger for mechanically mediated dexterous manipulation. This finger enables re-orientation of a grasped object by using a pneumatic braking mechanism to transition between free-rotating and fixed (i.e., braked) phases. Our design allows controlled high-bandwidth (5 Hz) phase transitions independent of the grasping force for manipulation of a variety of objects. We demonstrate several pick-and-place manipulations common to industrial and laboratory automation settings that are simplified by our design.
 <a href="https:://nddoshi.github.io/assets/pdfs/taylor_iros2020.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=dtDefve8KFk" target="_blank"><b> [Video]</b></a>
</p>

<p>
<img src="/assets/img/Seb_EA.png" alt="hamr-ea" style="float:left;width:15%;" hspace="25" />
</p>
<p> <b> Science Robotics 2018: Climbing with a quadrupedal centimeter-scale robot using electroadhesion.</b> We present a centimeter-scale quadrupredal robot with electroadhesive feet. This robot leverages electroadhesion to achieve locomotion on horizontal, vertical, inverted, and curved conductive surfaces, highlighting its unique locomotive flexibility. As a demonstration of its potential for industrial applications, such as in-situ inspection of high-value assets, we show that the robot is capable of achieving open-loop, inverted locomotion inside a curved portion of a commercial jet engine. 
<a href="https:://nddoshi.github.io/assets/pdfs/deRivaz_scirob2018.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=hPqFJ_lwHjY&ab_channel=MicroroboticsLab" target="_blank"><b> [Video]</b></a>
</p>

<br>
<hr>
<!-- ########################## Entry 3 ############################# -->

<h3 style="text-align:center;"> Design of flexure-based centimeter-scale robots </h3>
<br>
Advances in laminate-based manufacturing have enabled the development of highly articulated centimeter-scale robots. In my work, I develop models of their joints (compliant flexures) and actuators (piezoelectric bimorphs) to predict their behavior and improve their design.
<br>

<p>
<img src="/assets/img/Delta1.png" alt="milldelta" style="float:right;width:15%;" hspace="25"> 
</p>
<p> <b> Science Robotics 2018: The milliDelta. </b> An improved understanding of the compliant flexures was used to inform the design of the milliDelta. This robot can operate with precision down to ∼5μm in a 7 mm<sup>3</sup> workspace and can follow periodic trajectories at frequencies up to 75 Hz. The milliDelta can be used for applications such as vibration cancellation in microsurgery and microassembly, or micromanipulation. 
<a href="https:://nddoshi.github.io/assets/pdfs/mcclintock_scirob2018.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=rHUnqYDgUFY" 
target="_blank"><b> [Video]</b></a>
</p>

<p>
<img src="/assets/img/sfb.png" alt="hamr-transmission"  style="float:left;width:20%;" hspace="25"> 
</p>

<p> <b> IROS 2015: Model driven design for flexure-based centimeter-scale robots. </b> We develop a lumped-parameter mechanics-model of the compliant flexures, and use this to build a model of a centimeter-scale quadrupedal robot's transmission. This model is then used to redesign the transmission, resulting in a 266% increase in the work done by the foot when compared to a previous version of the robot. The results in a payload capacity of 2.9g, which is about twice the robot's mass and a 114% increase. 
<a href="https:://nddoshi.github.io/assets/pdfs/doshi_iros2015.pdf" target="_blank"><b>[Publication]</b></a> 
</p>



