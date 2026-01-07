<div align="center">

<!-- ===== Banner (Title + Tech Stack) ===== -->
<h1>MNIST Lab — Baseline Classification with Mean Images</h1>

<p>
  <img alt="Python" src="https://img.shields.io/badge/Python-3.14-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img alt="NumPy" src="https://img.shields.io/badge/NumPy-Array%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-Plotting-11557C?style=for-the-badge&logo=plotly&logoColor=white" />
  <img alt="Seaborn" src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=for-the-badge&logo=python&logoColor=white" />
  <img alt="scikit-learn" src="https://img.shields.io/badge/scikit--learn-Metrics%20%26%20Tools-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
</p>

<p><b>Course / Lab:</b> Computer Vision Lab - Assignment 3 — MNIST • <b>Topic:</b> Distance-based baseline (MAE vs MSE) + Accuracy + Confusion Matrix</p>

</div>

---

## Overview
This repository contains my work for **Assignment 3 (MNIST)**.  
The notebook loads MNIST from IDX files, explores the dataset, visualizes examples, and implements a **simple distance-based classifier** using **class mean images**. Two distance measures are compared:
- **MAE (Mean Absolute Error)**
- **MSE (Mean Squared Error)**

The project concludes with **accuracy evaluation** and a **(normalized) confusion matrix**.

---

## Key Concepts
- MNIST data parsing (IDX format)
- Dataset exploration and visualization
- Mean image and pixel-wise standard deviation
- Baseline classification via distance to class prototypes
- Model evaluation:
  - Accuracy
  - Confusion matrix (counts + normalized 0–1)

---

## Dataset
**MNIST (Handwritten Digits)**  
- Image size: **28×28**
- Training samples: **60,000**
- Test samples: **10,000**

---

## What’s Implemented (Q1–Q9)
- **Q1:** Dataset info (dimensions + number of images)
- **Q2:** Load training/testing sets and verify shapes
- **Q3:** Visualize digits (0–9) in a 2×5 grid
- **Q4:** Function to extract images of a digit + count per digit
- **Q5:** Montages for selected digits (e.g., 1, 3, 7)
- **Q6:** Mean image and std image for a chosen digit (e.g., 5)
- **Q7:** Prediction using MAE and MSE to class mean images
- **Q8:** Compute test accuracy for MAE vs MSE classifiers
- **Q9:** Confusion matrix (including normalized version 0.0–1.0)

---

## Project Structure
```text
.
├── Assignment_3.ipynb
├── data/
│   ├── train-images-idx3-ubyte.gz
│   ├── train-labels-idx1-ubyte.gz
│   ├── t10k-images-idx3-ubyte.gz
│   └── t10k-labels-idx1-ubyte.gz
└── README.md
```
---
## Notes on Reproducibility

- Results may vary slightly if any randomized operations are used.
- For cross-validation workflows, random_state is used to keep splits reproducible.
---
## Results (Fill In After Running)

**MAE Accuracy:** __
**MSE Accuracy:** __
**Most common confusions:** __ (e.g., 4↔9, 3↔5)
---
## License
This project is intended for educational use.
---
