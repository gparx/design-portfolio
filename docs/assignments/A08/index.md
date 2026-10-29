
# A08: Gear Box Design

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Project Overview

Design a gearbox which can be assembled and disassembled. The spur gears have a gear ratio of 24:9 and are listed in the resource section. The output gear torque and speed are to be 1.25 in-lbf and 1100 rpm relative. The input (pinion,power-transmission) and output (gear, short shaft) shaft diameters are .125 and .25 inches respectively and each have a length of 1 inch. Use the appropriate equations in the Machinery’s Handbook for empirical units. The critical features of the gearbox include the shafts, and the journal bearings.

### Design Specifications

| Parameter | Value |
|---|---|
| Gear Ratio | 24:9 |
| Output Torque | 1.25 in-lbf |
| Output Speed | 1100 rpm |
| Input Shaft Diameter | 0.125 in |
| Output Shaft Diameter | 0.250 in |
| Shaft Length | 1.00 in each |
| Gear Train | Ideal |

### Design Assumptions

- Ideal gear train with no power losses.
- Negligible bending moments from radial gear forces.
- Shafts are press-fitted into the gear hubs.
- Running/sliding fits are used at the bearing interfaces.
- Adequate clearance is maintained between moving components and the housing.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 1. Shaft Design — Torsional Stress


### Input Shaft

**Known Parameters:**

| Parameter | Value |
|---|---|
| Length | 1.00 in |
| Shaft Diameter | 0.125 in |
| Input Torque | ? |
| Input Speed | ? |
| Material | ? |
| Maximum Shear Stress | ? |
| Allowable Shear Stress | ? |
| Sufficient Diameter? | ? |

**Free-Body Diagram:**

<img width="1167" height="453" alt="image" src="https://github.com/user-attachments/assets/6f874aee-8c9d-4866-a123-8822e59e77c0" />


**Equations:**

- T_in = T_out(9/24) 
- n_in = n_out(24/9) 
- J = πd⁴/32
- τ_max = Tc/J = 16T/(πd³)
- τ_max = 1222.3 psi


<img width="1199" height="579" alt="image" src="https://github.com/user-attachments/assets/82590317-8cf9-4da7-ae81-1ad8c971eb69" />


<img width="1146" height="1097" alt="image" src="https://github.com/user-attachments/assets/1f628bf2-99e2-44d6-937c-3e6b57d91fe6" />


**Results:**

| Parameter | Result |
|---|---|
| Length | 1.00 in |
| Shaft Diameter | 0.125 in |
| Input Torque | 0.46875 in-lbf |
| Input Speed | 2933 rpm |
| Maximum Shear Stress in | 1222 psi |
| Maximum Shear Stress out | 407 psi |
| Allowable Shear Stress | 8447 psi |
| Sufficient Diameter? | Y |
| Material | - |

### Output Shaft

**Known Parameters:**

| Parameter | Value |
|---|---|
| Length | 1.00 in |
| Shaft Diameter | 0.250 in |
| Output Torque | 1.25 in-lbf |
| Output Speed | 1100 rpm |
| Maximum Shear Stress | ? |
| Allowable Shear Stress | ? |
| Sufficient Diameter? | ? |
| Material | - |

**Free-Body Diagram:**

<img width="1114" height="370" alt="image" src="https://github.com/user-attachments/assets/677a0f2e-fe82-4eab-ae31-04e32f814f6d" />


<img width="1103" height="934" alt="image" src="https://github.com/user-attachments/assets/2c03d016-514f-453d-be81-af49f1dabfd6" />


**Results:**

| Parameter | Result |
|---|---|
| Length | 1.00 in |
| Shaft Diameter | 0.250 in |
| Output Torque | 1.25 in-lbf |
| Output Speed | 1100 rpm |
| Maximum Shear Stress in | 1222 psi |
| Maximum Shear Stress out | 407 psi |
| Allowable Shear Stress | 8447 psi |
| Sufficient Diameter? | Y |
| Material | - |



<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 2. Journal Bearing Design

Journal bearings are used to support the rotating shafts while allowing relative rotation.

### Bearing Length and Material Selection

**Known / Unknown Parameters:**

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Shaft Diameter | 0.125 in | 0.250 in |
| Shaft Speed | 2933 rpm | 1100 rpm |
| Bearing Load | ? | ? |
| Bearing Length | ? | ? |
| Bearing Material | ? | ? |


| Parameter | Input Pinion | Output Gear |
|---|---|---|
| McMaster Part | 7880K19 | 7880K24 |
| Number of Teeth | 18 | 48 |
| Pitch Diameter | 0.375 in | 1.000 in |
| Pressure Angle | 20° | 20° |


**Free-Body Diagram:**

<img width="1087" height="462" alt="image" src="https://github.com/user-attachments/assets/5c6dcf3c-91aa-4691-81b4-c7a4a53cc7d9" />


**Design Equations:**

- Tangential Gear Force: Fₜ = 2T/Dₚ
- Radial Gear Force: Fᵣ = Fₜ × tan(φ)
- Resultant Gear Force: F = √(Fₜ² + Fᵣ²)
- Bearing Load: W = F (assuming one bearing supports the full load)
- Bearing Pressure: P = W/(L × d)
- Surface Velocity: V = πdn/12 (ft/min)
- PV Rating = P × V

<img width="1198" height="1209" alt="image" src="https://github.com/user-attachments/assets/ecd10054-a585-4148-8d50-a93142463fae" />


**Calculated Results:**

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Shaft Diameter | 0.125 in | 0.250 in |
| Bearing Load | 2.66 lbf | 2.66 lbf |
| Proposed Length | 0.250 in | 0.250 in |
| Pressure | 85.13 psi | 42.57 psi |
| Surface Velocity | 95.99 ft/min | 72.00 ft/min |
| PV Rating | 8,172 psi·ft/min | 3,065 psi·ft/min |
| Preliminary P/V/PV Check | Pass | Pass |


### Bearing Wall Thickness

Bearing wall thickness is determined by analyzing the stresses acting on the sleeve.

**Selected Material:** 
SAE 841 oil-impregnated bearing bronze

| Specification | Published Limit |
|---|---|
| Maximum Pressure | 2,000 psi |
| Maximum Velocity | 1,200 ft/min |
| Maximum PV Rating | 50,000 psi·ft/min |
| Tensile Y. Str. | 11,000 psi |


**Calculations:**

<img width="1175" height="695" alt="image" src="https://github.com/user-attachments/assets/b1cb4329-a612-482d-88df-0f243996264f" />


### Final Journal Bearing Wall Thickness Results

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Bearing Load | 2.66 lbf | 2.66 lbf |
| Bearing Pressure | 85.13 psi | 42.57 psi |
| Assumed Allowable Stress | 5,500 psi | 5,500 psi |
| Calculated Minimum Thickness | 0.000967 in | 0.000968 in |
| Selected Nominal Thickness | 0.03125 in | 0.03125 in |
| Material | SAE 841 Bronze | SAE 841 Bronze |
| Preliminary Thickness Check | Pass | Pass |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 3. Gearbox Housing Design

The gearbox housing consists of two separate halves designed to support the bearings and gears while allowing assembly and disassembly.

The housing must provide sufficient gear clearance, shaft alignment, and appropriate fastening features.

### Preliminary Housing Sketch



### Housing Design Features

- Two-piece removable housing.
- Aligned shaft and bearing openings.
- Adequate internal gear clearance.
- Fastening features for secure assembly.
- Appropriate shaft and bearing fits.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 4. Parametric CAD Modeling

The gearbox components are modeled and assembled in SolidWorks using parametric dimensions based on the shaft, gear, and bearing specifications.

### Parametrics

"Pinion_Pitch_Dia" = 0.375in
"Output_Pitch_Dia" = 1.000in

"Gear_Center_Distance" = ("Pinion_Pitch_Dia" + "Output_Pitch_Dia") / 2

"Input_Shaft_Dia" = 0.125in
"Output_Shaft_Dia" = 0.250in
"Shaft_Length" = 1.000in

"Input_Bearing_OD" = 0.1875in
"Output_Bearing_OD" = 0.3125in
"Bearing_Length" = 0.250in

"Housing_Length" = 2.500in
"Housing_Width" = 2.000in
"Housing_Height" = 0.375in

"Cavity_Length" = 2.000in
"Cavity_Width" = 1.500in
"Cavity_Depth" = 0.250in

"Wall_Thickness" = ("Housing_Length" - "Cavity_Length") / 2
"Floor_Thickness" = "Housing_Height" - "Cavity_Depth"


**Input and Output Shafts**

<img width="1615" height="1093" alt="Screenshot 2026-10-28 233457" src="https://github.com/user-attachments/assets/707ef524-cdb6-4c80-8977-629ecb7f5411" />

<img width="1622" height="1092" alt="Screenshot 2026-10-28 233515" src="https://github.com/user-attachments/assets/8952d534-ddf2-48c4-9456-7bd9e872ce26" />


**Journal Bearings and Gears**

<img width="1031" height="712" alt="Screenshot 2026-10-28 233446" src="https://github.com/user-attachments/assets/2e60dd28-f50f-4cf8-a3da-4489dbe9c66d" />

<img width="1302" height="956" alt="Screenshot 2026-10-28 233525" src="https://github.com/user-attachments/assets/5d2f6f1a-c066-447d-a3ed-cc29d7d0eac4" />

<img width="3839" height="2159" alt="Screenshot 2026-10-28 203420" src="https://github.com/user-attachments/assets/3c3c806f-8f24-40df-8217-ac9a329046c8" />


**Gearbox Housing — Upper and Lower Halves**

<img width="1276" height="734" alt="image" src="https://github.com/user-attachments/assets/d96c38b5-22ea-43e9-a24e-ad8a67b6a56f" />

<img width="1809" height="1206" alt="Screenshot 2026-10-28 233503" src="https://github.com/user-attachments/assets/defea4a4-0ef0-46cf-9507-639b59beb37f" />


### Final Assembly

The shafts, gears, bearings, and housing are assembled using appropriate mates to establish alignment and component positioning.

<img width="1732" height="1374" alt="Screenshot 2026-10-28 232719" src="https://github.com/user-attachments/assets/a3e2af9a-9a60-4d8d-bd60-c79e937247a9" />


### Engineering Drawings

Six multiview part drawings and one assembly drawing are required.

<img width="2460" height="1912" alt="Screenshot 2026-10-29 000708" src="https://github.com/user-attachments/assets/b9f187bc-6b8f-445f-98ce-8fe1051fa281" />

<img width="2573" height="1931" alt="Screenshot 2026-10-29 000713" src="https://github.com/user-attachments/assets/370d7eb9-afd3-42f8-90d6-7a0cd55f90e5" />

<img width="1928" height="1490" alt="Screenshot 2026-10-29 000719" src="https://github.com/user-attachments/assets/1789909a-78bd-4619-886d-353b1b9ade6c" />

<img width="1736" height="1126" alt="Screenshot 2026-10-29 000736" src="https://github.com/user-attachments/assets/5a94f816-822e-4198-a301-2183fee05d49" />

<img width="2267" height="1467" alt="Screenshot 2026-10-29 000759" src="https://github.com/user-attachments/assets/e7f3dbe7-7d70-4b99-b314-a5940ac59cef" />

<img width="1842" height="1401" alt="Screenshot 2026-10-29 000702" src="https://github.com/user-attachments/assets/5e776018-9770-4a3b-9c67-4640077f3797" />

**General Tolerances (in):**

| Dimension | Tolerance |
|---|---|
| X.X | ±0.02 |
| X.XX | ±0.01 |
| X.XXX | ±0.005 |

### CAD Files

[MASTER FILE DOWNLOAD HERE](https://github.com/user-attachments/files/34111946/Gear_Box.zip)


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 5. Lessons Learned

- Applying torsional stress equations to shaft design.
- Evaluating journal bearing pressure, velocity, and PV limits.
- Designing mechanical components with appropriate fits and tolerances.
- Developing parametric CAD components and assemblies.
- Considering manufacturability, alignment, and ease of assembly.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## References

1. Machinery's Handbook, 32nd Edition — Shafts, pp. 295–297.
2. Machinery's Handbook — Gears and Gearing, pp. 2204–2211.
3. Machinery's Handbook — Plain Bearing Materials, pp. 2435–2443.
4. [McMaster-Carr — Pinion Gear](https://www.mcmaster.com/catalog/129/1330/7880K19)
5. [McMaster-Carr — Output Gear](https://www.mcmaster.com/catalog/129/1330/7880K24)
6. [McMaster-Carr — Sleeve Bearings](https://www.mcmaster.com/products/journal-bearings/sleeve-bearings-3~/)
