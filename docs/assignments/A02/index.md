# A2 – Truss Stress Analysis



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Project Overview

The overall purpose of this project was to simulate a scaled down version of a real life problem someone might work on. Specifically, the task was to design a light weight planar truss using A500 structural steel which included creating a free body diagram of our design, calculating member forces, resultant forces, minimum cross sectional areas of the steel and pins that could withstand the sheer forces of the truss. Additionally, our assignment guidelines constricted us to only using 1 sheer plane.

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
- Pin connection type: [**Single Sheer**]

<img width="1319" height="448" alt="Screenshot 2026-09-02 192436" src="https://github.com/user-attachments/assets/408c7706-d797-434b-ac8b-def5ecc6aecc" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 2. Truss Design

## 2a. Overall Truss Geometry

### Initial Truss Design

<img width="1290" height="865" alt="Screenshot 2026-09-02 193952" src="https://github.com/user-attachments/assets/7eef4f57-a767-49af-ad2c-ae81190829fe" />

Initially looking at the problem, I didn't know where to start. My initial thought process was to make this as simple as possible while maintaining the standards and quality that I expected from the design. After doing some researching online I became aware of an equation that I had not seen before. **M + R = 2J**, in other words, the number of members + the number of support reactions = 2x the number of joints for a determinately stable truss system. Noticing that this would make my truss even more simple than I imagined, I quicky drew out a fifth member that would help cancel out opposing forces. The geometry of the truss keeps things simple and minimizes the number of members while also bracing the applied upward load (P) towards joint A, creating a triangular truss system. 


<br>

### 2a.i. Member Geometry and Lengths

<img width="1185" height="894" alt="Screenshot 2026-09-02 201208" src="https://github.com/user-attachments/assets/952758c7-f78b-4d4d-bacc-61bd146a2ee3" />


## 2a.ii. Free-Body Diagrams

<img width="1182" height="1290" alt="Screenshot 2026-09-02 201500" src="https://github.com/user-attachments/assets/d2439766-71de-4616-bdb4-cccb6a879854" />


## 2a.iii-iv. Symbolic Internal Force Analysis and Numerical Internal Force Analysis

<img width="1155" height="675" alt="Screenshot 2026-09-02 201558" src="https://github.com/user-attachments/assets/a90f13b2-50bd-43e9-a2da-32ab45d4987d" />


[Explain why the method of joints was used.]

[Explain how the joint equations were solved.]

[Explain what the symbolic analysis determines.]


# 2b. Truss Member Cross-Section Design

## 2b.i. Knowns and Unknowns

<img width="1134" height="751" alt="Screenshot 2026-09-02 202650" src="https://github.com/user-attachments/assets/72a10cfd-866d-4e11-ba68-f90460b79cc8" />


## 2b.ii. Symbolic Cross-Sectional Area Calculation

<img width="825" height="491" alt="Screenshot 2026-09-02 202756" src="https://github.com/user-attachments/assets/03c331fd-1d90-4e73-a6a1-ac1976c459be" />



## 2b.iii. Numerical Cross-Sectional Area

<img width="1118" height="361" alt="Screenshot 2026-09-02 202843" src="https://github.com/user-attachments/assets/92a86e21-6beb-4a81-a557-820b2aa86856" />


## 2b.iv. Approximate Truss Weight

<img width="1135" height="540" alt="Screenshot 2026-09-02 202936" src="https://github.com/user-attachments/assets/98f9b8f5-827b-4dac-b666-384ccdfbffb1" />



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 3. Connecting Pin Design

## 3a. Single-Shear Pin Connection

[Explain why a single-shear model is used.]

[Explain how the critical pin load was determined.]

[Explain what dimensions were determined from the analysis.]

<br><br>

## 3a.i-ii. Knowns and Unknowns & Critical Pin Free-Body Diagram

<img width="1157" height="1158" alt="Screenshot 2026-09-02 205923" src="https://github.com/user-attachments/assets/8719a9ed-69d4-4b8f-8ea3-9b85141c5033" />



## 3a.iii-iv. Symbolic Pin Area Calculation & Numerical Pin Area

<img width="1189" height="391" alt="Screenshot 2026-09-02 210155" src="https://github.com/user-attachments/assets/0999c873-a4bc-4a77-8a14-920c445b42a1" />



## 3a.v. Approximate Combined Pin Weight

<img width="1194" height="1003" alt="Screenshot 2026-09-02 210434" src="https://github.com/user-attachments/assets/54b705e6-4db0-4f53-b3fc-9c4026d4cc3d" />




<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 4. CAD Model and Verification

## 4a. Truss CAD Model


## 4b. Pin Joint Geometry


## 4c. Design Verification


## 4d. CAD Mass Properties



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 5. Engineering Lessons Learned


# Project Files

## CAD Files

**[Download the completed CAD files](TRUSS (2).zip)**

> The downloadable file should include the truss part, pin part, and completed assembly.

<br><br>

# Project Time

| Task | Time |
|---|---:|
| Truss geometry and FBDs | [3 HRS] |
| Analytical calculations | [3 HRS] |
| Pin calculations | [2 HRS] |
| CAD modeling | [2 HRS] |
| CAD assembly and mass properties | [1 HRS] |
| Portfolio documentation | [2 HRS] |
| **Total Time** | **[15 HRS]** |

<br><br>
