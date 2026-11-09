
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
| Minimum Root Diameter | TBD |
| Selected Screw Diameter | TBD |
| Rotational Speed Range | TBD |
| Maximum Torque per Screw | TBD |
| Selected Lead Screw | TBD |

---

## 2. Nut and Flange Design

Select a bronze nut/flange compatible with the chosen lead screw. Verify thread bearing and bending stresses using a safety factor of 4.

**FBD & Calculations:**


| Result | Value |
|---|---|
| Nut Material | Bronze |
| Thread Engagement | TBD |
| Bearing Stress | TBD |
| Thread Bending Stress | TBD |
| Safety Factor | TBD |
| Selected Nut/Flange | TBD |

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
| Selected Material | TBD |
| Crosshead Length | TBD |
| Crosshead Width | TBD |
| Crosshead Height | TBD |
| Maximum Stress | TBD |
| Maximum Deflection | TBD |
| Safety Factor | TBD |

### Preliminary Sketch


---

## 4. FEA and Optimization

Perform SolidWorks FEA on the crosshead under a 2 kN axial load. Verify mesh convergence and optimize the geometry.

**Boundary Conditions:**
- Load: 2,000 N
- Fixtures: Nut/flange attachment interfaces

| Result | Initial | Refined 1 | Refined 2 | Optimized |
|---|---|---|---|---|
| Elements | TBD | TBD | TBD | TBD |
| Max Stress | TBD | TBD | TBD | TBD |
| Max Deflection | TBD | TBD | TBD | TBD |
| Safety Factor | TBD | TBD | TBD | TBD |
| Mass | TBD | TBD | TBD | TBD |


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
| Lead Screws | 2 | TBD | TBD | TBD |
| Bronze Nut/Flange | 2 | TBD | TBD | TBD |
| Aluminum Frame | TBD | TBD | TBD | TBD |
| Other Hardware | TBD | TBD | TBD | TBD |
| **Total** | | | **TBD** | |

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

*Summarize engineering decisions, calculations, material selection, FEA optimization, and assembly challenges.*

---

## References

- MEGR 2157 — A10 Assignment Instructions
- [McMaster-Carr](https://www.mcmaster.com/)
- SolidWorks — CAD and FEA 
