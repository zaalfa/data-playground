# 🩺 Health Case Bill Analysis

### 📌 Background
Asuransi kesehatan merupakan salah satu kebutuhan penting dalam perencanaan keuangan masa depan. Dalam sistem ini, pengguna membayar premi secara rutin kepada perusahaan asuransi, dan perusahaan akan menanggung biaya kesehatan pengguna. Penentuan nilai premi menjadi tantangan karena banyak faktor yang memengaruhi profil risiko pengguna.

### 📊 Dataset
Dataset yang digunakan dapat diakses di Kaggle.

### 📈 Descriptive Statistics
Beberapa temuan dari analisis deskriptif:

- Rata-rata umur pengguna: **39.2 tahun**
- Rata-rata BMI: **30.66**
- Rata-rata tagihan perokok jauh lebih tinggi dari non-perokok (**selisih ≈ 23,435.75**)
- Tidak ada missing atau duplicate data

### 🔍 Categorical Variable Analysis
Analisis distribusi dan peluang menunjukkan bahwa:
- Pengguna wanita memiliki rata-rata tagihan lebih tinggi daripada pria.
- Region *Southeast* memiliki jumlah pengguna terbanyak.
- Proporsi perokok sebesar **20.5%** dari seluruh pengguna.

### 📈 Continuous Variable Analysis
- Pengguna dengan **BMI > 25** lebih mungkin memiliki tagihan di atas 16.7k.
- Pengguna **perokok dengan BMI > 25** memiliki peluang **98%** memiliki tagihan di atas 16.7k.
- Korelasi positif antara **BMI dan tagihan kesehatan**, terutama untuk perokok.

### 🧪 Hypothesis Testing
1. **Tagihan perokok > non-perokok** → ✅ *H0 ditolak (p-value = 0.00)*
2. **Tagihan BMI > 25 > BMI < 25** → ✅ *H0 ditolak (p-value = 0.00)*
3. **Tagihan pria > wanita** → ✅ *H0 ditolak (p-value = 0.02)*

### 💡 Conclusion
Faktor yang memengaruhi besarnya tagihan kesehatan:
- **Umur**
- **BMI**
- **Jenis kelamin**
- **Kebiasaan merokok**

Semakin besar BMI dan usia, serta jika pengguna merokok, maka tagihan kesehatan cenderung meningkat.

## 🔍 Full Report
For a complete analysis, detailed explanations, and visualizations, you can check the full article on Medium:
[Read it here →](https://medium.com/@zalfarmdhni/faktor-yang-memengaruhi-besaran-tagihan-kesehatan-1d4c400518ab)
