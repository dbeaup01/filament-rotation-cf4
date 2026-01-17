# filament-rotation-cf4
Reproducible analysis notebook for detecting coherent rotation in nearby cosmic filaments using Cosmicflows-4 reconstructed velocity fields and conservative null tests.

# Coherent Rotation in Nearby Cosmic Filaments (Cosmicflows-4)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/dbeaup01/filament-rotation-cf4/blob/main/SFH_Filament_Rotation_CF4_Reproducible.ipynb
)

## Overview

This repository contains the fully reproducible analysis notebook accompanying the paper:

**“Coherent Rotation in Nearby Cosmic Filaments and Its Dependence on Environmental Asymmetry”**

The analysis detects and characterizes coherent, axis-aligned rotational motion in nearby cosmic filaments using reconstructed peculiar-velocity fields from **Cosmicflows-4**. The methodology emphasizes conservative geometry, explicit null tests, and population-level robustness rather than model-dependent interpretation.

This repository is intended to allow independent readers to:
- inspect the full analysis pipeline,
- reproduce all key measurements and null tests,
- and explore filament kinematics using the same assumptions and data handling as in the paper.

---

## Scientific Scope

- **Data:** Cosmicflows-4 reconstructed peculiar velocity field  
- **Objects:** Nearby cosmic filaments (local universe)  
- **Method:** Cylindrical ring sampling around filament spines  
- **Key tests:**
  - Axis-randomization nulls (geometry-destroying)
  - Environment-destroying permutation tests
  - Leave-one-out robustness checks  

The notebook focuses strictly on **observational kinematics**.  
Interpretation is deliberately conservative and does not rely on any specific gravity or cosmological model.

---

## Notebook Structure

The notebook is organized sequentially and heavily commented:

1. **Environment setup**  
   Directory creation, imports, and configuration.

2. **Data loading**  
   Filament skeletons and Cosmicflows-4 velocity field access.

3. **Estimator definition**  
   Cylindrical ring-sampling circulation estimator.

4. **Signal measurement**  
   Segment-level and filament-level rotation proxies.

5. **Null tests**  
   Axis randomization, environment randomization, permutation tests.

6. **Statistical analysis**  
   Correlations with environmental asymmetry metrics.

7. **Validation & robustness**  
   Leave-one-out checks and sanity controls.

Cells explicitly marked *“DO NOT RUN”* are retained for provenance and documentation only.

---

## How to Run

### Option 1 — Google Colab (recommended)
Click the **Open in Colab** badge above and follow the notebook instructions.

### Option 2 — Local execution
Clone the repository and run the notebook in a standard Python environment with:
- `numpy`
- `scipy`
- `pandas`
- `matplotlib`

---

## Notes on Reproducibility

- All randomizations are seeded where appropriate.
- No parameter tuning is performed to enhance signal detection.
- The analysis is local in scope and does not extrapolate beyond the data.

---

## Related Work

This repository is part of a broader set of reproducible analyses exploring cosmic kinematics using observational data.  
Related papers and datasets are available on the author’s Zenodo profile.

---

## Correspondence

**Daniel Beaupré**  
Independent researcher  
GitHub: https://github.com/dbeaup01

---

## License

This project is released for scientific inspection and reuse with attribution.
