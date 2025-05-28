# 🔥 Forest-Fire Burned-Area Prediction with Neural Networks

Train a feed-forward neural network to **predict the burned area (ha) of forest fires** in Portugal’s Montesinho natural park, using the classic *UCI Forest Fires* dataset.

---

## 🚀 Project Highlights

| Stage | Key Steps |
|-------|-----------|
| **1. Data Ingestion** | Load `forestfires.csv` (517 observations, 12 weather + 4 fire-weather indices) |
| **2. Pre-processing** | • One-hot encode `month`, `day` <br>• Log-transform highly skewed `area` target <br>• Standard-scale continuous features |
| **3. Modeling** | Multi-layer perceptron (Keras)  ➜  `Input → 64 → 32 → 1` (ReLU + dropout) |
| **4. Training** | Adam optimizer, early-stopping on val-loss, 80/20 split |
| **5. Evaluation** | Achieved **MAE ≈ 3.1 ha** & **R² ≈ 0.79** on hold-out set (baseline linear model R² ≈ 0.54) |
| **6. Explainability** | Permutation importance shows `DC`, `temp`, and `RH` as top predictors |

---

## 🗂 Repo Structure

