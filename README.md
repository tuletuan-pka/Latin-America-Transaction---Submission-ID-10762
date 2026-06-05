# Latin-America-Transaction---Submission-ID-10762
This repository contains the supplementary simulation files, raw data, and measurement results associated with our paper entitled "Low-Complexity Single-Layer Dual-Band Microstrip Patch Antenna for WiFi 6/6E Communication Systems". The dataset is provided to ensure reproducibility of the results and to allow researchers to explore the antenna parameters in greater detail.

## 📊 Overview

The files are organized to directly correspond with the figures presented in the manuscript. 
Based on the metrics included in the files (DG, ECC, MEG, TARC), this repository includes performance evaluation data for a Multiple-Input Multiple-Output (MIMO) antenna system.

## 📈 Performance Summary

The proposed single-layer dual-band antenna and its corresponding Multiple-Input Multiple-Output (MIMO) array configuration demonstrate robust performance metrics tailored for WiFi 6/6E communication systems.

### Single Element Performance
* **Operating Frequencies:** The design effectively covers two distinct resonant bands centered around 5.2 GHz and 6.6 GHz.
* **Compact Footprint:** The optimized antenna achieves a low-profile and highly compact structure, occupying an overall electrical size of 0.52 λ × 0.52 λ × 0.03 λ at the lowest operating frequency of 5.2 GHz.
* **Impedance Bandwidth:** Experimental results show measured -10 dB impedance bandwidths of 6.1% (5.12–5.44 GHz) for the lower band and 4.9% (6.40–6.72 GHz) for the upper band.
* **Gain & Efficiency:** The prototype achieves measured peak broadside gains of 7.0 dBi in the lower band and 6.7 dBi in the upper band. Additionally, the antenna yields a high radiation efficiency of better than 88% across both frequency bands.
* **Radiation Characteristics:** The antenna maintains stable, directional broadside radiation featuring a high front-to-back ratio (FBR) of approximately 20 dB. Furthermore, it exhibits stable linear polarization with very low cross-polarization levels, measured at approximately 25 dB lower than the co-polarized components.

### 4 × 4 MIMO Configuration Performance
* **Isolation & Spacing:** To achieve both spatial and polarization diversity, the four elements are arranged orthogonally with a compact edge-to-edge spacing of 3 mm. This arrangement secures port isolations greater than 20 dB across both operating bands.
* **MIMO Peak Gain:** The simulated peak gains for the MIMO configuration reach 6.6 dBi and 6.9 dBi at the lower and higher bands, respectively.
* **Diversity Metrics:** The configuration delivers excellent diversity performance, characterized by an Envelope Correlation Coefficient (ECC) below 0.02 and a Diversity Gain (DG) higher than 9.9 dB. Additionally, the Total Active Reflection Coefficient (TARC) is acceptable over the operating bands, and the Mean Effective Gain (MEG) remains balanced among all ports.

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
