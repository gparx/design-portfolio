# Bracket Design – Stress, Stiffness, and Fits Analysis

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


<img width="1039" height="804" alt="image" src="https://github.com/user-attachments/assets/d34ea6c7-fce7-4203-ba0b-1bd007366ccf" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


<img width="1031" height="568" alt="image" src="https://github.com/user-attachments/assets/4b9c05a1-cc14-4a1f-a63f-4a07e111b268" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">




## Project Overview

### Design Requirements

- Safety Factor: SF = 4
- Maximum Deflection: 0.005 in
- Assume no failure due to direct shear stress.
- Assume shear deflection is negligible.

### Feature Models

- Feature A: Cantilever Beam
- Feature B: Axially Loaded Bar
- Feature C: Simply Supported Beam with Center Load
- Feature D: TBD
- Feature E: TBD


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Stress Analysis


## Feature A

### Knowns:

- Safety Factor: SF = 4
- Maximum Deflection: 0.005 in
- F (chosen) = 600 lbf
- l (chosen) = 3"
- SF = 4
- Elastic Modulus: E = 29,000,000 psi
- Yield Strength: Sy = 36,000 psi
- Sy = 36,000 psi
- σallow = 9,000 psi
- Assume no failure due to direct shear stress.
- Assume shear deflection is negligible.

### Unknowns

- Required Dimensions of Feature A

### Assumptions

- Feature A is a cantilever beam
- A36 steel
- Direct shear failure neglected
- Linear elastic behavior
- Symmetric strap loading

### FBD and Calculations

<img width="1190" height="864" alt="Screenshot 2026-09-23 191444" src="https://github.com/user-attachments/assets/7c0564ec-129d-48b7-9f83-d628a26c659b" />

---

## Feature B

### Knowns:

- P = 2F
- P = 1200 lbf
- SF = 4
- ASTM A36 Steel
- Sy = 36,000 psi
- σallow = Sy / SF
- σallow = 9,000 psi
- b = 1.375 in

### Unknowns:

- Minimum required cross-sectional area, A

- Minimum required thickness, t

### Assumptions:

- Feature B is modeled as an axially loaded bar.
- Load acts through the centroid of the cross-section.
- Bending is neglected.
- Feature B has a rectangular cross-section.
- Direct shear failure is neglected.
- Material remains linear-elastic.

---

### FBD and Calculations

<img width="1178" height="846" alt="Screenshot 2026-09-23 195723" src="https://github.com/user-attachments/assets/ee5c7ae7-0edf-4cd0-82b8-e267ca110a19" />

---

## Feature C

### Knowns:
- P = 1200 lbf
- SF = 4
- Sy = 36,000 psi
- σallow = 9,000 psi
- LC = TBD
- Material = A36 Steel
- T-Beam Geometry:
- a = 0.498 in
- b = 0.9992 in
- F = 600 lbf

### Unknown:
- Required thickness of Feature C

### Assumptions:
- Simply supported beam
- Center point load
- Symmetric loading
- Rectangular constant cross-section
- Ignore direct shear and stress concentrations
- Linear-elastic material

### FBD and Calculations

<img width="1181" height="856" alt="Screenshot 2026-09-23 204407" src="https://github.com/user-attachments/assets/bc3e1a16-8d19-4ce2-9555-380ece255ee4" />

---

## Feature D

### Knowns
RD = 600 lbf
SF = 4
Sy = 36,000 psi
σallow = 9,000 psi
t = 3.0 in

### Unknown
Minimum required thickness of D, d

### Assumption
- Feature D is axially loaded.
- Symmetric loading: each D carries 600 lbf.
- Constant rectangular cross-section.
- Load acts through the centroid.
- Linear-elastic material.
- Stress concentrations are neglected.


### FBD and Calculations

<img width="1187" height="859" alt="Screenshot 2026-09-23 212324" src="https://github.com/user-attachments/assets/d6806844-a4fe-437f-899d-902c793c4557" />

---

## Feature E

### Knowns
- P = 600 lbf
- L = 0.9992 in
- SF = 4
- Sy = 36,000 psi
- σ-allow = 9,000 psi
- t = 3.0 in

### Unknown
Minimum required thickness, e

### Assumptions
- Feature E is modeled as a cantilever beam.
- Each E carries 600 lbf due to symmetry.
- Load is distributed over the contact surface.
- Rectangular constant cross-section.
- Linear-elastic material.
- Direct shear failure is neglected.

### FBD and Calculations

<img width="1183" height="840" alt="Screenshot 2026-09-23 214734" src="https://github.com/user-attachments/assets/45111177-d0a8-4ccf-8179-1d7750ff4681" />


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Stiffness Analysis

**Maximum Allowable Deflection: 0.005 in**

## Feature A

- Safety Factor: SF = 4
- Maximum Deflection: 0.005 in
- F (chosen) = 600 lbf
- l (chosen) = 3"
- SF = 4
- Elastic Modulus: E = 29,000,000 psi
- Yield Strength: Sy = 36,000 psi
- Sy = 36,000 psi
- σallow = 9,000 psi

### Unknowns
- Minimum required radius, r
- Minimum required diameter, d

### Assumptions
- Feature A is modeled as a cantilever beam.
- The strap load is distributed symmetrically along Feature A.
- Feature A has a constant solid circular cross-section.
- Material remains linear-elastic.
- Small-deflection beam theory applies.
- Shear deflection is neglected.


### FBD and Calculations


<img width="1182" height="865" alt="image" src="https://github.com/user-attachments/assets/73a577bf-3d3e-4aef-81b0-7277f6f8426e" />

---

## Feature B

### Knowns:
- P = 1200 lbf
- LB = 1.5 in
- E = 29,000,000 psi
- δallow = 0.005 in

### Unknown:
- Minimum cross-sectional area, A

### Assumptions
- Axially loaded member
- Centric loading
- Constant rectangular cross-section
- Linear-elastic material
- Small deformation
- Neglect bending

### FBD and Calculations

<img width="1187" height="797" alt="Screenshot 2026-09-23 195729" src="https://github.com/user-attachments/assets/b8cbb046-80f9-4675-a89d-d8b159ec6371" />


---

## Feature C

### Knowns
- P = 1200 lbf
- L = 2.4964 in
- E = 29,000,000 psi
- δallow = 0.005 in
- t = 3.0 in

### Unknowns
- Minimum required height, h
- Maximum deflection, δmax

### Assumptions
- Simply supported beam
- Center point load
- Constant rectangular cross-section
- Linear-elastic material
- Small deflection
- Neglect shear deflection

### FBD and Calculations

<img width="1173" height="838" alt="Screenshot 2026-09-23 204410" src="https://github.com/user-attachments/assets/05b94c74-84b1-451c-9582-b99765ca5242" />

---

## Feature D

### Knowns
P = 600 lbf
L = 1.499 in
E = 29,000,000 psi
δallow = 0.005 in
t = 3.0 in

### Unknown
Minimum required thickness, d

### Assumptions
- Feature D is axially loaded.
- Each D carries 600 lbf due to symmetry.
- Constant rectangular cross-section.
- Linear-elastic material.
- Small deformation.
- Neglect bending.

### FBD and Calculations

<img width="1188" height="851" alt="Screenshot 2026-09-23 212328" src="https://github.com/user-attachments/assets/0a6c3919-5d96-4925-a939-716815c422d4" />


---

## Feature E

### Knowns
P = 600 lbf
L = 0.9992 in
E = 29,000,000 psi
δallow = 0.005 in
t = 3.0 in

### Unknown
Minimum required thickness, e

### Assumptions
- Feature E is modeled as a cantilever beam.
- Each E carries 600 lbf due to symmetry.
- Load is distributed across the lip.
- Constant rectangular cross-section.
- Linear-elastic material.
- Small deflection.
- Neglect shear deflection.

### FBD and Calculations

<img width="1177" height="844" alt="Screenshot 2026-09-23 214737" src="https://github.com/user-attachments/assets/1c72ea71-77e1-4e58-bf23-afb9baa80f7a" />

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Final Bracket Dimensions


| Feature | Stress Requirement | Stiffness Requirement | Governing Requirement |
|---------|-------------------:|----------------------:|----------------------|
| A | 1.268 in diameter | 0.869 in diameter | Stress |
| B | 0.097 in thickness | 0.009 in thickness | Stress |
| C | 0.408 in height | 0.221 in height | Stress |
| D | 0.022 in thickness | 0.0021 in thickness | Stress |
| E | 0.258 in thickness | 0.127 in thickness | Stress |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Multiview Sketches

## Stress-Based Design

<img width="1174" height="852" alt="Screenshot 2026-09-23 230818" src="https://github.com/user-attachments/assets/e0d77daf-53f8-4c42-b2fd-5646dd01a233" />

---

## Stiffness-Based Design

<img width="1178" height="856" alt="Screenshot 2026-09-23 230822" src="https://github.com/user-attachments/assets/349d8e7b-9456-4650-8570-85e777029b4d" />

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Linkage and Fits

## Link Design

- Feature A Connection: Running / Sliding Fit
- Second Shaft Diameter: 1.000 in
- Second Shaft Connection: Light Assembly Pressure
- Link Material: ASTM A36 Steel

- ### Knowns

- P = 1200 lbf
- SF = 4
- Sy = 36,000 psi
- E = 29,000,000 psi
- δallow = 0.005 in
- Feature A Diameter = 0.1268 in
- Shaft Diameter = 1.000 in

### Unknowns

- Link Width, w
- Link Thickness, t
- Link Length, L
- Minimum Net Area
- Required Fit Dimensions


### Stress and Deflection Calculations

<img width="1186" height="857" alt="Screenshot 2026-09-24 001420" src="https://github.com/user-attachments/assets/03866224-4bb6-436f-8d50-cbc68c3a0947" />

---

<img width="1184" height="858" alt="Screenshot 2026-09-24 001423" src="https://github.com/user-attachments/assets/308079cb-9ae0-4bc2-a412-bd697ef83115" />

---

## Feature A Fit

**Selected Fit:** TBD

**Manufacturing Method:** TBD

<!-- Insert fit table / calculations here -->


## 1-Inch Shaft Fit

**Selected Fit:** TBD

**Manufacturing Method:** TBD

<!-- Insert fit table / calculations here -->


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Engineering Lessons Learned

## Governing Requirement

- Stress governed all equations.

## Error Propagation

- If calculating the diameter of feature 'A' had error it would mess the design of feature 'B' and so on.

## Assumption Sensitivity

- It was important to assume the loading was symmetrical, otherwise our design could change dramatically.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Time Spent

| Task | Time |
|------|------|
| Stress Analysis |2hr |
| Stiffness Analysis |2hr |
| Fits / Linkage |2hr |
| Sketches |1hr |
| Documentation |1hr |
| **Total** |8hr |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


