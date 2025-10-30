# 🏬 WOMart Sales Prediction

### 📌 Introduction
Analisis ini menggunakan dataset WOMart yang berisi **18 bulan data penjualan dari 365 toko**. Tujuan utamanya adalah memahami faktor-faktor yang memengaruhi *Sales* dan membangun model prediksi.

### 📊 Dataset
Sumber: [Kaggle - WOMart Superstore Dataset](https://www.kaggle.com/datasets/roopacalistus/superstore)  
Jumlah data: **188,340 baris × 9 kolom**

Fitur utama:
- `Store_ID`, `Store_Type`, `Location_Type`, `Region_Code`, `Date`, `Holiday`, `Discount`, `#Order`, `Sales`  
Tidak ada missing atau duplicate value.

### 🔍 Data Preparation
- Ubah tipe data: `Store_ID`, `Holiday` → object; `Date` → datetime  
- Analisis korelasi menunjukkan **Sales dan Order** memiliki korelasi positif kuat.

### 📈 Exploratory Analysis
- **Holiday:** Sales lebih rendah saat hari libur.  
- **Discount:** Sales cenderung lebih rendah saat diskon.  
- **Region:** Tidak ada perbedaan signifikan antar wilayah.  

### 🧪 Statistical Testing
1. **Holiday vs Non-Holiday:** Sales berbeda signifikan (95% CI: 8195–8695)
2. **Discount vs Non-Discount:** Sales berbeda signifikan (95% CI: -12184 – -11861)

### 🤖 Regression Modelling
- **Simple Linear Regression:**  
  `Sales = 3879.28 + 570.41 * Order`
  → Korelasi kuat, R² ≈ 0.89
- **Multiple Linear Regression (Order, Holiday, Discount):**
  - Holiday → menurunkan Sales sebesar **1577.28**
  - Discount → meningkatkan Sales sebesar **4148.37**
  - Order → peningkatan 1 unit Order menambah Sales sebesar **552.15**

### 💡 Conclusion
Model mampu menjelaskan sekitar **89.89% variasi Sales**.  
Faktor yang berpengaruh signifikan terhadap Sales adalah:
- Order Volume  
- Diskon  
- Hari Libur

## 🔍 Full Report
For a complete analysis, detailed explanations, and visualizations, you can check the full article on Medium:
[Read it here →](https://medium.com/@zalfarmdhni/statistics-for-business-womart-sales-prediction-b3a7aca1a248)

