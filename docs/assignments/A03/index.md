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

<img width="1217" height="956" alt="Screenshot 2026-09-09 213901" src="https://github.com/user-attachments/assets/123c2350-88f1-4676-b183-ffa90576c5f8" />

- Changing the material of the model to alumunum and confirming that the elasticity modulus matchest our chosen value (10e+6 psi)

---

<img width="3044" height="1883" alt="Screenshot 2026-09-09 204451" src="https://github.com/user-attachments/assets/462af909-a629-43a5-a340-b57381f8cc3e" />

- The next procedure consisted of conducting a finite element analysis of the model. I statically restrained one end of the bar and applied my chosen normal force (300lbf) to the other end of the bar. Next, we mesh the bar using polygons and run our simulation.


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 2. Finite Element Analysis

### Deflection Map

### von Mises Stress

### Factor of Safety

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 3. Design Reflection

### Hand Calculation vs. FEA

### Stress Concentration From Pin Hole

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## 4. Lessons Learned

### Mistakes Made

### Time Spent

| Activity | Time Spent |
| --- | ---: |
| Parametric Design | |
| FEA | |
| Analysis & Reflection | |
| Website | |
| **Total** | ** hrs** |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


## Sources
