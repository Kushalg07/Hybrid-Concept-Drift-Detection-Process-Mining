# 🔍 Hybrid Concept Drift Detection in Process Mining
### A Control Flow Perspective (IEEE Research Project)

📄 Published Research Implementation based on IEEE Conference Paper

---

## 📌 Project Overview

This project presents a **Hybrid Framework for Detecting and Localizing Incremental Concept Drift** in Process Mining using a Control Flow perspective.

The approach integrates:

- Statistical drift detection (CUSUM)
- Machine learning methods (K-Means, Random Forest, Bagging)
- Dimensionality Reduction (SVD)
- Process Mining techniques (Alpha Miner, Heuristics Miner)
- Model comparison (Pre-drift vs Post-drift)

The system is validated using the **BPI Challenge 2016 dataset**.

---

## 🎯 Problem Statement

Business processes evolve over time.  
Incremental concept drift causes gradual changes in process behavior, making detection challenging.

Traditional methods focus mainly on sudden drift.

This project proposes a **hybrid, multi-method detection and localization framework** to detect gradual changes and identify affected process regions.

---

## 🧠 Proposed Hybrid Architecture

1. Data Preprocessing
2. Time-window segmentation (Monthly)
3. CUSUM drift detection
4. K-Means clustering analysis
5. Ensemble Model (Random Forest + Bagging)
6. SVD dimensionality reduction
7. Process discovery using Alpha Miner
8. Pre-drift vs Post-drift model comparison
9. ROC-AUC performance evaluation

---

## 📊 Key Results

| Method | AUC Score |
|--------|------------|
| CUSUM | **1.00** |
| Ensemble (RF + Bagging + SVD) | 0.80 |
| K-Means | 0.59 |
| Alpha Miner Proxy | 0.55 |

### 🔹 Major Drift Detected:
October 2015

### 🔹 Process Model Fitness Degradation:
- Pre-drift log fitness: 0.341
- Post-drift log fitness: 0.266

---

## 📈 Techniques Used

### 🔹 Statistical Method
- Cumulative Sum (CUSUM)

### 🔹 Machine Learning
- K-Means Clustering
- Random Forest
- Bagging Classifier
- SVD

### 🔹 Process Mining
- Directly-Follows Graph (DFG)
- Alpha Miner (Petri Nets)
- Heuristics Miner
- Replay Fitness Analysis

---

## 🛠 Tech Stack

- Python
- Pandas
- Scikit-learn
- PM4Py
- NetworkX
- Matplotlib / Seaborn

---

## 📂 Dataset

- BPI Challenge 2016 (Complaint Management Process)
- Event log-based dataset
- Monthly segmentation for incremental drift detection

---

## 🔬 Research Contribution

- Hybrid detection combining statistical + ML + process mining
- Effective localization of incremental drift
- Demonstrated superiority of CUSUM for gradual drift
- Comparative ROC-AUC analysis of multiple techniques
