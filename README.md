# 📌 Customer E-Loyalty Clustering Analysis

## 📖 Deskripsi
Proyek ini bertujuan untuk menganalisis **customer e-loyalty** menggunakan metode **Clustering (K-Means)**.  
Langkah-langkah yang dilakukan meliputi:
1. Import & eksplorasi data
2. Uji reliabilitas & validitas instrumen (Cronbach’s Alpha, EFA)
3. Preprocessing (handling missing values & scaling)
4. Dimensionality reduction (PCA)
5. Clustering (K-Means)
6. Evaluasi hasil clustering (Silhouette Score, Davies-Bouldin Index)
7. Profiling & interpretasi cluster
8. Kesimpulan & rekomendasi

---

## 📂 Struktur Project
```
.
├── customer_eloyalty.xlsx   # Dataset utama
├── analysis.ipynb           # Notebook utama (Google Colab / Jupyter)
├── requirements.txt         # List dependencies
└── README.md                # Dokumentasi project
```

---

## ⚙️ Instalasi
Clone repositori ini:
```bash
git clone https://github.com/username/customer-eloyalty.git
cd customer-eloyalty
```

Install dependencies:
```bash
pip install -r requirements.txt
```

---

## 📊 Tahapan Analisis
### 1. Import & Load Data
- Data diambil dari file Excel (`customer_eloyalty.xlsx`).  
- Cek struktur data, statistik deskriptif, dan informasi dataset.

### 2. Reliabilitas & Validitas
- **Cronbach’s Alpha** → mengukur konsistensi internal instrumen.  
- **EFA (Exploratory Factor Analysis)** → mengecek validitas konstruk.

### 3. Preprocessing
- Menghapus kolom ID (`Nomor`).  
- Mengecek missing values.  
- **StandardScaler** untuk standarisasi data.

### 4. PCA (Principal Component Analysis)
- Reduksi dimensi untuk memudahkan visualisasi & clustering.  
- Menentukan komponen utama yang paling signifikan.

### 5. Clustering
- Metode: **K-Means**.  
- Menentukan jumlah cluster optimal dengan **Elbow Method & Silhouette Score**.  
- Visualisasi hasil cluster dalam 2D (PCA).

### 6. Evaluasi Cluster
- **Silhouette Score**: 0.14 (cukup rendah → cluster agak tumpang tindih).  
- **Davies-Bouldin Index**: 2.061 (lebih kecil lebih baik, berarti masih bisa dioptimalkan).  

### 7. Profiling Cluster
- Setiap cluster dianalisis berdasarkan skor rata-rata tiap dimensi.  
- Visualisasi dengan heatmap.

### 8. Interpretasi & Rekomendasi
- Cluster 0 → **Customer rata-rata (netral)**  
- Cluster 1 → **Customer kurang loyal (skor rendah di banyak dimensi)**  
- Cluster 2 → **Customer sangat loyal (skor tinggi konsisten)**  

---

## 📌 Hasil Utama
- Data terbagi menjadi **3 cluster utama**.  
- Profil cluster membantu strategi pemasaran & retensi customer.  
- Potensi optimasi lebih lanjut dengan metode clustering lain (DBSCAN, Hierarchical, GMM).

---

## 🚀 Next Steps
- Coba algoritma clustering lain untuk validasi hasil.  
- Tambahkan visualisasi interaktif (Plotly, Dash).  
- Lakukan uji hipotesis antar cluster.

---

## 👨‍💻 Author
Dikerjakan oleh **[Nama Kamu]**  
Proyek analisis ini dibuat menggunakan **Python (pandas, scikit-learn, seaborn, matplotlib, factor_analyzer)**.  
