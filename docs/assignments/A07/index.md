
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

<img width="1835" height="1384" alt="Screenshot 2026-10-21 202454 - Copy - Copy" src="https://github.com/user-attachments/assets/734f626c-d01f-43de-ae74-2ceb879b478a" />


### Mesh Convergence

### Mesh 1 

<img width="2080" height="1323" alt="Screenshot 2026-10-21 202538" src="https://github.com/user-attachments/assets/fe3338a6-8c4e-424a-8e13-bf2371b7bccd" />

<img width="2146" height="1432" alt="Screenshot 2026-10-21 202546" src="https://github.com/user-attachments/assets/45d2cc0c-5518-4745-9c18-fb1ae58ccede" />

<img width="2214" height="1422" alt="Screenshot 2026-10-21 202552" src="https://github.com/user-attachments/assets/48dfd60c-b387-4177-b01d-b36f44de87bd" />

<img width="711" height="583" alt="Screenshot 2026-10-21 202607" src="https://github.com/user-attachments/assets/529aefa6-e67e-4e0d-8734-9d7143e8e502" />


### Mesh 2

<img width="2302" height="1415" alt="Screenshot 2026-10-21 202824" src="https://github.com/user-attachments/assets/29d3edc7-c884-4d70-aa78-c03588bbd405" />

<img width="2087" height="1358" alt="Screenshot 2026-10-21 202827" src="https://github.com/user-attachments/assets/886edb0a-5b1f-4ed2-ae94-cc671ecd7216" />

<img width="2211" height="1399" alt="Screenshot 2026-10-21 202831" src="https://github.com/user-attachments/assets/e47af265-7a1d-490b-99ff-877668d2b86f" />

<img width="870" height="612" alt="Screenshot 2026-10-21 202846" src="https://github.com/user-attachments/assets/44566171-3f5a-4269-aa2b-53a9868942e7" />


### Mesh 3

<img width="2274" height="1408" alt="Screenshot 2026-10-21 203149" src="https://github.com/user-attachments/assets/e5d1f48b-e587-4bfb-aa3c-8a0d4191ad41" />

<img width="2130" height="1420" alt="Screenshot 2026-10-21 203153" src="https://github.com/user-attachments/assets/2be77559-948c-4c96-8ec6-7ddf21c7b318" />

<img width="2138" height="1359" alt="Screenshot 2026-10-21 203157" src="https://github.com/user-attachments/assets/ef383252-be57-44e2-99a9-25de15cee8a0" />

<img width="869" height="601" alt="Screenshot 2026-10-21 203205" src="https://github.com/user-attachments/assets/be760032-34a1-40f2-8078-e4d9a095b407" />

### Stress and Displacement

<img width="2000" height="1371" alt="Screenshot 2026-10-21 203439" src="https://github.com/user-attachments/assets/72c6330a-0429-4126-9e0a-9d17c9202e04" />

<img width="705" height="1189" alt="Screenshot 2026-10-21 203457" src="https://github.com/user-attachments/assets/67b4fe3c-1f60-43ec-a315-b67099ed7083" />


| Parameter | Result |
|---|---|
| Maximum Stress | 279,340 psi |
| Stress Location | Vertical support near cylinder |
| Maximum Deflection | 0.2893 in |
| Deflection Location | Free end of cylinder |
| Mass | 2.51 lb |
| Safety Factor | 0.1298 |
| Number of Elements | 27,417 |

### Mesh Convergence

| Parameter | Mesh 1 | Mesh 2 | Mesh 3 |
|---|---|---|---|
| Elements | 3,682 | 9,480 | 27,417 |
| Max Stress (MPa) | 1,566 | 1,698 | 1,926 |
| Max Deflection (mm) | 7.021 | 7.215 | 7.348 |

- Stress Convergence: 11.84%
- Deflection Convergence: 1.81%
- Requirement: ≤ 7% (Stress Not Converged)


---

# Design III - Second Modification

<img width="1665" height="1203" alt="Screenshot 2026-10-21 205709" src="https://github.com/user-attachments/assets/b500cfbf-5d09-4bf2-b075-86b7d07fcc69" />

<img width="1246" height="1196" alt="Screenshot 2026-10-21 205717" src="https://github.com/user-attachments/assets/76d9c2a5-e8fc-4227-9c1c-d5b58c04a0cc" />


### Mesh Convergence

### Mesh 1

<img width="2149" height="1449" alt="Screenshot 2026-10-21 205813" src="https://github.com/user-attachments/assets/9a42d9b8-6ae7-40ab-bc16-3c0956438a93" />

<img width="1932" height="1440" alt="Screenshot 2026-10-21 205819" src="https://github.com/user-attachments/assets/e8099af4-5047-4b55-963c-23b91056931e" />

<img width="1948" height="1465" alt="Screenshot 2026-10-21 205822" src="https://github.com/user-attachments/assets/08429b67-c364-41b3-87d6-35f2e9aa9f56" />


### Mesh 2 

<img width="2011" height="1437" alt="Screenshot 2026-10-21 210145" src="https://github.com/user-attachments/assets/46f7f74a-114b-406c-8671-9277b1a40d03" />

<img width="1907" height="1419" alt="Screenshot 2026-10-21 210150" src="https://github.com/user-attachments/assets/48c0fccf-a3ab-40ad-b3df-507e29e5a284" />

<img width="2002" height="1397" alt="Screenshot 2026-10-21 210154" src="https://github.com/user-attachments/assets/ef7a91c2-3312-471c-8dd4-9924977f2a96" />


### Mesh 3

<img width="2076" height="1445" alt="Screenshot 2026-10-21 210326" src="https://github.com/user-attachments/assets/20ab8e01-8e77-4e79-b7e4-5ddaf3c63d69" />

<img width="2017" height="1425" alt="Screenshot 2026-10-21 210329" src="https://github.com/user-attachments/assets/421b9704-d93a-47ea-ad80-54cde55982ec" />

<img width="2044" height="1415" alt="Screenshot 2026-10-21 210333" src="https://github.com/user-attachments/assets/f47284fe-b800-4548-bd9b-e3525827680d" />

<img width="878" height="614" alt="Screenshot 2026-10-21 210453" src="https://github.com/user-attachments/assets/77a82df4-7d85-4836-95b5-e9d91eb6ea40" />


### Stress and Displacement
<!-- Insert simulation images -->

<img width="701" height="1186" alt="Screenshot 2026-10-21 210507" src="https://github.com/user-attachments/assets/157fae03-f31a-4832-ae04-473fefbfcd8b" />

<img width="1828" height="1438" alt="Screenshot 2026-10-21 210525" src="https://github.com/user-attachments/assets/931326e4-cbc6-4a30-b5a6-947ba4e59c36" />

| Parameter | Result |
|---|---|
| Maximum Stress | 251,350 psi |
| Stress Location | Support near cylinder connection |
| Maximum Deflection | 0.2169 in |
| Deflection Location | Free end of cylinder |
| Mass | 2.54 lb |
| Safety Factor | 0.1442 |
| Number of Elements | 28,101 |

### Mesh Convergence

| Parameter | Mesh 1 | Mesh 2 | Mesh 3 |
|---|---|---|---|
| Elements |  |  | 28,101 |
| Max Stress (MPa) | 1,307 | 1,422 | 1,733 |
| Max Deflection (mm) | 5.288 | 5.368 | 5.510 |

- Stress Convergence: 17.95%
- Deflection Convergence: 2.58%
- Requirement: ≤ 7% (Stress Not Converged)

- 
<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">


# Final Design Comparison

| Parameter | Design I | Design II | Design III |
|---|---|---|---|
| Max Stress (psi) | 1,101,850 | 279,340 | 251,350 |
| Max Deflection (in) | 2.064 | 0.2893 | 0.2169 |
| Mass (lb) | 2.47 | 2.51 | 2.54 |
| Safety Factor | 0.03291 | 0.1298 | 0.1442 |
| Number of Elements | 31,849 | 27,417 | 28,101 |


<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">

# Engineering Reflection

### Lessons Learned

### Time Spent
- Total Time:

<hr style="border: none; border-top: 2px solid #888; margin: 30px 0;">
