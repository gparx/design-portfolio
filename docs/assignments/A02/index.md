# A2 – Truss Stress Analysis

<br>

## Project Overview

[Briefly describe the purpose of the project.]

[Explain what was designed, how the design was analyzed, and what tools were used.]

[Describe the overall goal of the project.]

<br>

### Design Constraints

- Applied load: [ ]
- Dimension \(a\): [ ]
- Dimension \(b\): [ ]
- Truss material: [ ]
- Member cross-sectional geometry: [ ]
- Member safety factor: [ ]
- Pin material: [ ]
- Pin safety factor: [ ]
- Pin connection type: [ ]

[Embed original design-constraint figure here.]

![Design Constraints](IMAGE_PATH)

<br><br>

# 1. Documentation

## Design Process

[Explain how the project was approached from beginning to end.]

[Describe why the chosen process was used.]

[Describe what major steps were completed.]

<br>

### Process Notes

- [Step / observation]
- [Step / observation]
- [Step / observation]

<br>

### Mistakes and Revisions

[Describe a mistake or problem encountered.]

[Explain how the problem was identified.]

[Explain what was changed to correct it.]

<br>

### Time Spent

**Total project time:** [ ]

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 2. Truss Design

## 2a. Overall Truss Geometry

### Initial Truss Design

[Explain why this truss geometry was selected.]

[Explain how the geometry satisfies the required locations and loads.]

[Explain what members were included in the final design.]

<br>

![Truss Geometry](IMAGE_PATH)

<br>

### 2a.i. Member Geometry and Lengths

#### Joint Coordinates

| Joint | Coordinates |
|---|---|
| A | [ ] |
| B | [ ] |
| C | [ ] |
| D | [ ] |

<br>

#### Member Lengths

| Member | Symbolic Length | Numerical Length |
|---|---:|---:|
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |

<br>

### Geometry Calculations

$$
[Equation]
$$

$$
[Equation]
$$

$$
[Equation]
$$

<br><br>

## 2a.ii. Free-Body Diagrams

### Entire Truss FBD

[Embed full-truss free-body diagram here.]

![Entire Truss FBD](IMAGE_PATH)

<br>

### Support Reaction Equations

$$
\sum F_x = 0
$$

$$
[Equation]
$$

$$
\sum F_y = 0
$$

$$
[Equation]
$$

$$
\sum M = 0
$$

$$
[Equation]
$$

<br>

### Support Reactions

| Reaction | Value |
|---|---:|
| [ ] | [ ] |
| [ ] | [ ] |
| [ ] | [ ] |

<br><br>

### Joint A FBD

![Joint A FBD](IMAGE_PATH)

$$
\sum F_x = 0
$$

$$
[Equation]
$$

$$
\sum F_y = 0
$$

$$
[Equation]
$$

<br><br>

### Joint B FBD

![Joint B FBD](IMAGE_PATH)

$$
\sum F_x = 0
$$

$$
[Equation]
$$

$$
\sum F_y = 0
$$

$$
[Equation]
$$

<br><br>

### Joint C FBD

![Joint C FBD](IMAGE_PATH)

$$
\sum F_x = 0
$$

$$
[Equation]
$$

$$
\sum F_y = 0
$$

$$
[Equation]
$$

<br><br>

### Joint D FBD

![Joint D FBD](IMAGE_PATH)

$$
\sum F_x = 0
$$

$$
[Equation]
$$

$$
\sum F_y = 0
$$

$$
[Equation]
$$

<br><br>

## 2a.iii. Symbolic Internal Force Analysis

[Explain why the method of joints was used.]

[Explain how the joint equations were solved.]

[Explain what the symbolic analysis determines.]

<br>

#### Member [ ]

$$
[Symbolic equation]
$$

#### Member [ ]

$$
[Symbolic equation]
$$

#### Member [ ]

$$
[Symbolic equation]
$$

#### Member [ ]

$$
[Symbolic equation]
$$

#### Member [ ]

$$
[Symbolic equation]
$$

<br><br>

## 2a.iv. Numerical Internal Force Analysis

| Member | Internal Force | Tension / Compression |
|---|---:|---|
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |
| [ ] | [ ] | [ ] |

<br>

### Critical Member

[Identify the member containing the largest internal force.]

$$
F_{\max} = [ ]
$$

<br><br>

# 2b. Truss Member Cross-Section Design

## 2b.i. Knowns and Unknowns

### Knowns

- Maximum internal force: [ ]
- Material yield strength: [ ]
- Safety factor: [ ]
- Material density: [ ]
- Member cross-sectional geometry: [ ]

<br>

### Unknowns

- Minimum member cross-sectional area: [ ]
- Member dimensions: [ ]
- Approximate truss weight: [ ]

<br><br>

## 2b.ii. Symbolic Cross-Sectional Area Calculation

[Explain why yield strength and the factor of safety are used.]

[Explain how allowable stress is determined.]

[Explain what the resulting area represents.]

$$
\sigma = \frac{F}{A}
$$

$$
\sigma_{allow} = [ ]
$$

$$
[Symbolic derivation]
$$

$$
\boxed{A_{min} = [ ]}
$$

<br><br>

## 2b.iii. Numerical Cross-Sectional Area

$$
[Substitution]
$$

$$
\boxed{A_{min} = [ ]}
$$

<br>

### Selected Member Geometry

Cross-sectional shape: [ ]

$$
[Geometry equation]
$$

$$
\boxed{[Final member dimensions]}
$$

<br><br>

## 2b.iv. Approximate Truss Weight

### Total Member Length

$$
L_{total} = [ ]
$$

<br>

### Truss Volume

$$
V = AL
$$

$$
V = [ ]
$$

<br>

### Truss Mass / Weight

$$
m = \rho V
$$

$$
m = [ ]
$$

$$
W = mg
$$

$$
\boxed{W = [ ]}
$$

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 3. Connecting Pin Design

## 3a. Single-Shear Pin Connection

[Explain why a single-shear model is used.]

[Explain how the critical pin load was determined.]

[Explain what dimensions were determined from the analysis.]

<br><br>

## 3a.i. Knowns and Unknowns

### Knowns

- Pin material: [ ]
- Shear yield strength: [ ]
- Density: [ ]
- Safety factor: [ ]
- Connection type: [ ]
- Critical pin force: [ ]
- Number of pins: [ ]

<br>

### Unknowns

- Minimum pin cross-sectional area: [ ]
- Pin diameter: [ ]
- Pin length: [ ]
- Combined pin weight: [ ]

<br><br>

## 3a.ii. Critical Pin Free-Body Diagram

![Critical Pin FBD](IMAGE_PATH)

<br>

### Resultant Pin Force

$$
\sum F_x = [ ]
$$

$$
\sum F_y = [ ]
$$

$$
V = \sqrt{(\sum F_x)^2 + (\sum F_y)^2}
$$

$$
\boxed{V_{max} = [ ]}
$$

<br><br>

## 3a.iii. Symbolic Pin Area Calculation

$$
\tau = \frac{V}{A}
$$

$$
\tau_{allow} = [ ]
$$

$$
[Symbolic derivation]
$$

$$
\boxed{A_{pin,min} = [ ]}
$$

<br><br>

## 3a.iv. Numerical Pin Area

$$
[Substitution]
$$

$$
\boxed{A_{pin,min} = [ ]}
$$

<br>

### Pin Diameter

$$
A = \frac{\pi d^2}{4}
$$

$$
d = [ ]
$$

$$
\boxed{d_{pin} = [ ]}
$$

<br><br>

## 3a.v. Approximate Combined Pin Weight

### Pin Length Assumption

[Explain how the approximate pin length was selected.]

$$
L_{pin} = [ ]
$$

<br>

### Pin Volume

$$
V_{pin} = A_{pin}L_{pin}
$$

<br>

### Combined Pin Weight

$$
W_{pins} = n\rho A_{pin}L_{pin}
$$

$$
[Substitution]
$$

$$
\boxed{W_{pins} = [ ]}
$$

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 4. CAD Model and Verification

## 4a. Truss CAD Model

[Explain how the truss was modeled as one CAD part.]

[Explain why the CAD geometry represents the analytical design.]

[Explain what dimensions were transferred from the hand calculations.]

<br>

![Truss CAD Part](IMAGE_PATH)

<br><br>

## 4b. Pin Joint Geometry

[Explain how the cross-sectional area was maintained near the pin joints.]

[Explain how the pin holes and surrounding material were modeled.]

[Explain what dimensions were used.]

<br>

![Pin Joint CAD](IMAGE_PATH)

<br><br>

## Pin CAD Model

![Pin CAD Part](IMAGE_PATH)

<br>

### Pin CAD Dimensions

| Feature | Dimension |
|---|---:|
| Diameter | [ ] |
| Length | [ ] |
| Cross-sectional area | [ ] |

<br><br>

## 4c. Design Verification

### Safety Factor

[Explain how the member dimensions satisfy the required safety factor.]

[Explain how the pin dimensions satisfy the required safety factor.]

[Explain why the final CAD dimensions were retained.]

<br>

### Geometric Constraints

[Explain how dimensions \(a\), \(b\), joint locations, and required geometry were maintained.]

<br>

### Structural Stability

[Explain why the truss geometry is structurally stable.]

<br>

### Weight Optimization

[Explain how material use was minimized while satisfying the design requirements.]

<br><br>

## Final CAD Assembly

![Final CAD Assembly](IMAGE_PATH)

<br><br>

## 4d. CAD Mass Properties

[Explain why CAD mass properties were calculated.]

[Explain what material properties were assigned.]

[Explain what the CAD mass result represents.]

<br>

![CAD Mass Properties](IMAGE_PATH)

<br>

### CAD Results

| Property | Value |
|---|---:|
| Volume | [ ] |
| Mass | [ ] |
| Weight | [ ] |

<br><br>

# Analytical vs. CAD Weight Comparison

| Method | Truss | Pins | Total |
|---|---:|---:|---:|
| Hand Calculation | [ ] | [ ] | [ ] |
| CAD Model | [ ] | [ ] | [ ] |

<br>

### Percent Difference

$$
\%\,Difference =
\frac{|[Value]-[Value]|}{[Reference Value]}
\times100
$$

$$
\boxed{\%\,Difference = [ ]}
$$

<br>

[Explain why the hand-calculated and CAD-predicted weights are not exactly identical.]

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# 5. Engineering Lessons Learned

[Describe a specific engineering principle learned during the project.]

[Explain how the project demonstrated that principle.]

[Explain how this knowledge could be applied to a future engineering design.]

<br>

### Additional Lessons

- [Specific lesson]
- [Specific lesson]
- [Specific lesson]

<br><br>

# Mistakes and Design Revisions

## Revision 1

**Problem:**  
[ ]

**Cause:**  
[ ]

**Correction:**  
[ ]

**Engineering lesson:**  
[ ]

<br>

## Revision 2

**Problem:**  
[ ]

**Cause:**  
[ ]

**Correction:**  
[ ]

**Engineering lesson:**  
[ ]

<br><br>

# Project Files

## CAD Files

**[Download the completed CAD files](/design-portfolio/files/TRUSS.zip)**

> The downloadable file should include the truss part, pin part, and completed assembly.

<br><br>

# Project Time

| Task | Time |
|---|---:|
| Truss geometry and FBDs | [ ] |
| Analytical calculations | [ ] |
| Pin calculations | [ ] |
| CAD modeling | [ ] |
| CAD assembly and mass properties | [ ] |
| Portfolio documentation | [ ] |
| **Total Time** | **[ ]** |

<br><br>
