# 🌍 Air Quality Data Analysis Dashboard

## 📌 Project Overview

Proyek ini merupakan dashboard interaktif berbasis **Streamlit** untuk menganalisis kualitas udara berdasarkan dataset Air Quality (2013–2017).

Dashboard ini memungkinkan pengguna untuk:
- Melihat rata-rata polutan per station
- Menganalisis hubungan variabel lingkungan terhadap PM2.5
- Melakukan filtering data secara interaktif
- Mengeksplorasi tren kualitas udara

Project ini dibuat sebagai bagian dari submission analisis data.

---

## 📊 Dataset

Dataset yang digunakan berisi informasi kualitas udara dari berbagai station dengan variabel seperti:

- PM2.5
- PM10
- SO2
- NO2
- CO
- O3
- TEMP (Temperature)
- PRES (Pressure)
- DEWP (Dew Point)
- WSPM (Wind Speed)
- Station
- Tanggal

---

## 🚀 Fitur Dashboard

✔️ Filter berdasarkan station  
✔️ Menampilkan metrik rata-rata polutan  
✔️ Visualisasi bar chart rata-rata PM2.5  
✔️ Scatter plot hubungan variabel cuaca dengan PM2.5  
✔️ Tampilan responsif dan interaktif  

---

## 🛠️ Tech Stack

- Python
- Streamlit
- Pandas
- Matplotlib
- Seaborn

---

## 📂 Struktur Folder


Air-Quality-Dataset-Data-Analysis/
│
├── dashboard/
│ ├── dashboard.py
│ └── main_data.parquet
├── data/
│ ├── PRSA_Data_Aotizhongxin_20130301-20170228
│ ├── PRSA_Data_Changping_20130301-20170228
│ ├── PRSA_Data_Dingling_20130301-20170228
│ ├── PRSA_Data_Dongsi_20130301-20170228
│ ├── PRSA_Data_Guanyuan_20130301-20170228
│ ├── PRSA_Data_Gucheng_20130301-20170228
│ ├── PRSA_Data_Huairou_20130301-20170228
│ ├── PRSA_Data_Nongzhanguan_20130301-20170228
│ ├── PRSA_Data_Shunyi_20130301-20170228
│ ├── PRSA_Data_Tiantan_20130301-20170228
│ ├── PRSA_Data_Wanliu_20130301-20170228
│ └── PRSA_Data_Wanshouxigong_20130301-20170228
├── README.md
├── notebook.ipynb
├── requirements.txt
└── url.txt
---

## ▶️ Cara Menjalankan Secara Lokal

1. Clone repository ini:
2. 
git clone https://github.com/rayrahmaa/Air-Quality-Dataset-Data-Analysis.git

3. Masuk ke folder project:

cd air-quality-dataset-data-analysis

3. Install dependencies:

pip install -r requirements.txt

4. Jalankan Streamlit:

streamlit run dashboard/dashboard.py

---

## 🌐 Live Demo

Aplikasi dapat diakses melalui:

https://air-quality-dataset-data-analysis-wafjt2vjtoozjappxhu8ebq.streamlit.app/

---

## 📈 Insight Utama

- Beberapa station menunjukkan rata-rata PM2.5 yang tinggi secara konsisten.
- Variabel cuaca seperti suhu dan tekanan udara memiliki hubungan tertentu terhadap konsentrasi PM2.5.
- Perbedaan kualitas udara antar station cukup signifikan.

---

## 👩‍💻 Author

Rahayu  
Project Data Analysis Submission  

