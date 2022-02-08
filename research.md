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

<p> <b> ICRA 2022: Manipulation of unknown objects via contact configuration regulation. </b> We developed an approach to robotic manipulation of unknown objects through regulation of the object’s contact configuration: the location, geometry, and mode of all contacts between the object, robot, and environment. A contact configuration constrains the forces and motions that can be applied to the object; however, synthesizing these constraints generally requires knowledge of the object’s pose and geometry. We develop an object-agnostic approach for estimation and control that circumvents this need. Our framework directly estimates a set of wrench and motion constraints which it uses to regulate the contact configuration. We use this to reactively manipulate unknown planar polygonal objects in the gravity plane. 
<a href="https://nddoshi.github.io/assets/pdfs/doshi_icra2022.pdf" target="_blank"><b>[Publication]</b></a>
</p>


<p>
    <img src="/assets/img/hddp_primitives.png" alt="Rectangle Balance" style="float:left;width:20%;" hspace="25" />
</p>
<p> <b> ICRA 2020: Hybrid DDP for planar manipulation primitives. </b> We use Hybrid Differential Dynamic Programming (HDDP) to plan pose-to-pose primitive manipulations by planning a trajectory over a finite horizon, considering a small number of contact switches, and generating a stabilizing controller. We can plan trajectories from most initial configurations in reasonable time (one to five seconds) for two planar manipulation primitives: pushing and pivoting. The success of our approach is contingent on the fact that while ability to select and switch contact locations is key to the success of these primitives, only one to two contact location switches are needed to converge from most initial configurations. 
<!-- <br> -->
<a href="https://nddoshi.github.io/assets/pdfs/doshi_icra2020.pdf"
 target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=YGSe4cUfq6Q&feature=youtu.be&ab_channel=MCubeLabMIT" target="_blank"><b> [Video]</b></a> 
</p>
<br>
<hr>

<!-- ########################## Entry 1 ############################# -->


<h3 style="text-align:center;"> Closed-loop locomotion
of centimeter-scale legged robots  </h3>
<br>
Planning locomotion strategies for centimeter-scale legged robots is challenging due to the limited availability of on-board computation. In my work, I develop high fidelity robot models and high accuracy trajectory optimization techniques for offline planning of realistic locomotion plan that can be tracked with simple on-board controllers.

<br>

<p>
    <img src="/assets/img/rml-hamr.png" alt="RML Hamr" style="float:right;width:35%;" hspace="25" />
</p>

<p> <b> ICRA 2021, Residual Model Learning for Microrobot Control </b>

 A majority of microrobots are constructed using compliant materials that are difficult to model analytically. Challenges in data collection on microrobots and large errors between simulated models and real robots make current model-based learning and sim-to-real transfer methods difficult to apply. We propose a novel framework residual model learning (RML) that leverages approximate models to substantially reduce the sample complexity associated with learning an accurate robot model. We show that using RML, we can learn a model of the Harvard Ambulatory MicroRobot (HAMR) using just 12 seconds of passively collected interaction data. The learned model is accurate enough to be leveraged as a "proxy-simulator" for learning walking and turning behaviors using model-free reinforcement learning algorithms.
<a href="https://nddoshi.github.io/assets/pdfs/gruenstein_icra2021.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?time_continue=1&v=rwsz5f2Yp8g&feature=emb_logo" target="_blank"><b> [Video]</b></a>
</p>

<p>
<img src="/assets/img/Intro-Fig_increasedexposure.png" alt="hamr-jump" style="float:left;width:30%;" hspace="10" vspace="10"/>
</p>
<p>
<b>RSS 2018, IJRR 2019: Contact-implicit trajectory optimization for a centimeter-scale quadrupedal robot. </b> We developed a framework for systematically modeling, planning, and controlling centimeter-scale legged robots. This involved building a three-dimensional dynamic model of a centimeter-scale quadruped and developing a second-order contact-implicit trajectory optimization method to generate feasible whole-body locomotion plans for this robot. Our method is used to plan periodic gaits at multiple stride frequencies and on various surfaces. These gaits achieve high per-cycle velocities, including a maximum of 10.87 mm/cycle, which is 33% faster than previously measured for this robot. We also plan and execute a vertical jump of 9.96 mm, which is 78% of the robot’s body height.
 <a href="https://nddoshi.github.io/assets/pdfs/doshi_rss2018.pdf" target="_blank"><b>[RSS Publication]</b></a> 
<a href="https://nddoshi.github.io/assets/pdfs/manchester_ijrr2019.pdf" target="_blank"><b>[IJRR Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=fg5MiyJ7dXw&ab_channel=HarvardAgileRoboticsLab" target="_blank"><b> [Video]</b></a>
</p>


<p>
<img src="/assets/img/bio_bio.png" alt="bio-bio" style="float:right;width:40%;" hspace="25" vspace="10"/> 
</p>
<p> <b> Bio&Bio 2019: Locomotion at multiple stride frequencies using proprioceptive feedback. </b> We use concomitant sensing for piezoelectric actuation with a computationally efficient framework for estimation and control of leg trajectories on a centimeter-scale quadrupedal robot. We demonstrate accurate position estimation and control during locomotion across a wide range of stride frequencies. This capability enables the exploration of two bio-inspired parametric leg trajectories designed to reduce leg-slip and increase locomotion performance. Our approach enables high performance locomotion at stride frequencies where the robot’s natural dynamics result in poor open-loop locomotion. 
 <a href="https://nddoshi.github.io/assets/pdfs/doshi_biobio2019.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://nddoshi.github.io/assets/vids/PerformanceRecovery_comp.mp4" target="_blank"><b> [Video]</b></a>

<br>
<hr>
<!-- ########################## Entry 2 ############################# -->


<h3 style="text-align:center;"> Controlling contact-interactions via mechanism design </h3>

<br>
Enforcing a sequence of planned motions can be challenging under model uncertainty and with limited sensing. My research uses switchable adhesion to enforce the planned contact-state (e.g., sticking versus sliding) during locomotion and manipulation.
<br>

<p>
<img src="/assets/img/pnugrip.png" alt="pnu-grip" style="float:right;width:40%;" hspace="25" />
</p>
<p> <b>IROS 2020: PnuGrip, an active two-phase gripper for dexterous manipulation. </b> We present the design of an active two-phase finger for mechanically mediated dexterous manipulation. This finger enables re-orientation of a grasped object by using a pneumatic braking mechanism to transition between free-rotating and fixed (i.e., braked) phases. Our design allows controlled high-bandwidth (5 Hz) phase transitions independent of the grasping force for manipulation of a variety of objects. We demonstrate several pick-and-place manipulations common to industrial and laboratory automation settings that are simplified by our design.
 <a href="https://nddoshi.github.io/assets/pdfs/taylor_iros2020.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=dtDefve8KFk" target="_blank"><b> [Video]</b></a>
</p>

<p>
<img src="/assets/img/Seb_EA.png" alt="hamr-ea" style="float:left;width:15%;" hspace="10" />
</p>
<p> <b> Science Robotics 2018: Climbing with a quadrupedal centimeter-scale robot using electroadhesion.</b> We present a centimeter-scale quadrupredal robot with electroadhesive feet. This robot leverages electroadhesion to achieve locomotion on horizontal, vertical, inverted, and curved conductive surfaces, highlighting its unique locomotive flexibility. As a demonstration of its potential for industrial applications, such as in-situ inspection of high-value assets, we show that the robot is capable of achieving open-loop, inverted locomotion inside a curved portion of a commercial jet engine. 
<a href="https://nddoshi.github.io/assets/pdfs/deRivaz_scirob2018.pdf" target="_blank"><b>[Publication]</b></a> 
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
<img src="/assets/img/afm-sarrus.png" alt="sarrus" style="float:right;width:15%;" hspace="25"> 
</p>

<p> <b> AFM 2021: A fabrication strategy for reconfigurable millimeter-scale metamaterials. </b> We use laminate manufacturing to develop a method for designing reconfigurable metamaterials at the millimeter-scale. Our approach is compatible with a wide range of materials and requires minimal manual assembly. We characterize how the use of laminate manufacturing affects the behavior of these multi-component arrays. To this end, a numerical model that captures the deformations exhibited by the structures is developed, and an analytic model that predicts the strain of the structure under compressive stress is built. Overall, this approach can be leveraged to develop millimeter-scale metamaterials for applications that require reconfigurable materials, such as in the design of tunable acoustics, photonic waveguides, and electromagnetic devices
<a href="https://nddoshi.github.io/assets/pdfs/doshi_afm2021.pdf" target="_blank"><b>[Publication]</b></a>

</p>

<p>
<img src="/assets/img/Delta1.png" alt="milldelta" style="float:left;width:20%;" hspace="10"> 
</p>
<p> <b> Science Robotics 2018: The milliDelta. </b> Developing a millimeter-scale Delta robot that maintains the characteristic input-output behavior and operates with high speed and precision requires overcoming manufacturing and actuation challenges. We present the design, fabrication, and characterization of an adapted Delta
robot at the millimeter scale (the “milliDelta”) that leverages printed circuit microelectromechanical system manufacturing techniques and is driven by three independently controlled piezoelectric bending actuators. This robot can operate with precision down to ∼5μm in a 7 mm<sup>3</sup> workspace and can follow periodic trajectories at frequencies up to 75 Hz. The milliDelta can be used for applications such as vibration cancellation in microsurgery and microassembly, or micromanipulation. 
<a href="https://nddoshi.github.io/assets/pdfs/mcclintock_scirob2018.pdf" target="_blank"><b>[Publication]</b></a> 
<a href="https://www.youtube.com/watch?v=rHUnqYDgUFY" 
target="_blank"><b> [Video]</b></a>
</p>

<p>
<img src="/assets/img/sfb.png" alt="hamr-transmission"  style="float:right;width:20%;" hspace="5"> 
</p>

<p> <b> IROS 2015: Model driven design for flexure-based millimeter-scale robots. </b> 

We present a non-linear, dynamic model of the Harvard Ambulatory Microrobot's (HAMR's) flexure-based transmission. The model is derived from first principles and has led to a more comprehensive understanding of the components in this transmission. In particular, an empirically-informed lumped-parameter mechanics-model of the compliant Kapton flexures is developed and verified against theoretical results from beam and vibration theory. The transmission model is used to redesign the transmission for improved performance in this regime. The model based redesign results in a 266%
increase in the work done by the foot when compared to a previous version of HAMR. This leads to a payload capacity of 2.9g, which is ∼ 2× the robot’s mass and a 114% increase. 
<a href="https://nddoshi.github.io/assets/pdfs/doshi_iros2015.pdf" target="_blank"><b>[Publication]</b></a> 
</p>



