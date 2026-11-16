
# A11 – Motor Selection and Design

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

  A tensile tester is a mechanical testing device used to measure how materials respond to uniaxial tension. It applies a controlled pulling force to a specimen while recording the resulting elongation, allowing engineers to determine properties such as yield strength, ultimate tensile strength, and elongation at break. This data is essential for understanding a material’s mechanical behavior and suitability for design applications. Develop the motorized drive and structural integration for the 2 kN tensile tester, focusing on motor selection, mounting, frame stability, and clamp design. This phase will ensure that the crosshead moves smoothly under controlled torque and speed while maintaining precise load alignment and secure specimen gripping.

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## A10 – Previous Design Specifications


| Parameter | Value |
|---|---|
| Application | Tensile Testing Machine |
| Maximum Load | 2,000 N |
| Load per Lead Screw | 1,000 N |
| Safety Factor | 4 |
| Crosshead Speed | 1–50 mm/min |
| Lead Screws | 2 × McMaster 97014A320 |
| Screw Material | 316 Stainless Steel |
| Screw Thread | 5/8"-8 ACME |
| Screw Length | 18 in |
| Screw Lead | 0.125 in/rev (3.175 mm/rev) |
| Required Screw Speed | 0.315–15.75 RPM |
| Estimated Torque per Screw | 1.63 N·m |
| Assumed Friction Coefficient | 0.15434 |
| Flange Nuts | 2 × McMaster 95120A119 |
| Nut Material | 932 Bearing Bronze |
| Nut Dimensions | Ø0.875 in body, Ø1.50 in flange, 1.25 in height |
| Crosshead Material | 6061-T6 Aluminum |
| Crosshead Dimensions | 10 × 2 × 1 in |
| Screw Center Spacing | 8 in |
| Max Allowable Deflection | 0.10 mm |
| Frame | 80 × 40 mm, 40-Series Aluminum T-Slot |
| Frame Connectors | 12 Corner Brackets, 24 M8 Fasteners |
| A10 Component Cost | $867.92 |

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 1. Motor Selection ( Grant )
### Knowns and Unknowns

| Known Parameter | Value |
|---|---|
| Maximum Tensile Load | 2,000 N |
| Number of Lead Screws | 2 |
| Load per Screw | 1,000 N |
| Screw Lead | 3.175 mm/rev |
| Required Screw Speed | 0.315–15.75 RPM |
| Estimated Torque per Screw | 1.63 N·m |
| Required Safety Factor | 4 |

| Unknown Parameter |
|---|
| Required Motor Design Torque |
| Required Mechanical Power |
| Selected Motor Type and Model |
| Motor Rated Speed and Torque |
| Motor Voltage, Current, and Efficiency |
| Motor Shaft and Mounting Dimensions |

### Motor Specifications

---

<img width="1189" height="872" alt="Screenshot 2026-11-15 202610" src="https://github.com/user-attachments/assets/bc43ce39-51bb-45c9-8689-d7b2248493a4" />

---

<img width="2253" height="1251" alt="Screenshot 2026-11-15 204252" src="https://github.com/user-attachments/assets/73632a73-c579-4a13-8289-0a54134c1c04" />

---

- Stepper motors provide high torque and lower speeds with incremental control. This is precisely what we are looking for if were trying to apply a lot of torque to a lead screw to add tensile stress to a material.

---

<img width="1817" height="1200" alt="Screenshot 2026-11-15 204330" src="https://github.com/user-attachments/assets/b4ea8b1d-18fe-40a3-b631-a7cf7da46c11" />
[LINK TO MOTOR HERE](https://www.omc-stepperonline.com/nema-23-stepper-motor-l-76mm-gear-ratio-10-1-mg-series-planetary-gearbox-23hs30-2904s-mg10)

---

### Torque and Speed Verification

---

<img width="1086" height="664" alt="Screenshot 2026-11-15 212300" src="https://github.com/user-attachments/assets/7b489af2-0911-4a76-b6d7-eb18353ec272" />

---

### Speed–Torque Curve

---

<img width="2292" height="928" alt="image" src="https://github.com/user-attachments/assets/6cc70370-9e32-4da8-b8d8-d8591976994f" />

---



---
### Selected Motor

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 2. Motor Mount Design
### Knowns and Unknowns
### Free Body Diagram
### Bearing Stress Analysis
### Minimum Bracket Thickness
### Selected Dimensions and Material

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 3. Coupler Design
### Knowns and Unknowns
### Free Body Diagram
### Torsional Shear Stress Analysis
### Coupler Wall Thickness
### Selected Coupler

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 4. Frame Connection Design
### Knowns and Unknowns
### Free Body Diagram
### Force and Moment Analysis
### Connector Stress Analysis
### Selected T-Slot Connectors

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 5. Top Frame FEA
### Model Setup
### Design 1
#### Mesh 1
#### Mesh 2
#### Mesh 3
### Mesh Convergence
### Safety Factor
### Optimization

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 6. Vertical Frame FEA
### Model Setup
### Design 1
#### Mesh 1
#### Mesh 2
#### Mesh 3
### Mesh Convergence
### Safety Factor
### Optimization

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 7. Floating Bearing Mount
### Knowns and Unknowns
### Bearing and Fit Selection
### Mount Dimensions
### Clearance Holes and Tolerances
### Final Design

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 8. Bill of Materials and Labor Costs
### Bill of Materials
### Engineering Labor
### Total Project Cost

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 9. Engineering Lessons Learned

## Engineering Drawings
### Motor Mount
### Coupler
### Frame Components
### Floating Bearing Mount
### Crosshead (A10)
### Assembly Drawing

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">
