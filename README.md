# House-Price-Prediction---Indonesia-AI
Prediksi harga rumah menggunakan Linear Regression, Random Forest, dan XGBoost  berbasis Ames Housing Dataset — mencakup feature engineering, encoding, dan hyperparameter tuning.

## 📌 Deskripsi

Proyek ini mengembangkan sistem prediksi harga rumah berbasis machine learning menggunakan Ames Housing Dataset yang memiliki 79 fitur deskriptif. Fokus utama proyek adalah membangun pipeline ML yang lengkap, mulai dari eksplorasi data (EDA), rekayasa fitur, preprocessing, encoding, hingga pelatihan dan optimasi model menggunakan **Linear Regression**, **Random Forest**, dan **XGBoost**.

## 🎯 Tujuan Proyek

Membangun dan membandingkan performa beberapa model regresi untuk memprediksi harga jual properti residensial secara akurat, sekaligus menerapkan praktik terbaik dalam preprocessing dan seleksi fitur.

## 🔧 Tahapan Utama

- 📊 **EDA** — analisis distribusi, korelasi fitur, dan deteksi outlier (IQR & Z-score)
- 🛠️ **Feature Engineering** — fitur komposit (GarageScore), fitur usia (HouseAge, RemodelAge), dan interaction terms
- 🔄 **Preprocessing** — imputasi missing value, penghapusan fitur near-zero variance, dan scaling
- 🏷️ **Encoding** — ordinal encoding, target encoding (Neighborhood), dan label encoding
- 🤖 **Modeling** — Linear Regression sebagai baseline, Random Forest, dan XGBoost
- ⚙️ **Hyperparameter Tuning** — optimasi xgboost

## 📄 Dataset

- 1460 data 
- 79 Feature
- 1 Feature Target Sale Price

## 📊 Model Performance

| No | Model | MAPE Test (%) | R² Test (%) |
|----|--------|--------------:|------------:|
| 1 | Linear Regression | 12.23 | 85.15 |
| 2 | Random Forest | 10.70 | 88.81 |
| 3 | XGBoost (Untuned) | 10.84 | 89.73 |
| 4 | **🔥 XGBoost (Tuned)** | **9.83** | **90.25** |

### 🏆 Best Model: XGBoost (Tuned)

### 🔍 Insight
- 🔥 XGBoost yang sudah di hyperparamater tuning memberikan performa terbaik dengan MAPE tertinggi
- Random forest terbukti lebih efektif dibandingkan model linear
- Linear Regression kurang optimal dibanding dengan XGboost dan random forest

## 🛠 Library yang Digunakan

`pandas` `numpy` `scikit-learn` `xgboost` seaborn` `matplotlib`

## 🚀 Cara Menjalankan
- Upload dataset ke environment (Google Colab / lokal)
- Pastikan path dataset sesuai:

