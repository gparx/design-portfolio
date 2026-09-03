# A2 – Truss Stress Analysis



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Project Overview

The overall purpose of this project was to simulate a scaled down version of a real life problem someone might work on. Specifically, the task was to design a light weight planar truss using A500 structural steel which included creating a free body diagram of our design, calculating member forces, resultant forces, minimum cross sectional areas of the steel and pins that could withstand the shear forces of the truss. Additionally, our assignment guidelines constricted us to only using 1 shear plane.

General Steps for this project includes:

- Choosing a truss design and load
- Create free body diagram
- Solve unknown forces and values
- Identify critical member
- Solve for member cross sectional area
- Create pin, solve for pin unknowns
- Translate information into CAD model
- Compare Values
- Sanity Check


<br>

### Design Constraints

- Applied load \(P\): [**20kN**]
- Dimension \(a\): [**0.4m**]
- Dimension \(b\): [**0.3m**]
- Truss material: [**A500 Steel**]
- Member cross-sectional geometry: [**Square**]
- Member safety factor: [**3.5**]
- Pin material: [**Hardened Tool Steel**]
- Pin safety factor: [**4**]
- Pin connection type: [**Single Shear**]

<img width="1319" height="448" alt="Screenshot 2026-09-02 192436" src="https://github.com/user-attachments/assets/408c7706-d797-434b-ac8b-def5ecc6aecc" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 2. Truss Design

## 2a. Overall Truss Geometry

### Initial Truss Design

<img width="1290" height="865" alt="Screenshot 2026-09-02 193952" src="https://github.com/user-attachments/assets/7eef4f57-a767-49af-ad2c-ae81190829fe" />

Initially looking at the problem, I didn't know where to start. My initial thought process was to make this as simple as possible while maintaining the standards and quality that I expected from the design. After doing some researching online I became aware of an equation that I had not seen before. **M + R = 2J**, in other words, the number of members + the number of support reactions = 2x the number of joints for a determinately stable truss system. Noticing that this would make my truss even more simple than I imagined, I quicky drew out a fifth member that would help cancel out opposing forces. The geometry of the truss keeps things simple and minimizes the number of members while also bracing the applied upward load (P) towards joint A, creating a triangular truss system. 


<br>

### 2a.i. Member Geometry and Lengths

Using locations of joints and general dimensions we can calculate all the member lengths and directions.

<img width="1185" height="894" alt="Screenshot 2026-09-02 201208" src="https://github.com/user-attachments/assets/952758c7-f78b-4d4d-bacc-61bd146a2ee3" />


## 2a.ii. Free-Body Diagrams

For each joint I quickly sketched a small free body diagram using the sectioning and joint methods to help calculate member and resultant forces.

<img width="1182" height="1290" alt="Screenshot 2026-09-02 201500" src="https://github.com/user-attachments/assets/d2439766-71de-4616-bdb4-cccb6a879854" />


## 2a.iii-iv. Symbolic Internal Force Analysis and Numerical Internal Force Analysis

Using our given information such as 'a, b, P', we can symbolically solve for member forces.


<img width="1155" height="675" alt="Screenshot 2026-09-02 201558" src="https://github.com/user-attachments/assets/a90f13b2-50bd-43e9-a2da-32ab45d4987d" />



# 2b. Truss Member Cross-Section Design

The truss members needed enough cross-sectional area to withstand the maximum calculated internal force without yielding. My general thought process was to make its form rectangular/square to simplify things. Safety factor and yield strength must be accounted for here.

## 2b.i. Knowns and Unknowns

We know our member lengths, member forces, density of the metal, the safety factor, the maximum force and the yield strength. What we need to solve for is the minimum area and the weight associated with the truss.

<img width="1134" height="751" alt="Screenshot 2026-09-02 202650" src="https://github.com/user-attachments/assets/72a10cfd-866d-4e11-ba68-f90460b79cc8" />



## 2b.ii. Symbolic Cross-Sectional Area Calculation

Using our stress equation we can symbolically solve for he minimum area with some substitutions and relationships between the allowable stress and normal stress.

<img width="825" height="491" alt="Screenshot 2026-09-02 202756" src="https://github.com/user-attachments/assets/03c331fd-1d90-4e73-a6a1-ac1976c459be" />



## 2b.iii. Numerical Cross-Sectional Area

After creating our equation for the minimum cross-sectional area we can plug in our numbers.

<img width="1118" height="361" alt="Screenshot 2026-09-02 202843" src="https://github.com/user-attachments/assets/92a86e21-6beb-4a81-a557-820b2aa86856" />


## 2b.iv. Approximate Truss Weight

Now that I know the cross-sectional area I can solve for the truss weight using volume, density and weight formulas. 

<img width="1135" height="540" alt="Screenshot 2026-09-02 202936" src="https://github.com/user-attachments/assets/98f9b8f5-827b-4dac-b666-384ccdfbffb1" />



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 3. Connecting Pin Design

## 3a. Single-Shear Pin Connection

With confusion settling in, I mistakenly assumed that the force causing shear on the pin was the greatest member force. Eventually I realized that I needed to take all the resultant forces into account when generating the shear forces on it. The initial incorrect calculation was the 37.97kN max. force, after recalculating I arrived at the answer of it equalling the opposing P force that I chose.

<br><br>

## 3a.i-ii. Knowns and Unknowns & Critical Pin Free-Body Diagram


<img width="1157" height="1158" alt="Screenshot 2026-09-02 205923" src="https://github.com/user-attachments/assets/8719a9ed-69d4-4b8f-8ea3-9b85141c5033" />



## 3a.iii-iv. Symbolic Pin Area Calculation & Numerical Pin Area

Here I solved for the minimum pin area using the safety factor (4) and our yield strength (Ty)

<img width="1189" height="391" alt="Screenshot 2026-09-02 210155" src="https://github.com/user-attachments/assets/0999c873-a4bc-4a77-8a14-920c445b42a1" />



## 3a.v. Approximate Combined Pin Weight

The pin weight and length are large estimates due to unknown variables that we aren't accounting for here such as nuts, washers and the mounting technique that will fasten the members. Here I estimated the length of the pins to be 2x the member width so they can at least fit two members on it at minimum.

<img width="1194" height="1003" alt="Screenshot 2026-09-02 210434" src="https://github.com/user-attachments/assets/54b705e6-4db0-4f53-b3fc-9c4026d4cc3d" />




<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 4. CAD Model and Verification

After all my calculations and estimates were finishing it was time to create the model in my chosen software, CREO. There is no specific reason I chose this software other than it's the most recent one I have used and I am more familiar with it. My plan was to simply sketch out the truss and pin, extrude them, change their properties and then run the simulations on their properties.

## 4a. Truss CAD Model

Initial Sketching

<img width="3839" height="2159" alt="Screenshot 2026-09-01 224424" src="https://github.com/user-attachments/assets/af115dca-020a-40c3-8e64-820da9cb0d71" />



Then Extruding

<img width="3783" height="2159" alt="Screenshot 2026-09-01 230049" src="https://github.com/user-attachments/assets/5301cae5-04e3-4987-b956-38e1faee23be" />



## 4b. Pin Joint Geometry

Creation of the pin

<img width="3839" height="2159" alt="Screenshot 2026-09-01 232534" src="https://github.com/user-attachments/assets/01b3ce4a-06af-4136-9113-01dcde1a2125" />



Combining with the truss

<img width="2218" height="1701" alt="Screenshot 2026-09-01 233454" src="https://github.com/user-attachments/assets/2d78fc3d-d478-44e7-a5d1-12849b0e543a" />



Finished.

<img width="3839" height="2159" alt="Screenshot 2026-09-01 234820" src="https://github.com/user-attachments/assets/f2ff6a3e-0098-4a24-9ff2-61b95327d64d" />


## 4c-d. Design Verification / CAD Mass Properties

Now the easy part, running the property simulation after changing the material. 

<img width="3820" height="2155" alt="Screenshot 2026-09-01 235344" src="https://github.com/user-attachments/assets/f590bd07-3c2d-4d0e-ba50-f33237529abc" />


**Hand Calculations vs. CAD Results**

*Hand-calculated truss mass: 11.44 kg*

*Estimated combined pin mass: 0.087 kg*

*Hand-calculated total mass: 11.53 kg*

CAD total mass: 11.23 kg

Difference in mass: 0.30 kg

Percent difference: 2.6%

*Hand-calculated total weight: ≈ 113.1 N*

CAD total weight: 110.1 N

Difference in weight: ≈ 3.0 N

*Hand-calculated total weight: ≈ 25.42 lb*

CAD total weight: 24.75 lb



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 5. Engineering Lessons Learned

I first want to clarify that there are many things that I learned from this assignment, one of which is the importance of a team to speed the engineering process up and build off of each others' critical thinking. To be more specific though, in this assignment I learned how to create a truss and solve for the internal forces of that truss. Once you solve for internal forces based on external forces and reaction forces you can begin to calculate the cross-sectional areas and the support features (pins). Additionally, I learned how to simulate materials on parts/systems in CAD to get information like mass and weight.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Project Files

## CAD Files

**[Download the completed CAD files](TRUSS (2).zip)**

> The downloadable file should include the truss part, pin part, and completed assembly.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Likelihood of Failure Modes in Truss Components


## Part 1 – Truss Members

## Member AB
- Expected failure mode: [YIELDING]
- Material behavior: [DUCTILE]
- Reasoning: [MEMBER IN TENSION]
- Design modification: [INCREASE CROSS-SECTIONAL AREA]

<hr>

## Member BC
- Expected failure mode: [BUCKLING]
- Material behavior: [DUCTILE]
- Reasoning: [MEMBER IN COMPRESSION]
- Design modification: [INCREASE CROSS-SECTIONAL AREA]

<hr>

## Member CD
- Expected failure mode: [YIELDING]
- Material behavior: [DUCTILE]
- Reasoning: [MEMBER IN TENSION]
- Design modification: [INCREASE CROSS-SECTIONAL AREA]

<hr>

## Member DA
- Expected failure mode: [YIELDING]
- Material behavior: [DUCTILE]
- Reasoning: [MEMBER IN TENSION]
- Design modification: [INCREASE CROSS-SECTIONAL AREA]

<hr>

## Member CA
- Expected failure mode: [BUCKLING]
- Material behavior: [DUCTILE]
- Reasoning: [MEMBER IN COMPRESSION & CLOSE TO BUCKLING LIMIT]
- Design modification: [INCREASE CROSS-SECTIONAL AREA]

<hr>

# Part 2 – Pin Connections

## Expected Failure Mode
- Failure mode: [ ]

## Supporting Data
- Shear stress: [ ]
- Shear yield strength: [ ]
- Safety factor: [ ]

## Reasoning
[ ]

## Design Modification
[ ]

## Sources
1. [https://www.altitube.com/en/products/astm-a500/]
2. [https://en.wikipedia.org/wiki/Yield_(engineering)]
3. [https://en.wikipedia.org/wiki/Euler%27s_critical_load]

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# Project Time

| Task | Time |
|---|---:|
| Truss geometry and FBDs | [3 HRS] |
| Analytical calculations | [3 HRS] |
| Pin calculations | [2 HRS] |
| CAD modeling | [2 HRS] |
| CAD assembly and mass properties | [1 HRS] |
| Portfolio documentation | [4 HRS] |
| **Total Time** | **[15+ HRS]** |

<br><br>
