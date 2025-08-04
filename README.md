# Distance-Analysis-in-new-DImension
# Distance Analysis in High Dimensions

This repository contains the solution for an assignment exploring how distances behave as dimensionality increases in a unit cube. We compare L1 and squared L2 distances for random point samples in dimensions from 1 to 1024.

## 📌 Problem Statement

For each dimension `d ∈ {2⁰, 2¹, ..., 2¹⁰}`, sample 100 random points from the unit cube `[0, 1]^d`, then:

1. Compute the **average** and **standard deviation** of all pairwise distances:
   - Squared Euclidean (L2): \\( \|x - y\|_2^2 = \sum_j (x_j - y_j)^2 \\)
   - Manhattan (L1): \\( \|x - y\|_1 = \sum_j |x_j - y_j| \\)

2. Plot:
   - Average distance vs. dimension
   - Standard deviation vs. dimension

## 📈 Visualizations

Plots for both L1 and squared L2 distances can be found in the [plots/](plots/) folder.

<p float="left">
  <img src="plots/avg_std_l2.png" width="400" />
  <img src="plots/avg_std_l1.png" width="400" />
</p>

## 📒 Writeup

Please refer to `Lab1_writeup.pdf` for a detailed report including:
- Problem summary
- Mathematical background
- Plots
- Observations

## 💻 Tools Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

## 📂 Folder Description

- `lab1.ipynb`: Source code with comments
- `plots/`: Output visualizations
- `data/`: (Optional) Serialized data for reuse
- `Lab1_writeup.pdf`: Submission-ready report

---

## 🧠 Observations (to be included in writeup)

- As dimension increases, the average distance increases.
- The standard deviation shrinks, i.e., pairwise distances concentrate around the mean (concentration of measure).
- This phenomenon illustrates why distance-based methods (like k-NN) become less effective in high dimensions.

---

## 🛡️ Note

This code is part of a class assignment. **Do not share it or use it for unauthorized purposes.**
