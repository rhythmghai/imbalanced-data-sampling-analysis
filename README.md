# 📊 Sampling Techniques on Imbalanced Credit Card Dataset

## 📌 Objective
The objective of this project is to analyze the importance of sampling techniques in handling highly imbalanced datasets and evaluate how different sampling strategies affect the performance of machine learning models.

Imbalanced datasets are common in real-world scenarios such as fraud detection, medical diagnosis, and anomaly detection. Proper balancing techniques help improve prediction performance and model reliability.

---

## 📂 Dataset
The dataset used is a **credit card transaction dataset** containing highly imbalanced classes.

- Majority class → Normal transactions  
- Minority class → Fraud transactions  

---

## ⚙️ Methodology

The following pipeline was implemented:

1. Load dataset  
2. Check class imbalance  
3. Apply different sampling techniques  
4. Train multiple ML models on each sampled dataset  
5. Compare performance using accuracy  

---

## 🔬 Sampling Techniques

| Sampling | Method |
|--------|--------|
| Sampling1 | Random Undersampling |
| Sampling2 | Random Oversampling |
| Sampling3 | SMOTE |
| Sampling4 | NearMiss |
| Sampling5 | SMOTEENN |

---

## 🤖 Machine Learning Models

| Model | Algorithm |
|------|-----------|
| M1 | Logistic Regression |
| M2 | Decision Tree |
| M3 | Random Forest |
| M4 | Linear SVM |
| M5 | K-Nearest Neighbors |

---

## 📈 Results

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|-----------|-----------|-----------|-----------|-----------|
| M1 | 66.67 | 91.92 | 91.70 | 16.67 | **95.11** |
| M2 | 66.67 | **99.13** | 97.60 | 16.67 | 98.85 |
| M3 | 83.33 | **99.56** | 99.13 | 16.67 | 99.14 |
| M4 | 50.00 | 91.48 | 92.79 | **100.00** | 95.40 |
| M5 | 16.67 | **98.47** | 82.97 | 83.33 | 94.83 |

---

## 🏆 Best Performing Models

| Model | Best Sampling | Accuracy |
|------|----------------|----------|
| M1 | Sampling5 | 95.11% |
| M2 | Sampling2 | 99.13% |
| M3 | Sampling2 | **99.56%** |
| M4 | Sampling4 | 100.00% |
| M5 | Sampling2 | 98.47% |

---

## 📊 Key Observations

- Oversampling methods performed significantly better than undersampling.
- Random Forest consistently achieved top accuracy scores.
- NearMiss sampling sometimes caused performance drops due to excessive data removal.
- Hybrid method (SMOTEENN) showed strong and stable results across models.

---

## ✅ Conclusion

Sampling techniques strongly influence machine learning performance on imbalanced datasets. Oversampling approaches such as **Random Oversampling** and **SMOTE** produced the best results, especially when paired with ensemble models like **Random Forest**.

Selecting the correct sampling strategy is crucial for building accurate and reliable classification systems when dealing with skewed class distributions.
