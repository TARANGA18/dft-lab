# 🔬 My Computational Materials Science & DFT Lab

Welcome to my central repository for first-principles quantum mechanical simulations using Density Functional Theory (DFT). This space serves as a living laboratory where I document my calculations, structural optimizations, and electronic property predictions for various materials.

## 🛠️ Global Methodology & Toolkit
* **Primary DFT Engine:** Quantum ESPRESSO (v7.x) / [Or your chosen software]
* **Approximation Functionals:** GGA-PBE / LDA
* **Pseudopotentials:** [e.g., SSSP Efficiency / PSlibrary]
* **Analysis Tools:** Python (Matplotlib), VESTA (Crystal Visualization), Bash Scripting

---

## 📚 Materials Library & Progress Tracker

| Material Formula | Structure Class | Calculation Status | Key Findings / Target Property |
| :--- | :--- | :--- | :--- |
| **CsPbI3** | Perovskite | 🟡 SCF Converged | Ground-state energy mapping for solar cell stability. |
| **Si** | Diamond Cubic | 🟢 Completed | Benchmark run; verified indirect band gap. |
| **[Next Material]** | [Class] | 🔴 Planned | Investigating optical absorption spectrum. |

*Status Legend: 🔴 Planned | 🟡 In Progress | 🟢 Completed*

---

## 📂 Quick Navigation
* `/shared_pseudos/` - Centralized repository for atomic pseudopotentials used across runs.
* `/materials/` - Contains material-specific input files (`.in`), output logs (`.out`), and localized analysis.

---

## 🚀 Useful Script Commands
To quickly extract convergence data from any Quantum ESPRESSO output file in this repo:
```bash
grep -e "Total energy" -e "iteration" material_scf.out
