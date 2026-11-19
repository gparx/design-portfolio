
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

[DOWNLOAD STEP FILE](https://github.com/user-attachments/files/34896086/MOTOR.zip)

---

### Torque and Speed Verification

---

<img width="1086" height="664" alt="Screenshot 2026-11-15 212300" src="https://github.com/user-attachments/assets/7b489af2-0911-4a76-b6d7-eb18353ec272" />

---

### Speed–Torque Curve

---

<img width="1747" height="805" alt="Screenshot 2026-11-15 215418" src="https://github.com/user-attachments/assets/ded96bf7-09da-490e-b680-bb292f42d875" />

---

- Conclusion: At 15.7 RPM Motor can operate at 13.28Nm of pull-out torque, exceeding our minimum of 6.52 Nm from the motor while meeting our RPM Goals.


### Motor Selection Summary

| Parameter | Value |
|---|---|
| Selected Motor | 23HS30-2904S-MG10 |
| Motor Type | NEMA 23 Geared Stepper |
| Gear Ratio | 10:1 |
| Required Output Torque | 6.52 N·m |
| Required Output Speed | 0.315–15.75 RPM |
| Motor Speed Range | 3.15–157.5 RPM |
| Pull-Out Torque at 15.7 RPM | 13.28 N·m |
| Gearbox Efficiency | 90% |
| Rated Current | 2.9 A/phase |
| Output Shaft Diameter | 14 mm |
| Quantity | 2 |

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 2. Motor Mount Design ( Grant )

### Unknowns

| Unknown Parameter | Symbol |
|---|---|
| Bolt Radius | r |
| Force per Bolt | F |
| Bearing Stress | σ |
| Minimum Bracket Thickness | t_min |
| Selected Bracket Thickness | t |


---

<img width="805" height="797" alt="Screenshot 2026-11-15 231507" src="https://github.com/user-attachments/assets/ebe929b6-4eca-4ca6-a7b7-688f4af8bf18" />

---

<img width="2260" height="881" alt="Screenshot 2026-11-15 231438" src="https://github.com/user-attachments/assets/5e33bdf7-12ae-410a-b3b5-f5365094ef3e" />

---
### Free Body Diagram

---

<img width="1114" height="428" alt="Screenshot 2026-11-15 235730" src="https://github.com/user-attachments/assets/79e42674-1122-47b6-9694-aef7125044c3" />

---

### Bearing Stress Analysis

---

<img width="1048" height="982" alt="Screenshot 2026-11-15 235756" src="https://github.com/user-attachments/assets/36a2401c-7913-48db-996f-2c9e939a40b3" />

---

### Minimum Bracket Thickness

---

<img width="1102" height="707" alt="Screenshot 2026-11-16 002524" src="https://github.com/user-attachments/assets/6d61a5ac-96e0-4f21-9b85-eb2e69ba83f0" />

---

### Calculated Results

| Parameter | Value |
|---|---|
| Mounting Hole Pattern | 47.14 × 47.14 mm |
| Hole Diameter | 5.2 mm |
| Bolt Diameter | 5.0 mm (M5) |
| Bolt Radius, r | 33.33 mm |
| Force per Bolt, Fb | 12.23 N |
| Minimum Thickness, t_min | 0.0354 mm |
| Selected Thickness | 6.35 mm |

- Conclusion: The minimum required thickness is 0.0354 mm. A common standard aluminum plate thickness is 6.35mm (0.25in) which covers our required thickness.
  
---

<img width="1546" height="988" alt="Screenshot 2026-11-16 140359" src="https://github.com/user-attachments/assets/d2a21b8c-01ab-4e2a-a1ee-42eb4b7b55b8" />

---

<img width="2030" height="1212" alt="Screenshot 2026-11-16 140446" src="https://github.com/user-attachments/assets/a99d5884-ede7-4a45-b1ee-80d0837d4a87" />

---

<img width="2168" height="1074" alt="Screenshot 2026-11-16 140449" src="https://github.com/user-attachments/assets/83658ed2-1db7-43ad-8897-6a955d42687c" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 3. Coupler Design ( Grant )

### FBD, Theoretical Design and Calculations

---

<img width="1181" height="1634" alt="image" src="https://github.com/user-attachments/assets/b8015a40-0cb0-4e4e-b995-42538ab972bf" />

---

### Designed Coupler

---

<img width="890" height="621" alt="Screenshot 2026-11-16 211704" src="https://github.com/user-attachments/assets/613c2183-0d5f-4079-8d23-d62ec3a5287e" />

---

<img width="1113" height="640" alt="Screenshot 2026-11-16 211709" src="https://github.com/user-attachments/assets/1090fd01-9f51-42d9-ad61-38a1cb0ce4f0" />

---

### Keyway

---

<img width="1093" height="565" alt="Screenshot 2026-11-16 221132" src="https://github.com/user-attachments/assets/f057963b-f279-4fd9-9c2a-30f40b54f49b" />

---

### Assembly Check

---

<img width="1453" height="796" alt="Screenshot 2026-11-16 215510" src="https://github.com/user-attachments/assets/bd0795f5-1079-4a79-9c1f-a8750692ca65" />

---

<img width="1599" height="975" alt="Screenshot 2026-11-16 215528" src="https://github.com/user-attachments/assets/48f64683-49f0-41fd-8b3e-5ddec26b4e77" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 4. Frame Connection Design (Bryan)

---

<img width="446" height="557" alt="1_Frame_Idea_to_verify" src="https://github.com/user-attachments/assets/4a911f4d-b4ca-49b6-ad3f-78b4710d5ad7" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 5. Top Frame FEA (Bryan)

---

<img width="438" height="341" alt="2_Bracket_Hand_Calcs" src="https://github.com/user-attachments/assets/83dd1569-56da-4325-975d-69220332c5b6" />

---

<img width="499" height="386" alt="3_Top_Bar_Fixture Force" src="https://github.com/user-attachments/assets/6cd1a0e8-8092-4561-a90c-df0dedb0a73a" />

---

<img width="379" height="393" alt="4_Top_Bar_Torque" src="https://github.com/user-attachments/assets/ef6c53f8-ef57-4b64-8614-5694199af2fa" />

---

<img width="755" height="451" alt="5_Top_Bar_Stress1" src="https://github.com/user-attachments/assets/9d9e7692-5404-4a41-90ec-9a76b69dac31" />

---

<img width="701" height="445" alt="6_Top_Bar_Defl1" src="https://github.com/user-attachments/assets/9153e66f-d34c-48bc-bc91-51defd26361c" />

---

<img width="595" height="539" alt="7_Max_Stress_Location" src="https://github.com/user-attachments/assets/aeb6f974-c75b-489f-ad56-e80731664bd7" />

---

<img width="527" height="377" alt="8_Top_Bar_Stress2" src="https://github.com/user-attachments/assets/192c49c9-3eaa-4f8e-a388-13b7a4bfe057" />

---

<img width="683" height="384" alt="9_Top_Bar_Defl2" src="https://github.com/user-attachments/assets/eefadb63-03c2-4b7d-9f9b-2f68a26a2058" />

---

<img width="351" height="138" alt="10_Top_Bar_Convergence" src="https://github.com/user-attachments/assets/d5aefc6a-ae2d-4cd0-9816-5934be7c26d5" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 6. Vertical Frame FEA (Bryan)

<img width="380" height="281" alt="11_Side_Bar_Fixture" src="https://github.com/user-attachments/assets/91d0ac64-5ae5-4450-80cf-a6673092f0e8" />

---

<img width="594" height="597" alt="13_Side_Bar_Transverse_Force" src="https://github.com/user-attachments/assets/ea3aed0a-606a-4b6e-a4de-94fb5fd5fe9e" />

---

<img width="440" height="417" alt="14_Side_Bar_Stress1" src="https://github.com/user-attachments/assets/74414fba-e377-4f95-b781-e7b20339cd14" />

---

<img width="449" height="278" alt="15_Side_Bar_Max_Stress" src="https://github.com/user-attachments/assets/0be5b7f5-6998-465f-8405-9db93726edbf" />

---

<img width="558" height="521" alt="16_Side_bar_Defl1" src="https://github.com/user-attachments/assets/6cbf5ffa-76f7-4b51-8113-e6ae3024b02a" />

---

<img width="631" height="494" alt="16_Side_Bar_Stress2" src="https://github.com/user-attachments/assets/5b312d63-6dea-45b4-ad43-cbe8316636e1" />

---

<img width="539" height="462" alt="17_Side_Bar_Defl2" src="https://github.com/user-attachments/assets/684c52b5-da1b-4276-bb7a-21f7bf936eb1" />

---

<img width="350" height="143" alt="18_Side_bar_Converges" src="https://github.com/user-attachments/assets/4ebe21ea-1c13-4cb5-b32e-048dd2734694" />

---

<img width="797" height="65" alt="19_FoS_and_Optimization" src="https://github.com/user-attachments/assets/67914bce-6b61-4f26-bf06-d76983e935a8" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 7. Floating Bearing Mount (Bryan)

---

<img width="1189" height="969" alt="Screenshot 2026-11-18 195057" src="https://github.com/user-attachments/assets/cc0eb3e6-f711-43b9-a1a8-aad9e3804f86" />

---

<img width="522" height="464" alt="2_Modeled_Part" src="https://github.com/user-attachments/assets/887aeb8a-dc2f-4afb-9c55-2b89449c7716" />

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 8. Bill of Materials and Labor Costs (Grant)

### Bill of Materials

| Item Number | Quantity | Name | Cost/Item | Cost | Purchase Link |
|:---:|:---:|---|---:|---:|---|
| 1 | 4 | T-Slot Aluminum Extrusion (2 ft) | $51.82 | $207.28 | [5537T112](https://www.mcmaster.com/5537T112/) |
| 2 | 8 | T-Slot 90° Corner Brackets | $20.18 | $161.44 | [3136N924](https://www.mcmaster.com/3136N924/) |
| 3 | 8 | M5 × 65 mm Screws (25-pack) | $4.10/pack | $4.10 | [91290A270](https://www.mcmaster.com/91290A270/) |
| 4 | 8 | M5 Flange Locknuts (100-pack) | $3.52/pack | $3.52 | [94920A120](https://www.mcmaster.com/94920a120/) |
| 5 | 8 | T-Slot Nut & Screw Combos (4-pack) | $25.10/pack | $50.20 | [5021N15](https://www.mcmaster.com/5021N15/) |
| 6 | 1 | 932 Bearing Bronze Stock (Floating Bearing) | $187.45 | $187.45 | [8234K22](https://www.mcmaster.com/8234K22/) |
| 7 | 1 | Custom Motor Coupler (Fabricated) | TBD | TBD | — |
| 8 | 1 | NEMA 23 Motor Mount | $5.75 | $5.75 | [RobotShop](https://www.robotshop.com/products/stepper-motor-mounting-bracket-nema-23) |
| 9 | 1 | NEMA 23 Geared Stepper Motor (10:1) | $40.05 | $40.05 | [StepperOnline](https://www.omc-stepperonline.com/nema-23-stepper-motor-l-76mm-gear-ratio-10-1-mg-series-planetary-gearbox-23hs30-2904s-mg10) |
| 10 | 2 | Acme Lead Screw, 5/8"-8, 36" Long | $102.38 | $204.76 | [97014A320](https://www.mcmaster.com/97014A320/) |
| 11 | 2 | Bronze Acme Flange Nut, 5/8"-8 | $138.20 | $276.40 | [95120A119](https://www.mcmaster.com/95120A119/) |
| 12 | 1 Pack (10 Screws) | Socket Head Screw, #6-32, 3/4" Long | $4.41/pack | $4.41 | [92200A151](https://www.mcmaster.com/92200A151/) |
| | | | **Total Material Cost** | **$1,145.36** | |

### Design Cost

| Person | Hours Worked | Cost/Hour | Cost |
|:---:|:---:|---:|---:|
| Grant | 12 | $30.00 | $360.00 |
| Ethan | 12 | $30.00 | $360.00 |
| Bryan | 12 | $30.00 | $360.00 |
| | | **Total Design Cost** | **$1,080.00** |

### Total Project Cost

| Category | Cost |
|---|---:|
| Materials and Components | $1,145.36 |
| Design Labor | $1,080.00 |
| **Total Cost of Project** | **$2,225.36** |

*Note: Total excludes the unpriced custom motor coupler, shipping, and taxes. Fastener costs account for complete purchase packs.*



<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">

## 9. Engineering Lessons Learned

## Engineering Drawings
### Motor Mount
### Coupler
### Frame Components
### Floating Bearing Mount
### Crosshead (A10)
### Assembly Drawing

## Google Drive

---

[DOWNLOAD CAD FILES HERE](https://drive.google.com/drive/folders/1u-TWogEifa_BrdLtgf8Pgp2fLFRhht96?usp=sharing)

---

<hr style="border: none; height: 3px; background-color: #888; margin: 20px 0;">
