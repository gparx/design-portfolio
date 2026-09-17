# A4 – Motor Mount Design

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Project Overview

Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations)

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

<img width="1518" height="500" alt="Screenshot 2026-09-16 190411" src="https://github.com/user-attachments/assets/a21422cd-c0f7-40b3-a928-095ebc9dbaa1" />

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

<img width="1674" height="809" alt="image" src="https://github.com/user-attachments/assets/1956b87e-9e8e-40d0-86db-174419d83cea" />

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 1. Feature 1 – Motor Attachment

### a) Knowns and Unknowns

**Knowns**

- P = 300N
- SF = 3
- δmax​ = 0.30 mm (Deflection)
- Applied Load: M = PL
- Material = (ABS)
- E ≈ 2.0 GPa = 2000 MPa
- σy​ ≈ 40 MPa
- σallow​ = 40/3 = 13.3 MPa​
- Motor Diameter = 28mm
- Chosen Length (L) = 45mm

---
**Unknowns**

- Feature width (b) = *?*
- Feature thickness (h) = *?*
- Feature cross-sectional geometry = *?*

### b) FBD

<img width="1148" height="841" alt="Screenshot 2026-09-16 205045" src="https://github.com/user-attachments/assets/6fa3c16c-e018-4b31-934f-a1a19c114136" />


### c) Modeling Equations

---

<img width="1175" height="845" alt="Screenshot 2026-09-16 205145" src="https://github.com/user-attachments/assets/4e39d084-6aa2-4fdb-8f7a-035b0ed07733" />

---

<img width="1169" height="657" alt="Screenshot 2026-09-16 205346" src="https://github.com/user-attachments/assets/64fe241d-1a25-45c6-b972-cc58cf2256e4" />

---
### d) C.S. Geometry

As you can see hstress​ = 11.62mm and hdeflection ​= 18.25mm. From this we use the largest value from the two, hdeflection ​= 18.25 mm and we'll just round up to 20mm so our numbers come out nicely. Now we have something that looks like 45mm x 45mm x 20mm (LxWxH). The cross-section is just 45mmx20mm, so 900mm^2.

- b = 45mm
- h = 20mm
- csa = 900mm^2

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 2. Feature 2 – Wall Attachment

---

### a) Knowns and Unknowns

**Knowns**

- Applied force: P = 300 N
- Applied moment: M = PL = 13,500 N·mm
- Factor of Safety: FS = 3
- Maximum allowable deflection: 0.30 mm
- Material: ABS
- Young's Modulus: E = 2000 MPa
- Yield Strength: σy = 40 MPa
- Selected width: b = 45 mm
- Free bending length: L₂ = 45 mm

---

**Unknowns**

- Required thickness, t₂
- Required cross-sectional geometry

---

### b) FBD

---

<img width="1153" height="582" alt="Screenshot 2026-09-16 220347" src="https://github.com/user-attachments/assets/58e61e1d-848f-412c-b568-54b7d86c9536" />

---

### c) Modeling Equations 

---

<img width="1178" height="649" alt="Screenshot 2026-09-16 220354" src="https://github.com/user-attachments/assets/f5d314b7-56e3-433e-8144-12f43416bddb" />

---

<img width="1142" height="611" alt="Screenshot 2026-09-16 220400" src="https://github.com/user-attachments/assets/443257c0-0415-43e7-bc2c-7948795c556a" />

---


### d) C.S. Geometry

- The deflection thickness is greater and take over with a value of 18.25mm, we can round up to 20mm for consistency. This makes our cross-sectional area = 45mm x 20mm = 900mm^2
- **NOTE: THIS IS ONLY THE PORTION FREE TO BEND**


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 3. Motor Mount Sketch

---

<img width="1194" height="673" alt="Screenshot 2026-09-16 231004" src="https://github.com/user-attachments/assets/16254cf2-25e2-4e13-b0f2-6d1355213763" />

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 4. CAD Model

---

<img width="2786" height="1545" alt="Screenshot 2026-09-16 231143" src="https://github.com/user-attachments/assets/0ab625d6-a98a-4bfc-ac64-6310813c3a75" />

---

<img width="1938" height="1369" alt="Screenshot 2026-09-16 233702" src="https://github.com/user-attachments/assets/15fe6816-e39e-45f5-8b86-a0f3f08ac117" />

---

<img width="2770" height="1581" alt="Screenshot 2026-09-16 234348" src="https://github.com/user-attachments/assets/a07d8346-a7b0-403f-9c9b-2f87cc36386b" />

---


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 5. Engineering Drawing


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## 6. Engineering Lessons Learned


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Project Files

### CAD Files

[Download Motor Mount CAD File](docs/assignments/A04/A4_Motor_Mount.zip)

### Drawing Files

[Download Drawing PDF](FILE-LINK-HERE)

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Project Time

### Time Spent

| Task | Time |
|---|---:|
| Feature 1 Calculations | |
| Feature 2 Calculations | |
| Sketch / Concept Design | |
| CAD / Parametric Design | |
| Engineering Drawing | |
| Website Documentation | |
| **Total** | ** hrs** |

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">





