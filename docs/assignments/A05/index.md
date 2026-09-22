# Bracket Design – Stress, Stiffness, and Fits Analysis

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Project Overview

### Objectives

- Conduct stress analysis to determine appropriate dimensions for the structural features.
- Generate free body diagrams (FBDs) for each feature.
- Identify known values, unknown values, assumptions, and algebraic models.
- Perform stiffness analysis to determine minimum dimensions based on deflection.
- Compare stress and stiffness requirements to determine final dimensions.
- Generate multiview sketches for both stress-based and stiffness-based designs.
- Design the linkage connecting Feature A to the 1-inch shaft.
- Determine the proper engineering fits and manufacturing methods.
- Document engineering lessons learned throughout the design process.


### Design Requirements

- Applied Load: 500 lbf < F < 800 lbf
- Safety Factor: SF = 4
- Maximum Allowable Deflection: 0.005 in
- Assume no failure due to direct shear stress.
- Shear deflection is assumed negligible.
- The bracket should be designed symmetrically where practical.
- Five structural features must be analyzed: A, B, C, D, and E.
- Each feature must be evaluated using both stress and stiffness analysis.


### Given Parameters

**Applied Load:**  
F = TBD lbf

**Safety Factor:**  
SF = 4

**Maximum Allowable Deflection:**  
δmax = 0.005 in

**Rigid T-Beam Dimensions:**

- a = 0.498 in (+0.000 / -0.001)
- b = 0.9992 in (+0.0000 / -0.0005)
- c = 1.499 in (+0.000 / -0.001)

**T-Beam Fit Requirements:**

- Dimension a: Accuracy is not essential.
- Dimension b: Close fit that can be expected to run freely.
- Dimension c: Accurate location with minimum play is desired.


### Material Selection

Available materials:

- Aluminum 6061-T6
- ASTM A36 Steel
- Titanium Ti-6Al-4V

**Selected Material:** TBD

**Yield Strength, Sy:** TBD

**Elastic Modulus, E:** TBD


### Initial Assumptions

- Material is homogeneous and isotropic.
- Material behavior is linear-elastic.
- The bracket remains within the elastic region.
- Small-deflection theory is applicable.
- Direct shear failure is neglected as specified.
- Shear deflection is negligible.
- Strap loading is symmetric.
- Stress concentrations are neglected for initial sizing unless otherwise required.
- Feature A is treated as a cantilever beam.
- Feature B is treated as an axially loaded bar.
- Feature C is treated as a simply supported beam with a concentrated center load.
- Loads and dimensions from earlier features may affect later features.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part I – Stress Analysis

**Allowable Stress Equation:**  
σallow = Sy / SF


## Feature A – Cantilever Beam

### Known Values

- Applied Load: F = TBD lbf
- Safety Factor: SF = 4
- Selected Material: TBD
- Yield Strength: Sy = TBD
- Feature A is treated as a cantilever beam.
- Strap loading is symmetric.
- Direct shear failure is neglected.


### Unknown Values

- Required Feature A dimension
- Maximum bending stress
- Maximum bending moment
- Support reaction force
- Support reaction moment


### Assumptions

- Feature A behaves as a cantilever beam.
- Cross-section is constant.
- Material remains linear-elastic.
- Loading is symmetric.
- Direct shear failure is neglected.
- Stress concentrations are neglected for initial sizing.


### Free Body Diagram

<!-- Insert Feature A FBD here -->


### Algebraic Model

Allowable Stress:

σallow = Sy / SF

Maximum Bending Stress:

σmax = Mmax / Z

Design Requirement:

σmax ≤ σallow


### Numerical Solution

TBD


### Required Dimension from Stress

**Feature A Stress-Based Dimension:** TBD


---

## Feature B – Axially Loaded Bar

### Known Values

- Feature B is treated as an axially loaded bar.
- Load is transferred from Feature A.
- Safety Factor: SF = 4
- Selected Material: TBD
- Yield Strength: Sy = TBD
- Direct shear failure is neglected.


### Unknown Values

- Axial load, P
- Required cross-sectional area
- Required Feature B dimension
- Normal stress


### Assumptions

- Feature B carries primarily axial loading.
- Load acts through the centroid.
- Bending is neglected.
- Cross-section is constant.
- Material remains linear-elastic.


### Free Body Diagram

<!-- Insert Feature B FBD here -->


### Algebraic Model

Normal Stress:

σ = P / A

Allowable Stress:

σallow = Sy / SF

Design Requirement:

P / A ≤ Sy / SF


### Numerical Solution

TBD


### Required Dimension from Stress

**Feature B Stress-Based Dimension:** TBD


---

## Feature C – Simply Supported Beam

### Known Values

- Feature C is treated as a simply supported beam.
- A concentrated load acts at the center.
- Load is transferred from the previous feature.
- Safety Factor: SF = 4
- Selected Material: TBD
- Yield Strength: Sy = TBD
- Direct shear failure is neglected.


### Unknown Values

- Support reactions
- Maximum bending moment
- Maximum bending stress
- Required Feature C dimension


### Assumptions

- Feature C behaves as a simply supported beam.
- Load acts at the center of the span.
- Cross-section is constant.
- Material remains linear-elastic.
- Direct shear failure is neglected.


### Free Body Diagram

<!-- Insert Feature C FBD here -->


### Algebraic Model

Support Reactions:

RA = RB = P / 2

Maximum Bending Moment:

Mmax = PL / 4

Maximum Bending Stress:

σmax = Mmax / Z

Design Requirement:

σmax ≤ Sy / SF


### Numerical Solution

TBD


### Required Dimension from Stress

**Feature C Stress-Based Dimension:** TBD


---

## Feature D – Structural Feature

### Known Values

- Load is transferred from Feature C.
- Safety Factor: SF = 4
- Selected Material: TBD
- Yield Strength: Sy = TBD
- Direct shear failure is neglected.


### Unknown Values

- Applied load
- Appropriate structural model
- Maximum stress
- Required Feature D dimension


### Assumptions

- Material remains linear-elastic.
- Direct shear failure is neglected.
- Loading model will be determined from the bracket geometry and load path.


### Free Body Diagram

<!-- Insert Feature D FBD here -->


### Algebraic Model

TBD


### Numerical Solution

TBD


### Required Dimension from Stress

**Feature D Stress-Based Dimension:** TBD


---

## Feature E – Structural Feature

### Known Values

- Load is transferred through the previous bracket features.
- Safety Factor: SF = 4
- Selected Material: TBD
- Yield Strength: Sy = TBD
- Direct shear failure is neglected.


### Unknown Values

- Applied load
- Appropriate structural model
- Maximum stress
- Required Feature E dimension


### Assumptions

- Material remains linear-elastic.
- Direct shear failure is neglected.
- Loading model will be determined from the bracket geometry and load path.


### Free Body Diagram

<!-- Insert Feature E FBD here -->


### Algebraic Model

TBD


### Numerical Solution

TBD


### Required Dimension from Stress

**Feature E Stress-Based Dimension:** TBD


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part II – Stiffness Analysis

**Maximum Allowable Deflection:** 0.005 in

**Assume shear deflections are negligible.**


## Feature A – Cantilever Beam

### Known Values

- Applied Load: F = TBD lbf
- Maximum Allowable Deflection: 0.005 in
- Elastic Modulus: E = TBD
- Feature A is treated as a cantilever beam.


### Unknown Values

- Required Feature A dimension
- Area moment of inertia, I
- Maximum deflection


### Assumptions

- Small-deflection beam theory applies.
- Material remains linear-elastic.
- Cross-section is constant.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature A stiffness FBD here -->


### Deflection Model

Cantilever beam deflection equation will be selected based on the final loading arrangement.


### Algebraic Solution

Design Requirement:

δ ≤ 0.005 in


### Numerical Solution

TBD


### Required Dimension from Stiffness

**Feature A Stiffness-Based Dimension:** TBD


---

## Feature B – Axially Loaded Bar

### Known Values

- Maximum Allowable Deflection: 0.005 in
- Elastic Modulus: E = TBD
- Axial Load: P = TBD
- Feature B is treated as an axially loaded bar.


### Unknown Values

- Required cross-sectional area
- Required Feature B dimension
- Axial deformation


### Assumptions

- Feature B carries axial loading.
- Material remains linear-elastic.
- Cross-section is constant.
- Load acts through the centroid.


### Free Body Diagram

<!-- Insert Feature B stiffness FBD here -->


### Deflection Model

Axial Deflection:

δ = PL / AE


### Algebraic Solution

Design Requirement:

PL / AE ≤ 0.005 in


### Numerical Solution

TBD


### Required Dimension from Stiffness

**Feature B Stiffness-Based Dimension:** TBD


---

## Feature C – Simply Supported Beam

### Known Values

- Feature C is treated as a simply supported beam.
- Concentrated load acts at the center.
- Maximum Allowable Deflection: 0.005 in
- Elastic Modulus: E = TBD


### Unknown Values

- Required Feature C dimension
- Area moment of inertia, I
- Maximum deflection


### Assumptions

- Feature C behaves as a simply supported beam.
- Load acts at the center.
- Material remains linear-elastic.
- Cross-section is constant.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature C stiffness FBD here -->


### Deflection Model

Maximum Deflection:

δmax = PL³ / 48EI


### Algebraic Solution

Design Requirement:

PL³ / 48EI ≤ 0.005 in


### Numerical Solution

TBD


### Required Dimension from Stiffness

**Feature C Stiffness-Based Dimension:** TBD


---

## Feature D – Structural Feature

### Known Values

- Maximum Allowable Deflection: 0.005 in
- Elastic Modulus: E = TBD
- Load is transferred from Feature C.


### Unknown Values

- Appropriate deflection model
- Required Feature D dimension
- Maximum deflection


### Assumptions

- Material remains linear-elastic.
- Small-deflection theory applies.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature D stiffness FBD here -->


### Deflection Model

TBD


### Algebraic Solution

Design Requirement:

δD ≤ 0.005 in


### Numerical Solution

TBD


### Required Dimension from Stiffness

**Feature D Stiffness-Based Dimension:** TBD


---

## Feature E – Structural Feature

### Known Values

- Maximum Allowable Deflection: 0.005 in
- Elastic Modulus: E = TBD
- Load is transferred from the preceding features.


### Unknown Values

- Appropriate deflection model
- Required Feature E dimension
- Maximum deflection


### Assumptions

- Material remains linear-elastic.
- Small-deflection theory applies.
- Shear deflection is negligible.


### Free Body Diagram

<!-- Insert Feature E stiffness FBD here -->


### Deflection Model

TBD


### Algebraic Solution

Design Requirement:

δE ≤ 0.005 in


### Numerical Solution

TBD


### Required Dimension from Stiffness

**Feature E Stiffness-Based Dimension:** TBD


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part III – Final Bracket Dimensions

The final dimension of each feature will be determined by comparing the minimum dimension required by stress with the minimum dimension required by stiffness.

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

Two separate detailed multiview sketches will be generated:

1. Stress-based bracket design
2. Stiffness-based bracket design


## Stress-Based Design

### Stress Analysis Multiview Sketch

<!-- Insert stress-based multiview sketch here -->


## Stiffness-Based Design

### Stiffness Analysis Multiview Sketch

<!-- Insert stiffness-based multiview sketch here -->


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part V – Linkage and Fits

## Linkage Design

The linkage connects Feature A to a second cylindrical feature and must safely support the same applied force.


### Link Design Requirements

- The link connects Feature A to a 1-inch diameter shaft.
- The Feature A connection requires a running/sliding fit.
- The 1-inch shaft connection requires light assembly pressure.
- Link dimensions must be verified using stress and axial deflection.
- The smallest cross-sectional areas at the holes must be analyzed.
- Engineering fit tables must be used to select the fits.
- Manufacturing methods must be selected for each fit.
- Sources and page numbers must be documented.


### Material Selection

Available materials:

- Aluminum 6061-T6
- ASTM A36 Steel
- Titanium Ti-6Al-4V

**Selected Link Material:** TBD


### Known Values

- Applied Load: F = TBD lbf
- Safety Factor: SF = 4
- Shaft Nominal Diameter: 1.000 in
- Feature A connection requires a running/sliding fit.
- 1-inch shaft connection requires light assembly pressure.


### Assumptions

- The link is primarily axially loaded.
- Load acts along the longitudinal axis of the link.
- The smallest net area at the holes governs the stress analysis.
- Material remains linear-elastic.
- Stress concentrations are initially neglected.


## Link Stress Analysis

### Critical Cross-Section at the Holes

For link width w, thickness t, and hole diameter d:

Anet = (w - d)t


### Required Cross-Sectional Area

Normal Stress:

σ = P / Anet

Allowable Stress:

σallow = Sy / SF

Design Requirement:

P / Anet ≤ Sy / SF


### Algebraic Solution

TBD


### Numerical Solution

TBD


## Link Stiffness Analysis

### Axial Deflection Model

δ = PL / AE


### Required Cross-Sectional Area

The minimum net cross-sectional area near the holes will be considered when evaluating linkage stiffness.


### Required Link Length

L = TBD


### Numerical Solution

TBD


---

## Feature A Running / Sliding Fit

### Fit Requirements

The hole connecting the linkage to Feature A must allow relative motion and requires a running/sliding fit.

**Feature A Nominal Diameter:** TBD


### Fit Selection Process

A standard limits-and-fits table will be used to determine the appropriate running/sliding fit.


### Selected Fit

TBD


### Hole and Shaft Limits

- Nominal Size: TBD
- Hole Minimum: TBD
- Hole Maximum: TBD
- Shaft Minimum: TBD
- Shaft Maximum: TBD
- Minimum Clearance: TBD
- Maximum Clearance: TBD


### Manufacturing Method

TBD


### Fit Tables Used

TBD – Include source and page number.


---

## 1-Inch Shaft Light Assembly Fit

### Fit Requirements

**Nominal Shaft Diameter:** 1.000 in

The fit must require light assembly pressure.


### Fit Selection Process

A standard limits-and-fits table will be used to determine the appropriate fit.


### Selected Fit

TBD


### Hole and Shaft Limits

- Nominal Size: 1.000 in
- Hole Minimum: TBD
- Hole Maximum: TBD
- Shaft Minimum: TBD
- Shaft Maximum: TBD
- Minimum Interference/Clearance: TBD
- Maximum Interference/Clearance: TBD


### Manufacturing Method

TBD


### Fit Tables Used

TBD – Include source and page number.


---

## Final Linkage Design

### Final Link Dimensions

- Link Thickness: TBD
- Link Width: TBD
- Hole Spacing: TBD
- Feature A Hole Diameter: TBD
- 1-Inch Shaft Hole Diameter: TBD


### Final CAD Model

<!-- Insert final linkage CAD image here -->


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Part VI – Engineering Lessons Learned

## Governing Failure Mode

### Stress vs. Stiffness

Compare the stress-based and stiffness-based dimensions for at least one feature.

- Stress Required: TBD
- Stiffness Required: TBD
- Final Selected Dimension: TBD
- Governing Requirement: TBD


## Error Propagation

Identify one instance where a force, dimension, or result from an earlier feature was carried into a later feature.

Discuss how an error in the earlier value could affect later calculations and what check was used to identify or prevent the error.


## Assumption Sensitivity

Evaluate at least one assumption made during the design.

Possible assumptions include:

- Material selection
- Neglecting direct shear failure
- Neglecting shear deflection
- Symmetric load distribution
- Linear-elastic behavior
- Idealized beam or bar models

Discuss how changing the assumption would affect the final dimensions.


## Additional Engineering Lessons Learned

TBD


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

TBD


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
