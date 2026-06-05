# Latin-America-Transaction---Submission-ID-10762
This repository contains the supplementary simulation files, raw data, and measurement results associated with our paper entitled "Low-Complexity Single-Layer Dual-Band Microstrip Patch Antenna for WiFi 6/6E Communication Systems". The dataset is provided to ensure reproducibility of the results and to allow researchers to explore the antenna parameters in greater detail.

## 📊 Overview

The files are organized to directly correspond with the figures presented in the manuscript. 
Based on the metrics included in the files (DG, ECC, MEG, TARC), this repository includes performance evaluation data for a Multiple-Input Multiple-Output (MIMO) antenna system.

## 🛠 Software Requirements

To fully utilize the files in this repository, you will need:
* **ANSYS Electronics Desktop (HFSS):** Required to open and run the 3D electromagnetic simulation models (`*.aedt` files).
* **Data Processing Tool:** Any tool capable of parsing Comma-Separated Values (CSV) or Text files (e.g., MATLAB, Python (Pandas/Matplotlib), Microsoft Excel, or OriginLab) to plot the antenna performance metrics.

## 📂 Repository Contents

### Simulation Models (`.aedt`)
These files contain the full 3D electromagnetic simulation setups in ANSYS Electronics Desktop:
* `Fig. 1 - sim.aedt` - Initial geometry / reference simulation setup for Figure 1.
* `Fig. 4 - sim.aedt` - Modified geometry / parametric setup for Figure 4.
* `Fig. 13 - sim.aedt` - Final optimized antenna simulation model for Figure 13.

### Parametric Study & Performance Data (`.csv` & `.txt`)
These files contain the exported S-parameters, gain, radiation patterns, or other plotted values corresponding to specific figures in the paper.

* **Figure 2:** `Fig. 2.csv`
* **Figure 3:** Length variations
    * `Fig. 3 - l1.csv`
    * `Fig. 3 - l2.csv`
* **Figure 5:** `Fig. 5.csv`
* **Figure 6:** `Fig. 6.csv`
* **Figure 7:** `Fig. 7.txt`
* **Figure 8:** Distance/dimension variations
    * `Fig. 8 - d1.csv`
    * `Fig. 8 - d2.csv`
* **Figure 9:** `Fig. 9.txt`
* **Figure 10:** `Fig. 10.csv`
* **Figure 11:** `Fig. 11.csv`
* **Figure 12:** Frequency specific analysis (e.g., Radiation Patterns)
    * `Fig. 12 - 5.2 GHz.csv`
    * `Fig. 12 - 6.6 GHz.csv`
* **Figure 14:** `Fig. 14.csv`
* **Figure 15:** `Fig. 15.csv`

### MIMO Diversity Performance Metrics
The following data sets correspond to Figure 16 and capture the calculated MIMO performance criteria of the proposed antenna:
* `Fig. 16(a) - DG.csv`: Diversity Gain (DG)
* `Fig. 16(a) - ECC.csv`: Envelope Correlation Coefficient (ECC)
* `Fig. 16(b) - MEG.csv`: Mean Effective Gain (MEG)
* `Fig. 16(b) - TARC.csv`: Total Active Reflection Coefficient (TARC)

## 🚀 Usage

1.  **To view simulations:** Open ANSYS Electronics Desktop, select File > Open, and choose any of the `.aedt` files. Note that solving these projects may require significant computational resources depending on your mesh settings.
2.  **To plot data:** Import the `.csv` or `.txt` files into your preferred data visualization script or software. The files are structured with headers for easy parsing.
