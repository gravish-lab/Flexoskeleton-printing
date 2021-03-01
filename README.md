<p align="center">


<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/ezgif-6-e2f3607475d6.gif width="120%">
 <i class="fa fa-sliders" /> A quadrupedal walking robot with flexoskeleton printed limbs</i>

</p>






# Flexoskeleton-Printing
## Overview of flexoskeleton printing

3D printing soft and flexible components typically involves using soft fillaments. Here we demonstrate an alternate method of 3D printing soft and flexible robots which uses rigid filament but printed atop a flexible laminate, as we call **"flexoskeleton printing"**. This method enables easy and rapid printing of flexible structures. The flexoskeleton printing process has the following advantages over typical multi-material printing:
1. Low-cost: this process can be performed on any fused-deoposition method 3D printer with a heated bed. We typically use the Prusa MK3S printers. 
2. Precision mechanical properties: Since the stiffness is controlled by layer thickness and geometry, flexure properties can be precisely controlled and gradients and heterogeneous stiffnesses embedded. 
3. Precision layout of joints/links in a robot: A flexoskeleton robot can be printed as a single monolithic entity. The printed material can define links and joints which produces functional, articulated components without any manual assembly. 
4. Precision curvature estimation: The curvature of the flexoskeleton when jammed can be estimated from parameters of mushroom array thanks to the simple geometry of flexoskeleton.
5. Structural support for silicone casing: The mushrooms give structural support for silicone casing, which can increase overall stiffness of flexoskeleton, seal it from water, and provide smooth surface. 

This process is based on the modification of consumer grade [fused deposition material (FDM) 3D printers](https://en.wikipedia.org/wiki/Fused_filament_fabrication) to extrude rigid FDM filaments (e.g. ABS/PLA) directly onto a flexible yet inextensible thermoplastic backing layer (PC, Polycarbonate). Upon deposition, the two materials form strong and instant bonding based on properly tuned heatbed temperature and initial Z-level of the nozzle. This method significantly improves the fatigue resistance and large-angle bendability of printed components and enables a class of insect-inspired robot morphologies, such as joint limits based on jamming and interlocking of rigid [mushrooms](https:cite). 

## Instructions on flexoskeleton printing

Flexoskeleton printing is based on direct deposition of traditional FDM filaments (e.g. ABS/PLA) onto a flexible yet inextensible backing film (e.g. PC, Polycarbonate). It combines the design concepts from lamination with 


### Fabrication steps

<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/fabrication%20steps.PNG width="120%">

<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/pre_preparation.gif width="50%"><img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/printing1.gif width="50%"> 

The picture above shows the basic farbication steps of flexoskeleton printing. First, we place and secure a thin piece of Polycarbonate film (5mils/10mils) onto the heatbed by applying glues (washable gluesticks) on one side of the PC film. We use rollers to further flatten out the film while preheating the heatbed to a high temperature (80°C—100°C). We then adjust the Z-level to have a nice compressed print line on the PC film as the print starts. During the printing process, one can simply pause the print and place (insert) any additional components such as electronic (resistors, transistors, switch), or structure components (springs, superelastic nitinol fibers) into the printed structures to expand the functionalities of the final prints. As the print finishes, we wait about 3—5 minutes for the part to cool and peel the whole layer off the bed manually. The last step is about releasing the final project from the backing layer by trimming the extra PC films using either scissors, or automatically by laser or vinyl cutting. 

<p align="center">
  
<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/printing2.gif width="60%">

</p>

### Components needed

Basic fabrication tools and materials needed: 

a. [A commercial FDM 3D printer with heatedbed.](https://www.prusa3d.com/original-prusa-i3-mk3/)

b. [Thermoplastic backing layer (Polycarbonate, PC)](https://www.mcmaster.com/polycarbonate/clear-impact-resistant-polycarbonate-film/)

c. [Standard PLA filament](https://www.amazon.com/HATCHBOX-3D-Filament-Dimensional-Accuracy/dp/B00J0GMMP6/ref=sr_1_5?dchild=1&keywords=pla+filament&qid=1600810806&sr=8-5)

c. [Washable glue stick](https://www.amazon.com/Elmers-Washable-All-Purpose-School-E556/dp/B0160P6XK4/ref=sr_1_6?dchild=1&keywords=glue+stick&qid=1613066825&sr=8-6)


### Thermal bonding 

Bonding between the rigid filament (PLA/ABS) and the backing layer (PC) is achieved based on the [thermal bonding effect](https://www.sciencedirect.com/science/article/pii/S0257897216312786) between different thermoplastic materials. High bonding strength is a product of high pressure and temperature between the thermoplastic interface. To do so, we adjust the nozzle to start at within 0.1mm above the backing layer. The heatbed is heated up to 80°C—100°C, with the nozzle around 200°C—220°C (depending on the materials you are printing). The picture on the left shows the first layer print quality with different Z-level of the printhead nozzle, with the right one showing a flexoskeleton printed knob can hold a heavy weight (7.5lbs) without delamination. Note that perfect nozzle height should provide a slightly compressed first layer print, leading to high material bonding.

<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/good%20thermal%20bonding.PNG width="120%">

### "Mushroom" designs

The "mushroom" designs are printed jammable structures that can stiffen the flexoskeleton printed flexure upon reaching the joint limit. Using mushrooms, one can predict the locked up curvature of the hinge between each two mushrooms, and thus the whole bendable curvature. 

There are two main types of "mushroom" designs:

A. Straight mushrooms as flexion joint limits. 



The jammed geometry of two mushrooms gives,

<p align="center">
 
<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/equation.gif width="15%">
 
</p>
 
Applying this simple equation to the straght mushroom array, the jamming curvature of the flexoskeleton structure can be predicted. In reverse, parameters of each mushroom can be designed before fabrication to match final jamming curvature to a prescribed curve, knowing only the function defining the curve. A few flexoskeleton structures that are designed to fit prescibed functions are shown below:


<p align="center">
 
<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/curf_surf.png width="100%">
 
</p>

B. Reverse mushrooms that locks up when the joints are flexed. 


<img src=https://github.com/jason12333/Flexoskeleton-Printing/blob/master/images/extension%20joint.PNG width="120%">

### 

## Gallery of flexoskeleton components

This folder shows a library of different flexoskeleton designs and objects. 

### A. Flexibility demonstration of flexoskeleton
When using backing layer of thickness within 0.8mm, we observe great durability and flexibility of the flexoskeleton.

<p align="center">

<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/flexible_example.gif width="60%">

</p>

### B. Tentacle grasping achieved by slant ridges
We observe slant "ridges" confine curving axis of flexoskeleton into a tilted angle, and the resulting curvature of flexoskeleton looks like octopus tentacle and is able to grasp thin objects:

<p align="center">

<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/curling.gif width="50%"><img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/grasping.gif width="50%">

</p>

## Flexoskeleton related projects

### A. Nonlinear hysteretic buckling joint

### B. Flexoskeleton fingers

With a few additional features, the flexoskeleton structure can be used to make up finger on a soft gripper. As shown below, a flexoskeleton finger with no mushroom on top is encased in a silicone shell; a tendon is routed through hole on each ridge on the flexoskeleton structure to actuate the finger. 

To design a two-finger underactuated soft gripper using this finger, Two flexoskeleton finger is mounted onto a chassis, where tendons through ridges of two flexoskeleton fingers are connected together and pass through a pulley. The pulley is connected to another tendon, which actuate two fingers. This makes up a normal (default) gripper with flexoskeleton fingers; its rendered form is presented below.

This default gripper demonstrates a good graspability for a wide range of objects, thanks to the underactuation mechanism as well as the soft continuum body of flexoskeleton finger. A few application examples of object grasping in free space is shown below.

Atop this default design, two reconfiguring mechanisms are incorporated and shown below.

#### 1) Variable Stiffness Sliding Layer Mechanism

Due to the underactuation mechanism we use on the default gripper, we observe that the gripper equiping two flexoskeleton finger with significantly different thickness of PLA backing layer shows a overlapping grip, as shown below:

<p align="center">
 
<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/sliding_layer.gif width="80%">

</p>

However, we observe an over-curved tip on the finger with thinner backing layer. This is due to the lack of mushroom that provide joint limit.
Inspired by this newly discovered grasping mode, we design a sliding layer that can slide freely through both fingers. This sliding layer also has flexoskeleton structure, with backing layer thickness of 0.8mm and teeth on it in order to mesh with gear on a servo motor. The rendered and actual view of this gripper is shown below. The straight mushroom is also added on both fingers to prevent over-curved tip.

As a result of this sliding layer mechanism, the overall stiffness of each flexoskeleton finger can be controlled by the length of sliding layer inserted. As shown above, when the sliding layer occupies 100% of space in one finger, the other finger has 0% space occupied, so the stiffness difference between two fingers reaches a maximum; if the sliding layer occupies 50% of space in one finger, the other finger also has 50% space occupied, meaning the stiffness difference goes to zero. Consequently, this reconfigurable gripper is able to achieve two grasping modes -- symmetric grasp when stiffness difference is zero and overlapping grasp when stiffness difference is at maximum.


#### 2) Hyperextension Motion and Ridge Locking Mechanism

The flexoskeleton finger can also be installed onto the chassis inversely, meaning the ridges face outward. As a result, the pulling of tendon that goes through ridges would open up the finger instead of closing it up. To accomodate this design, a pre-curved silicone shell is cast to ensure a curved finger when unactuated. This accomplishes a hyperextension motion, where the gripper is able to close and grasp object when unactuated, and release object when actuated.

However, the lifting force generated by this gripper is low compared to previous grippers, since it comes entirely from the silicone shell. To amend this, we introduce a locking mechanism, as shown below. The mushroom on each ridge of flexoskeleton finger has the change of inclined ellipse, and another flexoskeleton with same elliptical mushroom is used as the slider in the finger. Two tendons control this slider, which "locks" with finger when it is pulled up, and "unlocks" when it is pulled down. This elliptical shape of mushroom transforms transversal motion into longitudinal motion, so the slider is able to lock with finger inside the silicone shell. A grasping demo is shown below.

<p align="center">
 
<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/locking_demo.gif width="80%">

<img src=https://github.com/gravish-lab/Flexoskeleton-printing/blob/master/images/locking.gif width="120%">

</p>
