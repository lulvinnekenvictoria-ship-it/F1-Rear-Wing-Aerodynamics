# F1 Rear Wing – CAD & Aerodynamic Analysis

## Overview
An engineering investigation into the aerodynamic performance of a Formula One-inspired rear wing[cite: 1]. The rear wing of an F1 car is critical for generating downforce and providing stability at high speeds[cite: 1]. This project encompasses parametric CAD modelling, computational fluid dynamics (CFD) using SOLIDWORKS Flow Simulation, and experimental wind-tunnel validation to analyze the relationship between the angle of attack (AOA), drag, and downforce.

## Engineering Objective
To apply airflow visualization and CFD simulation to an F1 rear wing design and compare computational results against experimental wind-tunnel test data to evaluate aerodynamic efficiency and stall characteristics[cite: 1].

## CAD Methodology
*(Placeholder: We will update this section once you provide the SolidWorks FeatureManager Design Tree details from Step 1.)*
*   **Aerodynamic Profiling:**
*   **Parametric Design:** 
*   **Solid Modelling:** 

## CFD Simulation Setup
The computational analysis was conducted using **SOLIDWORKS Flow Simulation**[cite: 1]. A numerical domain and mesh were configured to discretize the fluid body and calculate properties around the wing boundary[cite: 1].

**Simulation Initial Conditions:**
*   **Fluid:** Air[cite: 1]
*   **Velocity:** 30 m/s[cite: 1]
*   **Atmospheric Pressure:** 101325 Pa (Sea level)[cite: 1]
*   **Temperature:** 293.2 K (Room temperature)[cite: 1]

## CFD Results
The CFD simulation analyzed the pressure contour distribution and airflow velocity streamlines at four different angles of attack (10°, 15°, 20°, and 25°)[cite: 1]. As expected, low-pressure zones concentrated on the bottom of the wing, generating the necessary pressure differential for downforce[cite: 1].

| Angle of Attack | Drag Force (N) | Downforce (N) | Drag Coefficient (Cd) |
| :--- | :--- | :--- | :--- |
| **10°** | 3.895 | -6.219 | 1.028 |
| **15°** | 4.750 | -7.623 | 1.023 |
| **20°** | 5.406 | -8.055 | 0.993 |
| **25°** | 5.879 | -7.276 | 1.048 |

**Key Findings:**
*   **Drag:** Increased proportionally as the angle of attack increased from 10° to 25°[cite: 1]. 
*   **Downforce:** The magnitude of downforce increased as the AOA progressed to 20°[cite: 1].
*   **Stall Phenomenon:** At 25° AOA, downforce magnitude decreased, indicating that the wing exceeded its critical angle of attack, resulting in airflow separation (stall)[cite: 1]. 
*   **Efficiency:** The drag coefficient remained relatively consistent (around 1.0), indicating the wing maintained consistent aerodynamic geometry performance across the tested range[cite: 1].

## Experimental Validation (Wind Tunnel)
To validate the computational model, a physical scale model manufactured from PLA was tested in a wind tunnel at a 15° AOA[cite: 1].

**Wind Tunnel Results (15° AOA):**
*   **Drag Force:** 6.17 N[cite: 1]
*   **Downforce:** -14.99 N[cite: 1]
*   **Drag Coefficient:** ~1.13[cite: 1]

### CFD vs. Experimental Discrepancies
The experimental data recorded a higher drag force (6.17 N vs 4.75 N) and a significantly greater magnitude of downforce (-14.99 N vs -7.623 N) compared to the CFD simulation[cite: 1].

**Engineering Analysis of Variance:**
*   **Surface Roughness:** The physical wing was 3D printed using PLA. The layer lines and surface finish of the PLA create a rougher surface than the perfectly smooth boundary conditions assumed in the CAD/CFD model, increasing drag[cite: 1].
*   **Boundary Conditions:** Interference from wind tunnel walls and mounting equipment can alter airflow, artificially affecting downforce measurements[cite: 1].
*   **Mesh Sensitivity:** The discrepancy highlights the high sensitivity of CFD software; slight inaccuracies in the numerical domain size or mesh resolution can heavily influence computational outputs[cite: 1].

## Future Improvements
If this project were to be iterated upon, I would implement:
1.  **Mesh Sensitivity Analysis:** Adjusting the grid resolution and comparing results to ensure mesh independence and capture finer flow details near the boundary layer[cite: 1].
2.  **Material Property Matching:** Applying computational surface roughness parameters that match PLA, or manufacturing the physical model from a material matching the computational assumptions (e.g., carbon fiber/resin)[cite: 1].
3.  **Wind Tunnel Calibration:** Tightening control over the experimental flow conditions to minimize inherent testing errors[cite: 1].
