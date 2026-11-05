
# A09 — Pulley System Design

## Overview
Design a belt-driven pulley system to transmit power between two parallel shafts while maintaining a minimum safety factor of 3.

### Design Specifications

| Parameter | Value |
|---|---|
| Pulley Diameter | 3 in |
| Center Distance | 4–6 in |
| Operating Speed | 1000–2000 rpm |
| Static Belt Tension | 4–6 lbf |
| Belt Material | Polyurethane |
| Belt Yield Strength | 471 psi |
| Shaft Material | AISI 1060 Hardened Steel |
| Minimum Safety Factor | 3 |

---

## 1. Belt Design

Determine the tight-side and loose-side forces, required belt cross-sectional area, and circumference.

**Selected Parameters:** TBD

**Free Body Diagram:**  


**Calculations:**

$$
\frac{F_1}{F_2}\leq e^{\mu\theta}
$$

$$
T=(F_1-F_2)r
$$

$$
A_{min}=\frac{F_1N}{S_y}
$$

$$
d_{min}=\sqrt{\frac{4A_{min}}{\pi}}
$$

$$
L=2C+\pi D
$$

| Result | Value |
|---|---|
| Tight-Side Force | TBD |
| Loose-Side Force | TBD |
| Minimum Belt Diameter | TBD |
| Required Circumference | TBD |
| Selected McMaster Belt | TBD |

---

## 2. Shaft Diameter Design (25%)

Determine the minimum shaft diameter for the applied torque using AISI 1060 hardened steel.

**Free Body Diagram:**  


**Calculations:**

$$
\tau_{max}=\frac{16T}{\pi d^3}
$$

$$
d_{min}=\sqrt[3]{\frac{16T}{\pi\tau_{allow}}}
$$

| Result | Value |
|---|---|
| Applied Torque | TBD |
| Allowable Shear Stress | TBD |
| Minimum Diameter | TBD |
| Selected Diameter | TBD |

---

## 3. Journal Bearing Design 

Size the journal bearings and select a material based on pressure, velocity, and PV limits from *Machinery's Handbook*.

**Free Body Diagram:**  


**Calculations:**

$$
P=\frac{W}{Ld}
$$

$$
V=\frac{\pi dn}{12}
$$

$$
PV=P\times V
$$

| Result | Value |
|---|---|
| Bearing Load | TBD |
| Bearing Length | TBD |
| Pressure | TBD |
| Velocity | TBD |
| PV Rating | TBD |
| Selected Material | TBD |

---

## 4. Frame Design 

Design a frame to support the two pulley shafts while maintaining proper alignment and a center distance of 4–6 inches.

**Selected Material:** TBD

**Frame Dimensions:** TBD

**Structural Analysis:** TBD

**Safety Factor:** TBD

### CAD Assembly
*Insert SolidWorks frame and assembly images.*

---

## 5. Engineering Lessons Learned 

*Summarize specific engineering principles and observations from the completed design.*

---

## References

- [McMaster-Carr — Round Belts](https://www.mcmaster.com/products/round-belts/round-belts-8/)
- *Machinery's Handbook* — Simple Stresses, p. 217
- *Machinery's Handbook* — Journal Bearings, p. 2440
- DJ Dunn — Pulley Drive Systems
- MEGR 2157 — A09 Assignment Instructions

