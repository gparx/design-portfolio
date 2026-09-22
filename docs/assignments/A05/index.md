# Bracket Design – Stress, Stiffness, and Fits Analysis

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Project Overview

### Objectives

- Conduct stress analysis to determine appropriate dimensions for the structural features of the bracket.
- Generate free body diagrams (FBDs) to visualize forces and constraints acting on each feature.
- Identify known variables, unknown variables, assumptions, and algebraic models used for each analysis.
- Perform stiffness analysis to determine minimum required dimensions based on the allowable deflection.
- Compare dimensions obtained from stress and stiffness analyses to determine which requirement governs the final design.
- Generate detailed multiview sketches showing the dimensions obtained from both stress and stiffness analyses.
- Design a linkage connecting Feature A to a 1-inch diameter shaft.
- Select appropriate engineering fits and manufacturing methods for the required connections.
- Document engineering lessons learned throughout the design process.


### Design Requirements

- The bracket must support the horizontal load applied symmetrically by the polyester strap.
- Applied load must satisfy:

\[
500\text{ lbf} < F < 800\text{ lbf}
\]

- Safety Factor:

\[
SF = 4
\]

- Maximum allowable deflection for each feature:

\[
\delta_{max} = 0.005\text{ in}
\]

- Direct shear failure is assumed not to govern the design.
- The bracket should be designed symmetrically where practical.
- Five separate structural feature analyses are required: Features A, B, C, D, and E.
- Dimensions obtained from earlier features are used to determine loads and dimensions for downstream features.
- Final dimensions must satisfy both stress and stiffness requirements.


### Given Parameters

**Applied Force**

\[
500\text{ lbf} < F < 800\text{ lbf}
\]

Selected design load:

\[
F = \text{TBD lbf}
\]

Because the polyester strap applies the force symmetrically, the loading on Feature A is represented by the resultant of the two strap forces as shown in the provided example.

**Safety Factor**

\[
SF = 4
\]

**Maximum Allowable Deflection**

\[
\delta_{max} = 0.005\text{ in}
\]

**Rigid T-Beam Dimensions**

\[
a = 0.498\text{ in}^{+0.000}_{-0.001}
\]

\[
b = 0.9992\text{ in}^{+0.0000}_{-0.0005}
\]

\[
c = 1.499\text{ in}^{+0.000}_{-0.001}
\]

**Fit Requirements for T-Beam**

- Dimension **a:** Accuracy is not essential.
- Dimension **b:** Close fit that can be expected to run freely.
- Dimension **c:** Accurate location with minimum play is desired.


### Material Selection

The bracket must be manufactured from one of the following materials:

- Aluminum 6061-T6
- ASTM A36 Steel
- Titanium Ti-6Al-4V

**Selected Material:** TBD

Required material properties:

- Yield Strength:

\[
S_y = \text{TBD}
\]

- Elastic Modulus:

\[
E = \text{TBD}
\]

The same material properties will be used in the stress and stiffness calculations as appropriate.


### Initial Assumptions

- The material behaves as a homogeneous, isotropic, linear-elastic material within the design loading range.
- The bracket remains within the elastic region during loading.
- Small-deflection beam theory is applicable.
- Stress concentrations are neglected unless specifically required.
- Direct shear stress is assumed not to cause failure, as specified by the project requirements.
- Shear deflection is assumed negligible.
- Loading from the polyester strap is symmetric.
- Features are treated using idealized beam/bar models as specified in Appendix D.
- Feature A is modeled as a cantilever beam.
- Feature B is modeled as an axially loaded bar.
- Feature C is modeled as a simply supported beam with a concentrated load at its center.
- Dimensions obtained from each feature analysis may affect the loading or geometry of subsequent features.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part I – Stress Analysis

The allowable normal stress for the selected material is determined using:

\[
\sigma_{allow} = \frac{S_y}{SF}
\]

where:

\[
SF = 4
\]


## Feature A – Cantilever Beam

### Known Values

- Applied strap force:

\[
F = \text{TBD lbf}
\]

- Safety factor:

\[
SF = 4
\]

- Material:

\[
\text{TBD}
\]

- Material yield strength:

\[
S_y = \text{TBD}
\]

- Feature A is modeled as a cantilever beam.
- The polyester strap applies the load symmetrically to Feature A.
- Direct shear failure is neglected.


### Unknown Values

- Minimum required Feature A cross-sectional dimension.
- Minimum required radius/diameter of Feature A.
- Maximum bending stress.
- Reaction force at the fixed end.
- Reaction moment at the fixed end.


### Assumptions

- Feature A behaves as a cantilever beam.
- Loading from the strap is symmetric.
- Feature A has a constant cross-section.
- Material remains within the elastic range.
- Direct shear failure is neglected.
- Stress concentrations are neglected for the preliminary sizing analysis.


### Free Body Diagram

<!-- Insert Feature A stress-analysis FBD here -->


### Algebraic Model

Allowable stress:

\[
\sigma_{allow} = \frac{S_y}{SF}
\]

Maximum bending stress:

\[
\sigma_{max} = \frac{M_{max}c}{I}
\]

or equivalently:

\[
\sigma_{max} = \frac{M_{max}}{Z}
\]

Design requirement:

\[
\sigma_{max} \leq \sigma_{allow}
\]


### Numerical Solution

TBD


### Required Dimension from Stress

\[
\boxed{\text{Feature A stress-based dimension = TBD}}
\]


---

## Feature B – Axially Loaded Bar

### Known Values

- Feature B is modeled as an axially loaded bar.
- Applied load is determined from the reaction/load transferred from Feature A.
- Safety factor:

\[
SF = 4
\]

- Material:

\[
\text{TBD}
\]

- Yield strength:

\[
S_y = \text{TBD}
\]

- Direct shear failure is neglected.


### Unknown Values

- Axial force carried by Feature B.
- Required cross-sectional area.
- Required Feature B dimensions.
- Normal stress in Feature B.


### Assumptions

- Feature B carries primarily axial loading.
- Load acts through the centroid of the member.
- Bending in Feature B is neglected for the idealized analysis.
- Material remains within the elastic range.
- Cross-section is constant over the analyzed portion.


### Free Body Diagram

<!-- Insert Feature B stress-analysis FBD here -->


### Algebraic Model

Normal stress:

\[
\sigma = \frac{P}{A}
\]

Allowable stress:

\[
\sigma_{allow} = \frac{S_y}{SF}
\]

Design requirement:

\[
\frac{P}{A} \leq \frac{S_y}{SF}
\]


### Numerical Solution

TBD


### Required Dimension from Stress

\[
\boxed{\text{Feature B stress-based dimension = TBD}}
\]


---

## Feature C – Simply Supported Beam

### Known Values

- Feature C is modeled as a simply supported beam.
- A concentrated load acts at the center of the beam.
- The load is transferred from the preceding structural features.
- Safety factor:

\[
SF = 4
\]

- Material:

\[
\text{TBD}
\]

- Yield strength:

\[
S_y = \text{TBD}
\]

- Direct shear failure is neglected.


### Unknown Values

- Support reactions.
- Maximum bending moment.
- Required cross-sectional dimension of Feature C.
- Maximum bending stress.


### Assumptions

- Feature C behaves as a simply supported beam.
- The concentrated load acts at the center.
- The cross-section is constant.
- Material remains within the elastic range.
- Direct shear failure is neglected.


### Free Body Diagram

<!-- Insert Feature C stress-analysis FBD here -->


### Algebraic Model

For a simply supported beam with a concentrated center load:

\[
R_A = R_B = \frac{P}{2}
\]

Maximum bending moment:

\[
M_{max} = \frac{PL}{4}
\]

Maximum bending stress:

\[
\sigma_{max} = \frac{M_{max}c}{I}
\]

Design requirement:

\[
\sigma_{max} \leq \frac{S_y}{SF}
\]


### Numerical Solution

TBD


### Required Dimension from Stress

\[
\boxed{\text{Feature C stress-based dimension = TBD}}
\]


---

## Feature D – Structural Feature

### Known Values

- Feature D receives loading transferred through Feature C.
- Safety factor:

\[
SF = 4
\]

- Material:

\[
\text{TBD}
\]

- Yield strength:

\[
S_y = \text{TBD}
\]

- Direct shear failure is neglected.


### Unknown Values

- Loading acting on Feature D.
- Appropriate structural model.
- Required Feature D dimension.
- Maximum stress.


### Assumptions

- Material remains within the elastic range.
- Direct shear failure is neglected.
- Final loading/model will be determined from the load path and geometry.


### Free Body Diagram

<!-- Insert Feature D stress-analysis FBD here -->


### Algebraic Model

TBD after determining the appropriate loading model for Feature D.


### Numerical Solution

TBD


### Required Dimension from Stress

\[
\boxed{\text{Feature D stress-based dimension = TBD}}
\]


---

## Feature E – Structural Feature

### Known Values

- Feature E receives loading transferred through the preceding bracket features.
- Safety factor:

\[
SF = 4
\]

- Material:

\[
\text{TBD}
\]

- Yield strength:

\[
S_y = \text{TBD}
\]

- Direct shear failure is neglected.


### Unknown Values

- Loading acting on Feature E.
- Appropriate structural model.
- Required Feature E dimension.
- Maximum stress.


### Assumptions

- Material remains within the elastic range.
- Direct shear failure is neglected.
- Final loading/model will be determined from the load path and geometry.


### Free Body Diagram

<!-- Insert Feature E stress-analysis FBD here -->


### Algebraic Model

TBD after determining the appropriate loading model for Feature E.


### Numerical Solution

TBD


### Required Dimension from Stress

\[
\boxed{\text{Feature E stress-based dimension = TBD}}
\]


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part II – Stiffness Analysis

**Maximum Allowable Deflection:**

\[
\boxed{\delta_{max} = 0.005\text{ in}}
\]

Shear deflections are assumed negligible.


## Feature A – Cantilever Beam

### Known Values

- Applied load:

\[
F = \text{TBD lbf}
\]

- Maximum allowable deflection:

\[
\delta_{max} = 0.005\text{ in}
\]

- Material elastic modulus:

\[
E = \text{TBD}
\]

- Feature A is modeled as a cantilever beam.


### Unknown Values

- Required Feature A cross-sectional dimension based on stiffness.
- Area moment of inertia:

\[
I
\]

- Maximum Feature A deflection.


### Assumptions

- Small-deflection beam theory applies.
- Material remains linear-elastic.
- Feature A has a constant cross-section.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature A stiffness-analysis FBD here -->


### Deflection Model

Cantilever-beam deflection equation selected based on the final loading arrangement.


### Algebraic Solution

Design requirement:

\[
\delta \leq 0.005\text{ in}
\]


### Numerical Solution

TBD


### Required Dimension from Stiffness

\[
\boxed{\text{Feature A stiffness-based dimension = TBD}}
\]


---

## Feature B – Axially Loaded Bar

### Known Values

- Feature B is modeled as an axially loaded bar.
- Maximum allowable deflection:

\[
\delta_{max} = 0.005\text{ in}
\]

- Material elastic modulus:

\[
E = \text{TBD}
\]

- Axial load:

\[
P = \text{TBD}
\]


### Unknown Values

- Required cross-sectional area.
- Required Feature B dimensions.
- Axial deformation.


### Assumptions

- Feature B carries axial loading.
- Material remains linear-elastic.
- Cross-sectional area is constant.
- Load acts through the centroid.


### Free Body Diagram

<!-- Insert Feature B stiffness-analysis FBD here -->


### Deflection Model

Axial deformation:

\[
\delta = \frac{PL}{AE}
\]


### Algebraic Solution

Design requirement:

\[
\frac{PL}{AE} \leq 0.005\text{ in}
\]


### Numerical Solution

TBD


### Required Dimension from Stiffness

\[
\boxed{\text{Feature B stiffness-based dimension = TBD}}
\]


---

## Feature C – Simply Supported Beam

### Known Values

- Feature C is modeled as a simply supported beam.
- Concentrated load acts at the center.
- Maximum allowable deflection:

\[
\delta_{max} = 0.005\text{ in}
\]

- Elastic modulus:

\[
E = \text{TBD}
\]


### Unknown Values

- Required cross-sectional dimensions.
- Area moment of inertia.
- Maximum beam deflection.


### Assumptions

- Feature C behaves as a simply supported beam.
- Load is concentrated at the center of the span.
- Material remains linear-elastic.
- Shear deflection is negligible.
- Cross-section is constant.


### Free Body Diagram

<!-- Insert Feature C stiffness-analysis FBD here -->


### Deflection Model

For a simply supported beam with a concentrated center load:

\[
\delta_{max} = \frac{PL^3}{48EI}
\]


### Algebraic Solution

Design requirement:

\[
\frac{PL^3}{48EI} \leq 0.005\text{ in}
\]


### Numerical Solution

TBD


### Required Dimension from Stiffness

\[
\boxed{\text{Feature C stiffness-based dimension = TBD}}
\]


---

## Feature D – Structural Feature

### Known Values

- Maximum allowable deflection:

\[
\delta_{max} = 0.005\text{ in}
\]

- Material elastic modulus:

\[
E = \text{TBD}
\]

- Loading is transferred from Feature C.


### Unknown Values

- Appropriate deflection model.
- Required Feature D dimension.
- Maximum Feature D deflection.


### Assumptions

- Material remains linear-elastic.
- Small-deflection theory applies.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature D stiffness-analysis FBD here -->


### Deflection Model

TBD


### Algebraic Solution

Design requirement:

\[
\delta_D \leq 0.005\text{ in}
\]


### Numerical Solution

TBD


### Required Dimension from Stiffness

\[
\boxed{\text{Feature D stiffness-based dimension = TBD}}
\]


---

## Feature E – Structural Feature

### Known Values

- Maximum allowable deflection:

\[
\delta_{max} = 0.005\text{ in}
\]

- Material elastic modulus:

\[
E = \text{TBD}
\]

- Loading is transferred from the preceding features.


### Unknown Values

- Appropriate deflection model.
- Required Feature E dimension.
- Maximum Feature E deflection.


### Assumptions

- Material remains linear-elastic.
- Small-deflection theory applies.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature E stiffness-analysis FBD here -->


### Deflection Model

TBD


### Algebraic Solution

Design requirement:

\[
\delta_E \leq 0.005\text{ in}
\]


### Numerical Solution

TBD


### Required Dimension from Stiffness

\[
\boxed{\text{Feature E stiffness-based dimension = TBD}}
\]


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part III – Final Bracket Dimensions

The final dimension of each feature will be selected by comparing its minimum dimension obtained from the stress analysis with its minimum dimension obtained from the stiffness analysis.

The larger required dimension will govern the final design.

## Stress vs. Stiffness Comparison

| Feature | Stress Requirement | Stiffness Requirement | Final Dimension | Governing Criterion |
|---------|-------------------|-----------------------|-----------------|--------------------|
| A | TBD | TBD | TBD | TBD |
| B | TBD | TBD | TBD | TBD |
| C | TBD | TBD | TBD | TBD |
| D | TBD | TBD | TBD | TBD |
| E | TBD | TBD | TBD | TBD |

### Final Selected Dimensions

- **Feature A:** TBD
- **Feature B:** TBD
- **Feature C:** TBD
- **Feature D:** TBD
- **Feature E:** TBD


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part IV – Multiview Sketches

Two separate detailed multiview sketches are required:

1. A bracket sized according to the stress analysis.
2. A bracket sized according to the stiffness analysis.


## Stress-Based Design

### Stress Analysis Multiview Sketch

<!-- Insert stress-based multiview sketch here -->


## Stiffness-Based Design

### Stiffness Analysis Multiview Sketch

<!-- Insert stiffness-based multiview sketch here -->


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part V – Linkage and Fits

## Linkage Design

The linkage connects Feature A of the bracket to a second cylindrical feature.

The connection must safely carry the same applied force acting on Feature A.

### Link Design Requirements

- Link must connect Feature A to a cylindrical 1-inch diameter shaft.
- The connection at Feature A must use a **running/sliding fit**.
- The connection at the 1-inch diameter shaft must use a fit requiring **light assembly pressure**.
- Link dimensions must be verified using both stress and axial deflection.
- The smallest cross-sectional area occurs at the holes and must be considered in the analysis.
- Fit selection must be supported using appropriate engineering fit tables.
- Manufacturing methods used to produce the required fits must be identified.
- Sources used for fit selection must include page numbers.


### Material Selection

The linkage must be manufactured from one of the three specified metals:

- Aluminum 6061-T6
- ASTM A36 Steel
- Titanium Ti-6Al-4V

**Selected Link Material:** TBD


### Known Values

- Applied force:

\[
F = \text{TBD lbf}
\]

- Safety factor:

\[
SF = 4
\]

- Second shaft nominal diameter:

\[
D = 1.000\text{ in}
\]

- Feature A connection requires a running/sliding fit.
- 1-inch shaft connection requires light assembly pressure.
- Link contains two holes.
- Critical cross-sectional regions occur adjacent to the holes.


### Assumptions

- Link is primarily loaded axially.
- Load acts along the longitudinal axis of the link.
- The minimum net area at the holes governs the axial stress calculation.
- Material remains within the elastic range.
- Stress concentrations around the holes are neglected in the preliminary nominal-stress calculation unless otherwise required.


## Link Stress Analysis

### Critical Cross-Section at the Holes

For a link of width \(w\), thickness \(t\), and hole diameter \(d\), the net cross-sectional area may be represented as:

\[
A_{net} = (w-d)t
\]

The smallest net section will be used for the strength analysis.


### Required Cross-Sectional Area

Normal stress:

\[
\sigma = \frac{P}{A_{net}}
\]

Allowable stress:

\[
\sigma_{allow} = \frac{S_y}{SF}
\]

Design requirement:

\[
\frac{P}{A_{net}} \leq \frac{S_y}{SF}
\]


### Algebraic Solution

TBD


### Numerical Solution

TBD


## Link Stiffness Analysis

### Axial Deflection Model

Axial deflection:

\[
\delta = \frac{PL}{AE}
\]


### Required Cross-Sectional Area

The minimum cross-sectional area at the holes will be used when evaluating the stiffness of the link.


### Required Link Length

Link length:

\[
L = \text{TBD}
\]


### Numerical Solution

TBD


---

## Feature A Running / Sliding Fit

### Fit Requirements

The hole connecting the linkage to Feature A must allow relative motion and therefore requires a **running/sliding fit**.

Feature A nominal diameter:

\[
D_A = \text{TBD}
\]


### Fit Selection Process

A standard limits-and-fits table will be used to select an appropriate running/sliding fit for the final diameter of Feature A.


### Selected Fit

TBD


### Hole and Shaft Limits

**Nominal Size:** TBD

**Hole limits:** TBD

**Shaft limits:** TBD

**Maximum clearance:** TBD

**Minimum clearance:** TBD


### Manufacturing Method

TBD after fit tolerances are determined.


### Fit Tables Used

TBD — include source and page number.


---

## 1-Inch Shaft Light Assembly Fit

### Fit Requirements

Nominal shaft diameter:

\[
D = 1.000\text{ in}
\]

The connection must require **light assembly pressure**.


### Fit Selection Process

A standard limits-and-fits table will be used to select the appropriate fit classification and corresponding shaft/hole tolerances.


### Selected Fit

TBD


### Hole and Shaft Limits

**Nominal Size:**

\[
1.000\text{ in}
\]

**Hole limits:** TBD

**Shaft limits:** TBD

**Maximum interference/clearance:** TBD

**Minimum interference/clearance:** TBD


### Manufacturing Method

TBD after fit tolerances are determined.


### Fit Tables Used

TBD — include source and page number.


---

## Final Linkage Design

### Final Link Dimensions

- Link thickness: TBD
- Link width: TBD
- Hole spacing: TBD
- Feature A hole diameter: TBD
- 1-inch shaft hole diameter/tolerance: TBD


### Final CAD Model

<!-- Insert final linkage CAD image here -->


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part VI – Engineering Lessons Learned

## Governing Failure Mode

### Stress vs. Stiffness

For at least one feature, compare the minimum dimension obtained from the stress analysis with the minimum dimension obtained from the stiffness analysis.

Example format:

- Stress required: TBD
- Stiffness required: TBD
- Final selected dimension: TBD
- Governing requirement: TBD


## Error Propagation

Identify one instance where a dimension, force, or other value obtained from an earlier feature was carried into a later analysis.

Discuss whether an error in the earlier value would affect downstream calculations and identify the check used to prevent or identify the error.


## Assumption Sensitivity

Evaluate at least one assumption used during the design.

Possible assumptions include:

- Material selection
- Neglecting direct shear failure
- Neglecting shear deflection
- Symmetric load distribution
- Linear-elastic material behavior
- Idealized beam or bar models

Discuss how changing the assumption would affect the required dimensions.


## Additional Engineering Lessons Learned

TBD after completion of the design.


---

# Final Design

## Final Bracket Model

<!-- Insert final CAD model here -->


## Final Dimensions

| Feature | Final Dimension |
|---------|-----------------|
| A | TBD |
| B | TBD |
| C | TBD |
| D | TBD |
| E | TBD |


## Design Summary

TBD after completing the stress, stiffness, and fit analyses.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Time Spent

| Task | Time |
|------|------|
| Research and Planning | |
| Stress Analysis | |
| Stiffness Analysis | |
| Fits Analysis | |
| CAD / Sketching | |
| Documentation | |
| **Total** | |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# References

1. TBD
2. TBD
3. TBD

