
# Bracket Finite Element Analysis (FEA)

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

## Project Overview

### Objectives
- Improve bracket strength and stiffness.
- Minimize mass through geometric optimization.
- Validate FEA results through mesh convergence (7%).

### Material and Loading
- Material: ASTM A36 Steel
- Applied Load:
- Constraints:

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# Design I - Original Bracket


<img width="2662" height="1315" alt="Screenshot 2026-10-21 192902" src="https://github.com/user-attachments/assets/bc92992c-a652-46a8-9052-e40fac7a5ff2" />



### Mesh 1 (Course)
<!-- Insert mesh results and calculations -->

<img width="1752" height="1394" alt="Screenshot 2026-10-21 193600" src="https://github.com/user-attachments/assets/e82d0a29-e093-4394-b895-563f987732e9" />

<img width="2796" height="1583" alt="Screenshot 2026-10-21 193606" src="https://github.com/user-attachments/assets/8fea5e8c-9d4d-494e-b1f3-900d6d05f850" />

<img width="2301" height="1455" alt="Screenshot 2026-10-21 194421" src="https://github.com/user-attachments/assets/6f1eebf8-c6f4-415c-9fb6-1c86b1ab65f2" />

<img width="629" height="395" alt="Screenshot 2026-10-21 194237" src="https://github.com/user-attachments/assets/eb3e3332-fa30-472c-9e8c-7028dd6733b5" />



### Mesh 2 (Medium)

<img width="2877" height="1627" alt="Screenshot 2026-10-21 194714" src="https://github.com/user-attachments/assets/bb68089b-26b3-4f77-b24f-a80f04f44ba9" />

<img width="2767" height="1410" alt="Screenshot 2026-10-21 194721" src="https://github.com/user-attachments/assets/ae467100-e7b7-4788-a345-724873f9385e" />

<img width="815" height="615" alt="Screenshot 2026-10-21 194825" src="https://github.com/user-attachments/assets/e414ede6-5706-418f-8476-a8f911959dd3" />



### Mesh 3 (Fine)

<img width="2485" height="1389" alt="Screenshot 2026-10-21 195028" src="https://github.com/user-attachments/assets/21fb44b5-7d3f-42d6-9018-5cf5231b4b5a" />

<img width="2295" height="1295" alt="Screenshot 2026-10-21 195032" src="https://github.com/user-attachments/assets/ab29778c-66ce-4887-b027-2874bc2eb5e0" />

<img width="2120" height="1421" alt="Screenshot 2026-10-21 195036" src="https://github.com/user-attachments/assets/f3d35fb0-75b4-4d29-adde-b919e84a08f4" />

<img width="815" height="620" alt="Screenshot 2026-10-21 195044" src="https://github.com/user-attachments/assets/ed9624e9-15a6-4c46-bfbc-4c8943607cee" />



### Stress and Displacement

<img width="2038" height="1274" alt="Screenshot 2026-10-21 195620" src="https://github.com/user-attachments/assets/e661d94b-6058-419f-be08-6b53c6b95c6b" />

<img width="707" height="1186" alt="Screenshot 2026-10-21 195554" src="https://github.com/user-attachments/assets/5e8fb201-cc42-4856-969b-95f8cf315ed9" />


## Design I - Original Bracket

### FEA Results

| Parameter | Result |
|---|---|
| Maximum Stress | 1,101,850 psi |
| Stress Location | Vertical support near cylinder |
| Maximum Deflection | 2.064 in |
| Deflection Location | Free end of cylinder |
| Mass | 2.47 lb |
| Safety Factor | 0.03291 |
| Number of Elements | 31,849 |

### Mesh Convergence

| Parameter | Mesh 1 | Mesh 2 | Mesh 3 |
|---|---|---|---|
| Elements | 4,694 | 14,955 | 31,849 |
| Max Stress (MPa) | 6,193 | 7,202 | 7,597 |
| Max Deflection (mm) | 49.83 | 51.92 | 52.43 |

- Stress Convergence: 5.20%
- Deflection Convergence: 0.97%
- Requirement: ≤ 7% (Satisfied)




---

# Design II - First Modification

### Geometry Changes

### Mesh Convergence

### Stress and Displacement
<!-- Insert simulation images -->

---

# Design III - Second Modification

### Geometry Changes

### Mesh Convergence

### Stress and Displacement
<!-- Insert simulation images -->

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# Final Design Comparison

| Parameter | Design I | Design II | Design III |
|---|---|---|---|
| Max Stress (psi) | | | |
| Max Deflection (in) | | | |
| Mass (lb) | | | |
| Safety Factor | | | |
| Number of Elements | | | |

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# Engineering Reflection

### Lessons Learned

### Time Spent
- Total Time:

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">
