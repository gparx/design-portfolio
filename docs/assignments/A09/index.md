
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
| Belt Material | Polyurethane Rubber |
| Pulley Material | Aluminum |
| Belt Yield Strength | 471 psi |
| Shaft Material | AISI 1060 Hardened Steel |
| Minimum Safety Factor | 3 |

---

## 1. Belt Design

Determine the tight-side and loose-side forces, required belt cross-sectional area, and circumference.

**Selected Parameters:** TBD

**Free Body Diagram:**

<img width="736" height="389" alt="Screenshot 2026-11-04 202903" src="https://github.com/user-attachments/assets/d7a9b911-3f40-489d-ad34-15b049f2692f" />

**Calculations:**

- Belt Tension Ratio: F₁ / F₂ ≤ e^(μθ)
- Transmitted Torque: T = (F₁ − F₂) × r
- Minimum Belt Area: A_min = (F₁ × N) / S_y
- Minimum Belt Diameter: d_min = √(4A_min / π)
- Belt Circumference: L = 2C + πD

<img width="846" height="462" alt="Screenshot 2026-11-04 202907" src="https://github.com/user-attachments/assets/3c04a278-f613-4905-8e6e-0a50b8bb553c" />


<img width="1029" height="830" alt="Screenshot 2026-11-04 202912" src="https://github.com/user-attachments/assets/e8626ba2-908b-4245-be99-13976c6f902c" />


| Result | Value |
|---|---|
| Tight-Side Force | 7.20 lbf |
| Loose-Side Force | 2.80 lbf |
| Transmitted Torque | 6.6 lbf*in |
| Minimum Belt Diameter | 0.233 in |
| Required Circumference | 20.2 in |
| Selected McMaster Belt | 1/4" Diameter, 12.25 - 24" |

---

## 2. Shaft Diameter Design

Determine the minimum shaft diameter for the applied torque using AISI 1060 hardened steel.


** FBD & Calculations: **

- Maximum Shear Stress: τ_max = 16T / (πd³)
- Minimum Shaft Diameter: d_min = ∛(16T / (πτ_allow))

<img width="959" height="785" alt="image" src="https://github.com/user-attachments/assets/119555d1-1319-4ddc-ac66-2c03ffe47384" />


| Result | Value |
|---|---|
| Applied Torque | 6.6 lbf*in |
| Allowable Shear Stress | 12667 psi |
| Minimum Diameter | 0.1384 in |
| Selected Diameter | 1/16" (0.1875 in) |

---

## 3. Journal Bearing Design

Size the journal bearings and select a material based on pressure, velocity, and PV limits from *Machinery's Handbook*.

** FBD & Calculations **

- Bearing Pressure: P = W / (Ld)
- Surface Velocity: V = πdn / 12
- PV Rating: PV = P × V


<img width="1174" height="850" alt="Screenshot 2026-11-04 213108" src="https://github.com/user-attachments/assets/875e8ca0-8e51-4708-b8bb-0d5ce991540b" />


| Result | Value |
|---|---|
| Bearing Load | 10 lbf |
| Bearing Length | 0.2356 in |
| Pressure | 53.3 psi |
| Velocity | 73.6 ft/min |
| PV Rating | 50,000 |
| Selected Material | SAE OIL-IMP. SINTERED BRNZE |

---

## 4. Frame Design

Design a frame to support the two pulley shafts while maintaining proper alignment and a center distance of 4–6 inches.

**Selected Material:** TBD

**Frame Dimensions:** TBD

**Structural Analysis:** TBD

**Safety Factor:** TBD

### CAD Assembly


---

## 5. Engineering Lessons Learned


---

## References

- [McMaster-Carr — Round Belts](https://www.mcmaster.com/products/round-belts/round-belts-8/)
- *Machinery's Handbook* — Simple Stresses, p. 217
- *Machinery's Handbook* — Journal Bearings, p. 2440
- DJ Dunn — Pulley Drive Systems
- MEGR 2157 — A09 Assignment Instructions
