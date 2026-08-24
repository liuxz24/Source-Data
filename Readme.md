markdown
# Source Data for [Tellurium-Assisted Rapid Synthesis of Violet Phosphorus via Solid-Phase Thermal Transformation]

This repository contains the source data supporting the findings of our manuscript. All data are organized to facilitate the reproduction and extension of the figures and computational results presented in the paper.

## Repository Structure
/
├── Source_Data_for_Figures/ # Raw data for all figures
│ ├── Figure_1.xlsx # Source data for Figure 1
│ ├── Figure_2.xlsx # Source data for Figure 2
│ ├── Figure_3.xlsx # Source data for Figure 3
│ ├── Figure_4.xlsx # Source data for Figure 4
│ └── Figure_5.xlsx # Source data for Figure 5
│
└── VASP/ # Input and output files for DFT calculations
├── WP/ # Calculations for WP (with different basis sets)
├── FP/ # Calculations for FP (with different basis sets)
├── VP/ # Calculations for VP (with different basis sets)
├── Te/ # Calculations for Te (with different basis sets)
├── FP-Te/ # FP-Te under PBE-DFTD3
├── FP-vac/ # FP-vac under PBE-DFTD3
├── VP-Te/ # VP-Te under PBE-DFTD3
├── VP-vac/ # VP-vac under PBE-DFTD3
└── Te-vac/ # Te-vac under PBE-DFTD3

## Figure Source Data

The `Source_Data_for_Figures/` folder contains five Microsoft Excel files, each corresponding to the raw data for **Fig. 1–5** in the main text.

- **File naming**: `Figure_1.xlsx` to `Figure_5.xlsx`
- **Sheet structure**: Each **sheet** within a file represents a single sub‑figure (e.g., **Fig.  1C**, **Fig.  2A**, etc.).
- **Content**: Each sheet provides the raw numerical values (e.g., mean, standard deviation, individual data points) used to generate the corresponding plot.

> **How to use**: You can directly open any `.xlsx` file with Microsoft Excel, LibreOffice Calc, or any spreadsheet software to inspect and reproduce the chart data.

---

## VASP Calculation Files

The `VASP/` directory contains all input and output files from our density functional theory (DFT) calculations performed with the VASP code.

### Subdirectory List

The following subdirectories are included:

| Folder       | Description |
|--------------|-------------|
| `WP/`        | Calculations for the WP system with various basis sets. |
| `FP/`        | Calculations for the FP system with various basis sets. |
| `VP/`        | Calculations for the VP system with various basis sets. |
| `Te/`        | Calculations for the Te unit cell with various basis sets. |
| `FP-Te/`     | FP‑Te system under the **PBE‑DFTD3**. |
| `FP-vac/`    | FP‑vacancy system under **PBE‑DFTD3**. |
| `VP-Te/`     | VP‑Te system under **PBE‑DFTD3**. |
| `VP-vac/`    | VP‑vacancy system under **PBE‑DFTD3**. |
| `Te-vac/`    | Te‑vacancy system under **PBE‑DFTD3**. |

### Standard VASP Files

Within each calculation folder, you will find the following standard VASP files:

- **`POSCAR`** – Input crystal structure (atomic positions and lattice vectors).
- **`POTCAR`** – Pseudopotential files used for each element.
- **`KPOINTS`** – k‑point grid and mesh information.
- **`INCAR`** – Main input file specifying calculation parameters (e.g., functional, convergence criteria, spin settings).
- **`CONTCAR`** – Final relaxed atomic positions after the calculation.
- **`OUTCAR`** – Main output file containing total energies, forces, stresses, and other key results.

> **Reproducibility**: All calculations were performed using the same VASP version and pseudopotential set. The input parameters in `INCAR` and `KPOINTS` are fully documented within the respective files.