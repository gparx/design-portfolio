
# A10 — Lead Screw Design

## Overview
Design a mechanically driven tensile testing machine capable of applying a 2 kN (449.62 lbf) axial load using two lead screws and a movable crosshead.

### Design Specifications

| Parameter | Value |
|---|---|
| Maximum Load | 2,000 N |
| Lead Screws | 2 |
| Load per Screw | 1,000 N (equal sharing) |
| Safety Factor | 4 |
| Crosshead Speed | 1–50 mm/min |
| Minimum Screw Length | 18 in |
| Maximum Crosshead Deflection | 0.10 mm |
| Operation | Mechanical |


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 1. Lead Screw Design (Ethan)

Determine the minimum lead screw diameter, rotational speed range, and required torque.

**FBD & Calculations:**


<img width="1219" height="1105" alt="Screenshot 2026-11-09 214926" src="https://github.com/user-attachments/assets/9046748b-efd4-40d7-bd4d-c9e2e24db4b6" />


<img width="2314" height="945" alt="Screenshot 2026-11-09 214930" src="https://github.com/user-attachments/assets/e2fa4149-091f-440a-8ab9-de280ed58416" />



- Axial Stress: σ = F/A
- Allowable Stress: σ_allow = Sy/N
- Minimum Root Diameter: d_min = √(4FN/πSy)
- Rotational Speed: n = v/lead
- Torque: Calculated using thread geometry and friction.


| Result | Value |
|---|---|
| Minimum Root Diameter | 0.196 in |
| Rotational Speed Range | 0.315 - 15.75 rpm |
| Friction Coeff. | 0.15454 |
| Maximum Torque per Screw | 1.64 N*m |
| Selected Lead Screw | 5/8"-8 316 Stainless Steel Acme Lead Screw |
| Selected Screw Diameter | 0.625 in |


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 2. Nut and Flange Design (Grant)

Select a bronze nut/flange compatible with the chosen lead screw. Verify thread bearing and bending stresses using a safety factor of 4.

**FBD & Calculations:**

<img width="461" height="350" alt="Screenshot 2026-11-09 203015" src="https://github.com/user-attachments/assets/9d094343-8ad7-4adc-a0fc-883a9af019a5" />



- Engaged Threads: nₑ = Lₑ / p

- Thread Bending Stress: σ_bend = 6F / (nₑπdₘp)

- Allowable Stress: σ_allow = Sᵧ / N

- Actual Safety Factor: N_actual = Sᵧ / σ_bend


<img width="750" height="377" alt="Screenshot 2026-11-09 203012" src="https://github.com/user-attachments/assets/d1ca5da8-d5e2-46eb-af89-224e9418eb70" />


| Result | Value |
|---|---|
| Selected Nut/Flange | 932 Bearing Bronze Acme Flange Nut, 5/8"-8 |
| Material | 932 Bearing Bronze |
| Thread Size | 5/8"-8 Acme |
| Thread Engagement | 10 (assumed) |
| Thread Pitch | 0.125 in |
| Mean Diameter | 0.5625 in |
| Thread Root Diameter | 0.645 in |
| Thread Bending Stress | 533 psi |
| Assumed Yield Strength | 14,000 psi |
| Allowable Stress | 3,500 psi |
| Required Safety Factor | 4 |
| Calculated Safety Factor | 26.3 (estimated) |
| Verdict | Preliminary Pass |

- McMaster Flange part was missing yield strength so we used a general 14,000 psi standard yield strength for the material.

<img width="1087" height="329" alt="image" src="https://github.com/user-attachments/assets/2abefb1f-d93f-4570-a572-2c251b8435ae" />

- Holes to be drilled through flange to mount onto crosshead

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 3. Crosshead Design (Grant)

Design the crosshead to support the 2 kN (449.62 lbf) tensile load while maintaining a maximum deflection of 0.10 mm.

### FBD

<img width="743" height="253" alt="Screenshot 2026-11-09 225756" src="https://github.com/user-attachments/assets/ed50efe2-7b52-43f7-97f2-d04a5ded6727" />


### Strength Analysis


| Known | Value |
|---|---|
| Applied Load | 449.62 lbf |
| Support Span | 8 in |
| Beam Width | 2 in |
| Trial Thickness | 1 in |
| Required Safety Factor | 4 |


| Unknowns | 
|---|
| Maximum Bending Moment | 
| Area Moment of Inertia | 
| Maximum Bending Stress | 
| Minimum Required Yield Strength | 
| Actual Safety Factor | 


- Maximum Bending Moment: M = PL/4
- Bending Stress: σ = Mc/I
- Allowable Stress: σ_allow = Sy/N

<img width="934" height="922" alt="Screenshot 2026-11-09 225707" src="https://github.com/user-attachments/assets/a2336076-77e4-4bb0-9822-bb443105408d" />

| Solved | Value |
|---|---|
| Maximum Bending Moment | 899.24 lbf·in |
| Area Moment of Inertia | 0.1667 in⁴ |
| Maximum Bending Stress | 2,698 psi |
| Minimum Required Yield Strength | 10,791 psi |
| Selected Material | 6061-T6 Aluminum |
| Material Yield Strength | 35,000 psi |
| Actual Safety Factor | 14.83 |
| Required Safety Factor | 4 |
| Result | Preliminary Pass |


### Deflection Analysis


| Known | Value |
|---|---|
| Applied Load | 449.62 lbf |
| Support Span | 8 in |
| Beam Width | 2 in |
| Trial Thickness | 1 in |
| Maximum Allowable Deflection | 0.003937 in (0.10 mm) |


| Unknowns |
|---|
| Area Moment of Inertia |
| Minimum Required Elastic Modulus |
| Selected Material |
| Material Elastic Modulus |
| Actual Maximum Deflection |

- Maximum Deflection: δ = FL³/(48EI)
- Deflection Limit: 0.10 mm


<img width="881" height="699" alt="image" src="https://github.com/user-attachments/assets/06150fc8-8e5f-440f-a684-c6063ba7f4ea" />



| Solved | Value |
|---|---|
| Area Moment of Inertia | 0.1667 in⁴ |
| Minimum Required Elastic Modulus | 7.3 × 10⁶ psi |
| Selected Material | 6061-T6 Aluminum |
| Material Elastic Modulus | 10 × 10⁶ psi |
| Actual Maximum Deflection | 0.002878 in (0.0731 mm)|
| Allowable Deflection | 0.003937 in (0.10 mm)|
| Result | Preliminary Pass |




### Preliminary Sketch


<img width="1190" height="916" alt="image" src="https://github.com/user-attachments/assets/1c36eb16-a757-4922-98b2-63b8103956a4" />


- Per Machinery's Handbook pg. 656, locational fit H7 for nominal diameter 0.71-1.19" is +0.0008/-0.0000

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


##  Cost Analysis (Ethan)


<img width="1242" height="555" alt="image" src="https://github.com/user-attachments/assets/cfba52aa-e5d0-4616-bd31-29d5e98db230" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## Parametric CAD Assembly (Bryan)

Model the crosshead parametrically in SolidWorks and assemble the following components:

### Crosshead

- In order: Parametrics -> Sketching & Extrusion -> Holes -> Material Assignment


<img width="523" height="104" alt="2_Global_vars" src="https://github.com/user-attachments/assets/00be718b-77a9-4a9f-8315-164359b1b746" />


<img width="830" height="362" alt="4_CH_Extrusion" src="https://github.com/user-attachments/assets/a34638bb-2f58-47b9-afc8-80c5f97deabf" />


<img width="617" height="227" alt="5_Hole_Sketch" src="https://github.com/user-attachments/assets/51ecf932-8003-401a-a561-9e8e808549a9" />


<img width="691" height="273" alt="8_Bolthole_mirrored" src="https://github.com/user-attachments/assets/a537b291-56ae-4a9a-85b0-2ad74bd67fb5" />


<img width="740" height="283" alt="10_bolthole_feature" src="https://github.com/user-attachments/assets/7760fed9-5455-48a7-bea8-8b41a611c0de" />


<img width="614" height="486" alt="11_Material_Assigned" src="https://github.com/user-attachments/assets/6e066310-92c5-4479-8322-d46fcd8d243f" />


<img width="838" height="583" alt="12_Finished_Part" src="https://github.com/user-attachments/assets/7d55cd1f-7056-48d3-a729-ba8875e733d6" />

---

### Bronze nut/flanges

- In order: Import -> Hole Sketch -> Holes -> Mate w/ Crosshead -> Material Assignment -> 2nd Nut 

<img width="371" height="239" alt="1_Imported_Nut" src="https://github.com/user-attachments/assets/2b945e41-f841-454b-b6d3-95de96f22b2c" />


<img width="440" height="486" alt="2_Hole_Sketch" src="https://github.com/user-attachments/assets/6597f266-a282-4c2a-8f99-fc66cf303ce4" />


<img width="595" height="476" alt="3_HoleWizard" src="https://github.com/user-attachments/assets/10e01b55-7ff9-412d-a00e-9a0d2f5a103e" />


<img width="228" height="286" alt="4_Mated_w_Crosshead" src="https://github.com/user-attachments/assets/cafd0150-3d89-4bf6-8afc-c7758c8ac1ba" />


<img width="614" height="482" alt="5_Assigned_Matl" src="https://github.com/user-attachments/assets/5abf5611-9f2b-410d-bfc5-e734d748c34a" />


<img width="397" height="209" alt="6_Added_2nd_Nut" src="https://github.com/user-attachments/assets/c338b9f9-1f70-4adf-baa2-764d1b55ef32" />


---

### Mounting Bolts


<img width="803" height="586" alt="Imported Mated_bolts" src="https://github.com/user-attachments/assets/bb8b3edc-9d40-44f6-8ef6-b7e50f1b0e75" />


---

### Lead screws

- In order: -> Import Lead Screws -> Cut -> Assemble

<img width="614" height="514" alt="1_Imported_LS" src="https://github.com/user-attachments/assets/4e3300a3-1299-4945-9ea5-5f7a6c489239" />


<img width="881" height="572" alt="2_Cutting_LS" src="https://github.com/user-attachments/assets/1f98f1f6-e9ba-4e36-b971-3bfe25448073" />


<img width="400" height="422" alt="3_Mated_LS+Final assembly" src="https://github.com/user-attachments/assets/5f716647-2699-472a-81ca-51a4518bbbd7" />

---

**Final Assembly:**




---

**CAD Files:**

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## FEA and Optimization (Bryan)

Perform SolidWorks FEA on the crosshead under a 2 kN (449.62 lbf) axial load. Verify mesh convergence and optimize the geometry.

**Boundary Conditions:**
- Load: 2,000 N
- Fixtures: Nut/flange attachment interfaces

| Result | Initial | Refined 1 | Refined 2 | Optimized |
|---|---|---|---|---|
| Elements | ? | ? | ? | ? |
| Max Stress | ? | ? | ? | ? |
| Max Deflection | ? | ? | ? | ? |
| Safety Factor | ? | ? | ? | ? |
| Mass | ? | ? | ? | ? |


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## Engineering Drawing

Create a detailed SolidWorks drawing of the final crosshead using third-angle projection and ASME Y14.5 dimensioning standards.

**General Tolerances:**

- X.X ± 0.02
- X.XX ± 0.01
- X.XXX ± 0.005


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 8. Engineering Lessons Learned (Ethan)

Ethan — Lead Screw Calculations
I completed the lead screw calculations and learned how the screw’s lead determines the rotational speed needed to move the crosshead. For the selected screw, each revolution moves the nut 0.125 inches. Using this value, I calculated the speed range needed to meet the required crosshead movement. I also learned how to use the inclined plane model from class to solve for the force needed to overcome the axial load and friction. Multiplying that force by the pitch radius gave the required torque. Working through the force balances made the torque equation easier to understand. Another thing I learned was to use the thread root diameter when calculating axial stress because this is the smallest section carrying the load.

Grant — Second Calculation Section
I completed the second math section and learned how to connect the free-body diagram to the equations used to size the components. Solving symbolically first helped me understand how changing the load, material strength, or dimensions would affect the result. I also learned how to apply the safety factor of 4 by reducing the allowable stress used in the calculations. The selected hardware also affected the design because the calculated dimensions needed to provide space for the nut and flange mounting features. This helped me understand why the calculations and part selection needed to be considered together.

Bryan — CAD Modeling and Assembly
I completed the CAD modeling and assembly and learned how to create a screw mate in SolidWorks. Setting the travel per revolution connected the rotation of the lead screw to the linear movement of the nut and crosshead. I also learned how to combine mates that kept the components aligned while allowing the intended movement. The screw mate required checking the direction of travel and the amount of movement produced by each revolution. Working with downloaded components also taught me to check the thread size, thread direction, and number of thread starts when selecting compatible parts.

The project took approximately 20 combined hours to complete.

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## References

- MEGR 2157 — A10 Assignment Instructions
- [Acme General Purpose 2G Thread Series Limiting Dimensions & Tolerances](https://www.dependableacme.com/internal-and-external-thread-dimensions)
- [McMaster-Carr](https://www.mcmaster.com/)
- [Lead Screw](https://www.mcmaster.com/97014A320/)
- [Bronze Bearing](https://www.mcmaster.com/95120A119/)
- [Socket Head Screw](https://www.mcmaster.com/92200A151/)
- SolidWorks — CAD and FEA 
