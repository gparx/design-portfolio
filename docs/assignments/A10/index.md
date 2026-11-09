
# A10 — Lead Screw Design

## Overview
Design a mechanically driven tensile testing machine capable of applying a 2 kN axial load using two lead screws and a movable crosshead.

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

---

## 1. Lead Screw Design

Determine the minimum lead screw diameter, rotational speed range, and required torque.

**FBD & Calculations:**

- Axial Stress: σ = F/A
- Allowable Stress: σ_allow = Sy/N
- Minimum Root Diameter: d_min = √(4FN/πSy)
- Rotational Speed: n = v/lead
- Torque: Calculated using thread geometry and friction.


| Result | Value |
|---|---|
| Minimum Root Diameter | ? |
| Selected Screw Diameter | ? |
| Rotational Speed Range | ? |
| Maximum Torque per Screw | ? |
| Selected Lead Screw | ? |

---

## 2. Nut and Flange Design

Select a bronze nut/flange compatible with the chosen lead screw. Verify thread bearing and bending stresses using a safety factor of 4.

**FBD & Calculations:**


| Result | Value |
|---|---|
| Nut Material | Bronze |
| Thread Engagement | ? |
| Bearing Stress | ? |
| Thread Bending Stress | ? |
| Safety Factor | ? |
| Selected Nut/Flange | ? |

---

## 3. Crosshead Design

Design the crosshead to support the 2 kN tensile load while maintaining a maximum deflection of 0.10 mm.

### Strength Analysis

- Maximum Bending Moment: M = FL/4
- Bending Stress: σ = Mc/I
- Allowable Stress: σ_allow = Sy/N


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


---

## 4. FEA and Optimization

Perform SolidWorks FEA on the crosshead under a 2 kN axial load. Verify mesh convergence and optimize the geometry.

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


---

## 5. Engineering Drawing

Create a detailed SolidWorks drawing of the final crosshead using third-angle projection and ASME Y14.5 dimensioning standards.

**General Tolerances:**
- X.X ± 0.02
- X.XX ± 0.01
- X.XXX ± 0.005


---

## 6. Cost Analysis

| Item | Quantity | Cost/Item | Total | Purchase Link |
|---|---|---|---|---|
| Lead Screws | 2 | ? | ? | ? |
| Bronze Nut/Flange | 2 | ? | ? | ? |
| Aluminum Frame | ? | ? | ? | ? |
| Other Hardware | ? | ? | ? | ? |
| **Total** | | | **?** | |

---

## 7. Parametric CAD Assembly

Model the crosshead parametrically in SolidWorks and assemble the following components:

- Designed crosshead
- Two identical lead screws
- Two bronze nut/flanges
- Aluminum T-slot frame

**Final Assembly:**


**CAD Files:**


---

## 8. Engineering Lessons Learned


---

## References

- MEGR 2157 — A10 Assignment Instructions

- [McMaster-Carr](https://www.mcmaster.com/)
- SolidWorks — CAD and FEA 
