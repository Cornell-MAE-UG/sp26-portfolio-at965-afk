---
layout: project
title: Updated Nutcracker Design
description: Updated design of a lever-style nutcracker for cracking macadamia nuts
technologies: [Mechanical Engineering, Lever Design]
image: /assets/images/nutcracker-updated-diagram.jpg
---

**Nutcracker Design**

**Given:**
Initially, the handles were considered in your nutcracker design to be rigid. Now, assume the nutcracker handles are no longer rigid. In fact, they are now best described as beams which bend due to the combined action of the forces from the nut and from theactuator.  

Macadamia nut diameter ≈ 2.5.  
Distance from pivot to nut ≈ 2.5 cm.  
Typical maximum human grip strength: 𝐹in ≈ 400N. This force is applied equally to both handles so 200N.   
Force required to crack a macadamia nut from literature is 225 kg x 9.8 m/s^2 = 2205N = Fout.   

**Find:**
Consider only the components of these forces transverse to your beam:  
a) Find the location of maximum elastic deflection in your handles. State your
assumptions clearly and describe your analysis.  
b) Choose a “beam” design (cross-section, material) such that the vertical elastic
deflection is below 2% of its length and is the most mass-efficient possible.  
c) Present your final design in an image or drawing.

**Assumptions**
1. Small deflection, "plane sections remain plane"  
2. Pin support as pivot  
3. Free end handles  
4. Uniform cross-section throughout  

**Actuator**
Use PA-MC2 Compact Micro Linear Actuator  

Why?  
Force: up to 249 N, exceeds required 200 N input  
Stroke: 2–8 inches, sufficient to close the nut gap  
At x = 13 cm from pivot  

Material selected: Aluminum (E = 70 GPa, ρ = 2710 kg/m³) and its light!  
Cross-section: Hollow tube   

**Solution**
The nut force is split equally between the two handles, so -1102.5 N   
∑M about pivot = 0: (200)(0.13) - (1102.5)(0.025) - R = 0  
Solve for R  

Pivot reaction R:  x = 0, 902.5 N   
Nut: x = 2.5 cm, 1102.5 N   
Actuator: x = 13 cm, 200 N   

Shear force is constant between applied forces and changes magnitude at x = 2.5 cm (nut) and x = 13 cm (actuator).   

Using beam theory EIy′′=M(x). Integrate twice.   
EI(dy/dx) = (R/2)x^2 − (F_nut/2)(x−0.025)^2 + C_1  
Setting dy/dx = 0: EI(dy/dx) = (R/2)x^2 − (F_nut/2)(x−0.025)^2 + C_1 = 0  
Solve for x, δ_max occurs at x = 4.5cm from pivot (between nut and actuator)  

Deflection limit: δ_max < 0.02 × 0.13 = 2.6 mm   
δ_max < 0.02(0.13) = 0.0026 m  
δ_max = [F a b (L^2 − b^2)^(3/2)] / (9 E I L √3)   
EI ≥ 0.0012 N·m^2   
I ≥ 0.0012 / (70×10^9) = 1.74×10^−11 m^4   
r_o = 0.008 m,  r_i = 0.006 m   

I = (π/4)(0.008^4 − 0.006^4) = 2.20×10^−9 m^4   
EI = (70×10^9)(2.20×10^−9) = 151.8 N·m^2   
151.8 >> 0.0012   
m = 2700 · π(0.008^2 − 0.006^2) · 0.13 = 0.031 kg   

**Diagram of nut cracker design:**
[Nutcracker diagram](../assets/images/nutcracker-updated-diagram.jpg)

**Discussion:**
The actuator removes the sole dependance on grip strength as the input force to crack the nut. But adding any form of electrical component can complicate the design.   

**Credits:**
Macadamia nut force data obtained from literature on nut cracking forces.   (https://link.springer.com/article/10.1007/s10071-007-0131-2)  
Actuators  
(https://www.progressiveautomations.com/collections/linear-actuators)  
