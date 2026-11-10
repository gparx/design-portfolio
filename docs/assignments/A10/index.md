
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


## 1. Lead Screw Design

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


## 2. Nut and Flange Design

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


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 3. Crosshead Design

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


- Maximum Bending Moment: M = FL/4
- Bending Stress: σ = Mc/I
- Allowable Stress: σ_allow = Sy/N

<img width="934" height="922" alt="Screenshot 2026-11-09 225707" src="https://github.com/user-attachments/assets/a2336076-77e4-4bb0-9822-bb443105408d" />



### Deflection Analysis

- Maximum Deflection: δ = FL³/(48EI)
- Deflection Limit: 0.10 mm


| Result | Value |
|---|---|
| Selected Material | ? |
| Crosshead Length | ? |
| Crosshead Width | ? |
| Crosshead Height | ? |
| Maximum Stress | ? |
| Maximum Deflection | ? |
| Safety Factor | ? |

### Preliminary Sketch

<img width="1088" height="565" alt="image" src="https://github.com/user-attachments/assets/3fc9cdf6-8525-4413-a191-64ece2d6840f" />

- Per Machinery's Handbook pg. 656, locational fit H7 for nominal diameter 0.71-1.19" is +0.0008/-0.0000

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 4. FEA and Optimization

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


## 5. Engineering Drawing

Create a detailed SolidWorks drawing of the final crosshead using third-angle projection and ASME Y14.5 dimensioning standards.

**General Tolerances:**

- X.X ± 0.02
- X.XX ± 0.01
- X.XXX ± 0.005


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 6. Cost Analysis

| Item | Quantity | Cost/Item | Total | Purchase Link |
|---|---|---|---|---|
| Lead Screws | 2 | ? | ? | ? |
| Bronze Nut/Flange | 2 | ? | ? | ? |
| Aluminum Frame | ? | ? | ? | ? |
| Other Hardware | ? | ? | ? | ? |
| **Total** | | | **?** | |


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 7. Parametric CAD Assembly

Model the crosshead parametrically in SolidWorks and assemble the following components:

- Designed crosshead
- Two identical lead screws
- Two bronze nut/flanges
- Aluminum T-slot frame

**Final Assembly:**


**CAD Files:**


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## 8. Engineering Lessons Learned


<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">


## References

- MEGR 2157 — A10 Assignment Instructions

- [McMaster-Carr](https://www.mcmaster.com/)
- SolidWorks — CAD and FEA 
