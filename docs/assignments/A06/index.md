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


<img width="1879" height="1452" alt="Screenshot 2026-09-30 003900" src="https://github.com/user-attachments/assets/0b68be61-08c3-4738-8d35-d967d79a9cc8" />


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



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## CAD Files







[Download CAD Files](LINK-HERE)
