# A3 – Parametric Bar Design

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">
## Objectives

- Design a bar using axial deflection
- Use parametric design to determine bar length
- Perform finite element analysis
- Compare analytical and FEA results
- **NOTE: Assignment says to make a circular c.s. bar, but later requests for thickness and side length, for consistency I will be making a circular c.s. bar.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 1. Parametric Design

### Initial Design Parameters

<img width="2195" height="1585" alt="Screenshot 2026-09-09 205601" src="https://github.com/user-attachments/assets/e92e7bb5-b603-42e8-a687-260bdc7551cf" />


- I chose a load value of 300lbf, an elastic modulus of 10e+6 psi and a diameter of a quarter inch. With these calculations I solved for a cross-sectional area of 0.049 in^2. Using this area and the given deflection of 0.009" I solved for the required length of the bar to be 14.73" in length. 


### CAD Model

<img width="2770" height="1590" alt="Screenshot 2026-09-09 202912" src="https://github.com/user-attachments/assets/84bfc1d1-f65e-49f4-80d1-a35aad41024f" />


- Figure above shows CAD model after sketching, extruding and assigning parameter values that were calculated in the initial design process. The parametric model allows you to change values such as length and area to see changes in strain.
  
---
### Material Selection

<img width="1217" height="956" alt="Screenshot 2026-09-09 213901" src="https://github.com/user-attachments/assets/123c2350-88f1-4676-b183-ffa90576c5f8" />

- Changing the material of the model to alumunum and confirming that the elasticity modulus matchest our chosen value (10e+6 psi)

---

### Finite Element Analysis Simulation Setup
<img width="3044" height="1883" alt="Screenshot 2026-09-09 204451" src="https://github.com/user-attachments/assets/462af909-a629-43a5-a340-b57381f8cc3e" />

- The next procedure consisted of conducting a finite element analysis of the model. I statically restrained one end of the bar and applied my chosen normal force (300lbf) to the other end of the bar. Next, we mesh the bar using polygons and run our simulation.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 2. Finite Element Analysis 

### Deflection Map

<img width="3047" height="1891" alt="Screenshot 2026-09-09 214732" src="https://github.com/user-attachments/assets/a459d93d-d656-4714-9938-f79fff81278d" />

- Max displacement from simulation =~ 0.00899" as expected

---

### von Mises Stress

<img width="2995" height="1536" alt="image" src="https://github.com/user-attachments/assets/4701a09b-a11c-42de-a1d2-3f57cd95ba48" />

- Theoretical axial stress =~ 6.47 ksi 

---

### Factor of Safety

**N = S/SIGMA = 40/6.47 = 6.18** 

- Note safety factor of 6.18 = N > 1

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 3. Design Reflection

### Hand Calculation vs. FEA

<img width="2023" height="1239" alt="image" src="https://github.com/user-attachments/assets/0f8dfaf3-0729-4387-83f3-d2a2bc9ac018" />

- No meaningful discrepancy, any difference is likely from rounding. The bar has a uniform cross-section and carries a simple load. I would trust hand calculations vs. a simulation for an axially loaded bar like this due to the accuracy of the equation and lack of possible discrepancies.  

---

### Stress Concentration From Pin Hole

<img width="1198" height="871" alt="Screenshot 2026-09-09 230123" src="https://github.com/user-attachments/assets/8c1add1e-7c38-4594-938a-604732efbe13" />

- Assuming pin hole that has a diameter of half the bar, and from the Peterson-type chart for a flat bar with a transverse hole in tension, the net-section stress concentration factor at d/W=0.50 is approximately 2.16. Peak stress would calculate to 27.9 ksi and our safety factor N = 1.43, still amounting above a factor of 1.

---

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Extra: Modify Design Parameters

"Cycle through #2, change each of the design parameters which include load, thickness, height and width. Keep the material and the fixture the same.

Before you calculate, take a guess if the length will increase, decrease, or stay the same. (You will not be penalized for guessing incorrectly.)"

- Given our formula for overall length **L = XAE / P**, increasing any of the values in the numerator will increase length, while increasing the force will decrease the length.

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 4. Lessons Learned

- Before this project, I had never used Solidworks or simulated a FEA analysis. I also learned how hand calculations can be verified with an FEA analysis and when a object has a more complex shape, using mesh is more helpful than hand calculations. 

### Time Spent

| Activity | Time Spent(hrs) |
| --- | ---: |
| Parametric Design | 1 |
| FEA | 0.5 |
| Analysis & Reflection | 0.5 |
| Website | 2 |
| **Total** | **4** |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Sources
