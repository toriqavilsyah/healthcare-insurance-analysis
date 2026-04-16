# 🏥 Healthcare Insurance Analysis

## 📌 Deskripsi Proyek
Biaya kesehatan global terus meningkat, dengan total pengeluaran mencapai USD 9.8 triliun. Dalam industri asuransi, penentuan premi yang akurat menjadi sangat penting karena dipengaruhi oleh berbagai faktor individu seperti usia, BMI, dan gaya hidup.

Proyek ini bertujuan untuk menganalisis faktor-faktor utama yang memengaruhi biaya asuransi kesehatan (insurance charges) sehingga perusahaan dapat mengoptimalkan strategi pricing dan risk assessment berbasis data.

---

## 🎯 Tujuan Analisis
- Menganalisis pengaruh usia (age) terhadap biaya asuransi  
- Menganalisis pengaruh BMI terhadap biaya asuransi  
- Mengevaluasi dampak status merokok terhadap biaya  
- Membandingkan biaya berdasarkan jenis kelamin  
- Mengidentifikasi faktor paling signifikan dalam menentukan biaya asuransi  

---

## 📂 Dataset
- Sumber: Kaggle (Health Insurance Charges Dataset)  
- Jumlah data: 1338 baris, 7 kolom  

**Fitur utama:**
- Age  
- Sex  
- BMI  
- Children  
- Smoker  
- Region  
- Charges  

---

## ⚙️ Proses Analisis

### 1. Data Cleaning
- Tidak terdapat missing value  
- Menghapus 1 data duplikat  

### 2. Handling Outlier
- Outlier ditemukan pada variabel Charges (139 data) dan BMI (9 data)  
- Outlier tetap dipertahankan karena mencerminkan kondisi nyata  

### 3. Feature Engineering
- Membuat:
  - Age Group  
  - BMI Category  
- Digunakan untuk analisis segmentasi  

### 4. Exploratory Data Analysis (EDA)
- Analisis distribusi  
- Analisis hubungan antar variabel  
- Visualisasi pola biaya asuransi  

---

## 📊 Key Insights

### 1. Usia berpengaruh signifikan terhadap biaya asuransi
- Biaya meningkat seiring bertambahnya usia  
- Usia 50+ memiliki biaya tertinggi (~$17.9K)  
- Usia <20 memiliki biaya terendah (~$8.5K)  

### 2. BMI memiliki pengaruh terhadap biaya
- BMI tinggi → biaya lebih tinggi  
- Obese: ~$15.57K (tertinggi)  
- Underweight: ~$8.85K (terendah)  
- Namun pengaruhnya tidak sekuat usia  

### 3. Status merokok adalah faktor paling dominan
- Perokok memiliki biaya jauh lebih tinggi  
- Obese + smoker: ~$50.4K vs non-smoker ~$8.9K  
- Efek konsisten di semua kelompok usia  

### 4. Gender tidak berpengaruh signifikan
- Perbedaan biaya laki-laki vs perempuan relatif kecil (~$1.4K)  
- Bukan faktor utama dalam penentuan harga  

---

## 💡 Business Recommendations

### 1. Terapkan age-based pricing
- Gunakan usia sebagai faktor utama dalam penentuan premi  
- Segmentasi pelanggan berdasarkan kelompok umur  

### 2. Pertimbangkan BMI dalam risk assessment
- Integrasikan BMI dalam model pricing  
- Dorong program kesehatan preventif (wellness program)  

### 3. Terapkan risk-based pricing untuk perokok
- Perokok → risiko tinggi → premi lebih tinggi  
- Implementasi program berhenti merokok untuk menekan biaya  

### 4. Fokus pada faktor berbasis risiko, bukan gender
- Hindari penggunaan gender sebagai faktor utama  
- Prioritaskan variabel yang lebih relevan (age, BMI, smoker)  

---

## 🛠 Tools yang Digunakan
- Python (Pandas, Matplotlib, Seaborn)  
- Power BI  
- Microsoft Excel  

---

## 📊 Dashboard
Dashboard digunakan untuk:
- Analisis biaya berdasarkan usia & BMI  
- Perbandingan biaya berdasarkan status merokok  
- Segmentasi pelanggan  
- Monitoring KPI utama  

---

## 📌 Kesimpulan
Analisis menunjukkan bahwa usia dan status merokok merupakan faktor paling signifikan dalam menentukan biaya asuransi kesehatan, diikuti oleh BMI. Sementara itu, gender tidak memiliki pengaruh yang berarti.

Insight ini dapat digunakan untuk meningkatkan akurasi pricing, optimalisasi risk assessment, serta menciptakan strategi bisnis yang lebih adil dan menguntungkan.
