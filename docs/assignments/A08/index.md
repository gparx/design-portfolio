
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
| Diameter | 0.125 in |
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


**Results:**

| Parameter | Result |
|---|---|
| Diameter | 0.125 in |
| Length | 1.00 in |
| Shaft Diameter | 0.125 in |
| Input Torque | 0.46875 in-lbf |
| Input Speed | 2933 rpm |
| Material | ? |
| Maximum Shear Stress in | 1222 psi |
| Maximum Shear Stress out | 407 psi |
| Allowable Shear Stress |  |
| Sufficient Diameter? |  |

### Output Shaft

**Known Parameters:**

| Parameter | Value |
|---|---|
| Diameter | 0.250 in |
| Length | 1.00 in |
| Output Torque | 1.25 in-lbf |
| Output Speed | 1100 rpm |
| Material | ? |

**Free-Body Diagram:**



**Equations:**

- J = πd⁴/32
- τ_max = Tc/J = 16T/(πd³)
- τ_max = ?

**Results:**

| Parameter | Result |
|---|---|
| Maximum Shear Stress | ? |
| Allowable Shear Stress | ? |
| Shaft Diameter | 0.250 in |
| Sufficient Diameter? | ? |

**Conclusion:** Final shaft diameter verification will be based on the selected shaft material and allowable shear stress.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 2. Journal Bearing Design

Journal bearings are used to support the rotating shafts while allowing relative rotation.

### Bearing Length and Material Selection

**Known / Unknown Parameters:**

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Shaft Diameter | 0.125 in | 0.250 in |
| Shaft Speed | 2933.33 rpm | 1100 rpm |
| Bearing Load | TBD | TBD |
| Bearing Length | TBD | TBD |
| Bearing Material | TBD | TBD |

**Free-Body Diagram:**



**Design Equations:**

- Bearing Pressure: P = W/(L × d)
- Surface Velocity: V = πdn/12 (ft/min)
- PV Rating = P × V

Where:
- W = Bearing load (lbf)
- L = Bearing length (in)
- d = Shaft diameter (in)
- n = Shaft speed (rpm)

**Calculated Results:**

| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Pressure (psi) | TBD | TBD |
| Velocity (ft/min) | TBD | TBD |
| PV Rating | TBD | TBD |
| Selected Length | TBD | TBD |
| Material | TBD | TBD |

### Bearing Wall Thickness

Bearing wall thickness is determined by analyzing the stresses acting on the sleeve.

**Stress Diagram:**

<!-- INSERT BEARING THICKNESS FBD -->

**Calculations:**


| Parameter | Input Bearing | Output Bearing |
|---|---|---|
| Calculated Thickness | TBD | TBD |
| Selected Thickness | TBD | TBD |
| Material | TBD | TBD |

### Selected Journal Bearings

| Component | Selected Part | Supplier |
|---|---|---|
| Input Shaft Bearing | TBD | McMaster-Carr |
| Output Shaft Bearing | TBD | McMaster-Carr |

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

### Component Modeling

**Input and Output Shafts**

<!-- INSERT SHAFT CAD IMAGES -->

**Journal Bearings and Gears**

<!-- INSERT GEAR AND BEARING CAD IMAGES -->

**Gearbox Housing — Upper and Lower Halves**

<!-- INSERT HOUSING CAD IMAGES -->

### Final Assembly

The shafts, gears, bearings, and housing are assembled using appropriate mates to establish alignment and component positioning.

<!-- INSERT FINAL ASSEMBLY IMAGE -->

### Engineering Drawings

Six multiview part drawings and one assembly drawing are required.

| Drawing | Status |
|---|---|
| Input Shaft | TBD |
| Output Shaft | TBD |
| Upper Housing | TBD |
| Lower Housing | TBD |
| Input Bearing | TBD |
| Output Bearing | TBD |
| Final Assembly | TBD |

All drawings will follow ASME Y14.5 dimensioning and tolerancing standards and use third-angle projection.

**General Tolerances (in):**

| Dimension | Tolerance |
|---|---|
| X.X | ±0.02 |
| X.XX | ±0.01 |
| X.XXX | ±0.005 |

At least two critical-feature tolerancing callouts will be included where appropriate.

<!-- INSERT ENGINEERING DRAWINGS -->

### CAD Files

**[Download Complete Gearbox CAD Files](REPLACE-WITH-CAD-DOWNLOAD-LINK)**

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 5. Lessons Learned

<!-- ADD REFLECTION AFTER COMPLETING THE PROJECT -->

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
