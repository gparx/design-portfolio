# A6 – Bracket Drawing (Drawings Part 1)

# Design for Strength and Stiffness II

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Parametric Design

### Design 


<img width="3830" height="2088" alt="Bracket" src="https://github.com/user-attachments/assets/bdf65825-b7f5-429c-840f-5627f9487556" />


### CAD Parameters


<img width="1802" height="893" alt="Parametric_Table" src="https://github.com/user-attachments/assets/be280f60-69c0-4faa-b333-d3742cf46d5e" />


### Design Decisions

- All of my dimensions were driven by stress and my parametric design was modeled around these stress values.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Engineering Drawing

### Multiview Drawing


<img width="2345" height="1812" alt="Screenshot 2026-09-30 011252" src="https://github.com/user-attachments/assets/8ddec6ae-8c8c-4a41-a2e9-307df10d51ea" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Design Process

### Mistakes and Changes

- Several mistakes were made while creating not only the model but the drawing. Solidworks was rounding all of my dimensions, messing up my drawing and my actual model. I had to fix that by going into my model options and extend the amount of decimals available. I also modeled my bracket incorrectly as well, luckily the parametrics made it an easy fix. 

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Reflections

### Introduction

In total I spent roughly around 6-8 hours on this portion of the project. Most of the time spend was learning Solidworks because I am unfamiliar with it and want to improve. Looking up how to add tolerances, coincidental constraints and troubleshooting amounted to the majority of my time. Going into this project was a massive headache because I am also taking solid mechanics alongside this class, so some of the things required were beyond my skillset, regardless, I figured out what the assignment was asking for and how I was going to navigate around it. 

### Part A

Stress drove all of my dimensions, but a basic demonstration can be provided if we examine part 'a' of the bracket (the cylinder). When looking at the bending stress that will be applied to this part, we can come to a basic conclusion (after deriving our equation to d = (32FL / (πσ_allow))^(1/3)) that this force will control our diameter. All that needs to be done to translate this into solidworks (or whatever modeling software you choose) is to make a global variable with this equation and add your values such as F, L, etc. into the parametric table.

### Part B

A Tighter tolerance was applied to the diameter of Feature A because it is a functional mating surface that connects to the link through a sliding fit. The tighter tolerance is necessary to maintain the required clearance and allow the parts to assemble and move properly without interferences.

A Looser tolerance was applied to the 3.0 in overall width of the bracket. This dimension is not critical because small variations in the overall width do not affect the fit or function of the bracket. Using the looser X.X ± 0.02 in tolerance is sufficient.

Applying unnecessarily tight tolerances to non-critical features would increase manufacturing and inspection difficulty and cost without providing a functional benefit.



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## CAD Files

---

[DOWNLOAD CAD AND DWG FILES HERE](https://github.com/user-attachments/files/32840685/BRACKET.zip)

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Topic: Drawings (2157 Students Only)

---

### Parametric Designs 

<img width="1786" height="888" alt="Parametrics_2" src="https://github.com/user-attachments/assets/54056adf-fcb5-4d1c-9833-dc81cf322314" />


<img width="3839" height="2084" alt="Link" src="https://github.com/user-attachments/assets/4a123999-cb12-481d-9cc6-a23d56f22c90" />


### Drawings



### Reflections

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

---


