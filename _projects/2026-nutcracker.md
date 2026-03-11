---
layout: project
title: Nutcracker Design
permalink: /projects/2026-nutcracker/
---

**Nutcracker Design**

**Obective:**
Design a simple lever-style nutcracker capable of cracking a macadamia nut using a hand. The objective is to determine the required dimensions of the lever system such that a typical human grip force can generate enough output force to crack the nut. The design should use a simple lever mechanism, be hand operated, and provide sufficient mechanical advantage to crack the nut.

**Constraints and Input Parameters:**
Macadamia nut diameter ≈ 2.5.
Distance from pivot to nut ≈ 2.5 cm.
Typical maximum human grip strength: 𝐹in ≈ 400N. This force is applied equally to both handles so 200N. 
Force required to crack a macadamia nut from literature is 225 kg x 9.8 m/s^2 = 2205N = Fout. 

**Approach:**
To crack the nut, the nutcracker must generate at least 2205N. Using the definition of mechanical advantage: MA = Fout/Fin = 2205N/400N = 5.5. The lever system must provide approximately 5.5× mechanical advantage.

Using moment equilibrium about the pivot:
∑𝑀 = 0 = (200N)(L) = (1102.5N)(2.5cm)
200L=2756.25
L = 13cm

Where L = handle length
1102.5N = half the nut force applied to each side
Therefore the required handle length is approximately 13cm.

**Diagram of nut cracker design:**
Pivot located at the hinge. Nut positioned 2.5 cm from the pivot. Human force applied at the handles. Handle length ≈ 13 cm.

![Nutcracker diagram](/assets/images/nutcracker-diagram.jpg)

**Discussion:**
Although the lever provides the required mechanical advantage, the design presents usability concerns. The calculated handle spacing is 13 cm, which may be too wide for the average human hand to grip comfortably.

**Credits:**
Macadamia nut force data obtained from literature on nut cracking forces. (https://link.springer.com/article/10.1007/s10071-007-0131-2)
