# 🏠 Prediksi Harga Rumah Menggunakan Machine Learning

## 📖 Deskripsi Proyek

Proyek ini bertujuan untuk memprediksi harga rumah berdasarkan karakteristik properti menggunakan algoritma Machine Learning.

Dataset yang digunakan berasal dari kompetisi Kaggle **House Prices: Advanced Regression Techniques** yang berisi 1.460 data rumah dengan 79 fitur yang menggambarkan kondisi, ukuran, kualitas bangunan, dan fasilitas rumah.

Melalui proyek ini, saya melakukan proses end-to-end mulai dari eksplorasi data, pembersihan data, feature engineering, pemodelan, hingga evaluasi model.

---

## 🎯 Tujuan Bisnis

Penentuan harga rumah sering kali bergantung pada pengalaman dan penilaian subjektif.

Dengan memanfaatkan Machine Learning, proses valuasi dapat dilakukan secara lebih cepat, objektif, dan berbasis data.

Potensi penggunaannya antara lain:

- Agen properti
- Pengembang perumahan
- Investor properti
- Perbankan dan lembaga pembiayaan

---

## 📊 Dataset

**Sumber Dataset:**

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques

**Karakteristik Dataset:**

| Informasi | Nilai |
|------------|---------|
| Jumlah Data | 1.460 |
| Jumlah Fitur | 79 |
| Target | SalePrice |

Contoh fitur yang digunakan:

- OverallQual
- GrLivArea
- GarageCars
- TotalBsmtSF
- YearBuilt

---

## 🔍 Exploratory Data Analysis (EDA)

Beberapa temuan utama:

### Distribusi Harga Rumah

Sebagian besar rumah berada pada rentang harga menengah dengan beberapa outlier berharga sangat tinggi.

### Faktor yang Berkorelasi Tinggi dengan Harga Rumah

- OverallQual
- GrLivArea
- GarageCars
- GarageArea
- TotalBsmtSF

Temuan ini menunjukkan bahwa kualitas bangunan dan luas area rumah memiliki pengaruh besar terhadap harga jual.

---

## ⚙️ Data Preparation

Tahapan yang dilakukan:

- Menangani missing values
- Encoding fitur kategorikal
- Scaling fitur numerik
- Train-test split
- Pembuatan pipeline machine learning

---

## 🤖 Model yang Digunakan

Beberapa model yang dibandingkan:

1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor

---

## 🏆 Hasil Model

Model terbaik yang diperoleh adalah **Gradient Boosting Regressor**.

### Hyperparameter Terbaik

```python
n_estimators = 162
learning_rate = 0.057
max_depth = 5
min_samples_leaf = 3
subsample = 0.958
max_features = "sqrt"
```

### Performa Model

| Metrik | Nilai |
|---------|---------|
| Cross Validation R² | 0.8828 |
| Kaggle Score | 0.13514 |

---

## 📈 Insight Bisnis

### 1. Kualitas Bangunan Sangat Berpengaruh

Rumah dengan kualitas konstruksi yang lebih baik cenderung memiliki harga jual yang jauh lebih tinggi.

### 2. Luas Area Hunian Menjadi Faktor Penting

Semakin besar area tempat tinggal, semakin tinggi nilai properti.

### 3. Garasi dan Basement Menambah Nilai Properti

Fasilitas tambahan seperti garasi dan basement memiliki kontribusi yang signifikan terhadap harga rumah.

### 4. Data Membantu Mengurangi Subjektivitas

Pendekatan berbasis data dapat membantu proses penilaian harga rumah menjadi lebih objektif dan konsisten.

---

## 🛠️ Teknologi yang Digunakan

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn

---

## 📂 Struktur Repository

```
house-price-prediction/
│
├── data/
├── notebook/
├── images/
├── submission/
├── requirements.txt
└── README.md
```

---

## 🚀 Kesimpulan

Model Gradient Boosting berhasil menjelaskan sekitar **88% variasi harga rumah** berdasarkan karakteristik properti yang tersedia.

Hasil ini menunjukkan bahwa Machine Learning dapat digunakan sebagai alat bantu dalam proses valuasi properti yang lebih cepat, konsisten, dan berbasis data.

---

## 👤 Author

**Rochyati**

GitHub: https://github.com/r0chaya

LinkedIn: https://linkedin.com/in/rochyati
