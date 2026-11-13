# 3x3 Microstrip Patch Antenna Array with Beam Steering (2.8 GHz)

## Overview
This repository contains the Ansys HFSS simulation files for a 3x3 probe-fed microstrip patch antenna array designed to operate at 2.8 GHz. The project demonstrates electronic beam steering using progressive phase shifts.

## Technical Specifications
*   **Software:** Ansys HFSS
*   **Operating Frequency:** 2.8 GHz
*   **Substrate Thickness:** 0.78 mm
*   **Element Spacing:**  79 mm
*   **Solver:** Finite Array Domain Decomposition Method (FADDM)
*   **Broadside Gain:** 7.96 dBi (at Theta = 0°).
*    **S11 / Return Loss:** -15.98 dB at 2.888 GHz


## Project Details
1.  **Unit Cell Design:** A single probe-fed patch was designed for 2.8 GHz
2.  **Array Construction:** Lattice pairs (Master/Slave boundaries) were assigned to the airbox side faces to define the periodicity.
3.  **Beam Steering:** A Source Group was created for all 9 ports. By applying a phase gradient (0°, 90°, 180°) to the columns, the main beam was steered

<img width="562" height="387" alt="3D_gain_plot" src="https://github.com/user-attachments/assets/5b4c0edf-9016-4276-94d9-26c32c3361b5" />
<img width="516" height="398" alt="image" src="https://github.com/user-attachments/assets/7a15dd4f-ec42-4e11-b53d-cf2144c47f84" />
<img width="1643" height="578" alt="S11_plot" src="https://github.com/user-attachments/assets/bb389248-6947-4aa5-8df2-1dd4f8c0b7dc" />


## How to Use
1. Clone the repository.
2. Open the `.aedt` file in Ansys HFSS (2023 or newer recommended).
3. Run the `Setup1` analysis.
4. View the `SourceGroup1` 3D Polar Plots to see the broadside and steered beams.

Disclaimer: The primary focus of this simulation was to validate the beam-steering algorithm using progressive phase shifts. The geometry and radiation parameters are not fully optimized for maximum gain or production-level efficiency, which will be addressed in future design iterations.
