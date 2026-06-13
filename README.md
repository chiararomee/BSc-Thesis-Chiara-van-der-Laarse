# BSc-Thesis-Chiara-van-der-Laarse
# Thesis Codebase

This repository contains the code used for my Bachelor's thesis on time series anomaly detection.

We evaluate three methods:
- TS-AIDA (baseline method)
- TS-AIDA-FS (Fourier smoothing extension)
- TS-AIDA-DFT (Fourier thresholding in the frequency domain)

In addition, we apply inlier screening to improve computational efficiency.

---

## Repository Structure

The repository is organized by experimental scenario. Each notebook follows the same pipeline:

1. Synthetic dataset generation
2. Fourier Smoothing (FS)
3. Application of anomaly detection methods:
   - TS-AIDA
   - TS-AIDA-FS
   - TS-AIDA-DFT
(4. Inlier screening analysis)
5. Visualization and performance evaluation (figures and tables)

---

## Experiment Notebooks

### DFT_Mixed_Anomalies.ipynb
Generates 4 datasets with mixed anomaly types:
- 2 local anomalies
- 2 structural anomalies

We apply:
- Fourier Smoothing (FS)
- TS-AIDA
- TS-AIDA-FS
- TS-AIDA-DFT
- Inlier screening

Results are presented using figures and performance tables.

---

### DFT_Regime_Shift.ipynb
Same pipeline as above, but applied to datasets containing regime shift anomalies.

---

### DFT_Flash_Crash.ipynb
Same pipeline applied to flash crash datasets.

---

### DFT_HighDrift_VolSpike.ipynb
Experiments on:
- High drift datasets
- Volatility spike datasets

Both follow the same evaluation pipeline.

---

### Thesis_Data_Simulation2.ipynb
This notebook contains:
- Geometric Brownian Motion (GBM) data generation
- Initial definitions of anomaly types

Note: In the DFT experiment notebooks, anomaly definitions are re-implemented for clarity and reproducibility within each scenario.

---

## Notes

- All experiments are reproducible from the provided notebooks.
- Synthetic data generation is included for full reproducibility.
