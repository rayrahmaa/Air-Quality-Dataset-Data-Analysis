# 🌍 Air Quality Data Analysis Dashboard

## 📌 Project Overview

Proyek ini merupakan dashboard interaktif berbasis **Streamlit** untuk menganalisis kualitas udara berdasarkan dataset Air Quality (2013–2017).

Dashboard ini memungkinkan pengguna untuk:
- Melihat rata-rata polutan per station dalam tahunan dan musiman
- Menganalisis hubungan variabel meteorologi terhadap PM2.5
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

## 📂 Project Structure

Air-Quality-Dataset-Data-Analysis/

│

├── dashboard/

│ ├── dashboard.py

│ └── main_data.parquet
│
├── data/

│ ├── PRSA_Data_Aotizhongxin_20130301-20170228.csv

│ ├── PRSA_Data_Changping_20130301-20170228.csv

│ ├── PRSA_Data_Dingling_20130301-20170228.csv

│ ├── PRSA_Data_Dongsi_20130301-20170228.csv

│ ├── PRSA_Data_Guanyuan_20130301-20170228.csv

│ ├── PRSA_Data_Gucheng_20130301-20170228.csv

│ ├── PRSA_Data_Huairou_20130301-20170228.csv

│ ├── PRSA_Data_Nongzhanguan_20130301-20170228.csv

│ ├── PRSA_Data_Shunyi_20130301-20170228.csv

│ ├── PRSA_Data_Tiantan_20130301-20170228.csv

│ ├── PRSA_Data_Wanliu_20130301-20170228.csv

│ └── PRSA_Data_Wanshouxigong_20130301-20170228.csv
│
├── README.md

├── notebook.ipynb

├── requirements.txt

└── url.txt

---

## ▶️ Cara Menjalankan Secara Lokal

1. Clone repository ini:
```
git clone https://github.com/rayrahmaa/Air-Quality-Dataset-Data-Analysis.git
```
3. Masuk ke folder project:
```
cd air-quality-dataset-data-analysis
```
3. Install dependencies:
```
pip install -r requirements.txt
```
4. Jalankan Streamlit:
```
streamlit run dashboard/dashboard.py
```

---

## 🌐 Live Demo

Aplikasi dapat diakses melalui:

https://air-quality-dataset-data-analysis-wafjt2vjtoozjappxhu8ebq.streamlit.app/

---

## 📈 Latar Belakang dan Pertanyaan Bisnis

Beijing dikenal sebagai salah satu kota dengan tingkat polusi udara tinggi di dunia, terutama pada awal dekade 2010-an. Fenomena smog yang parah menjadi perhatian global karena dampaknya terhadap kesehatan masyarakat dan aktivitas ekonomi. Sebagai respons terhadap kondisi tersebut, pemerintah Tiongkok mulai menerapkan berbagai kebijakan pengendalian emisi sejak tahun 2013 untuk menurunkan tingkat polusi udara, khususnya partikel halus PM2.5.

Evaluasi efektivitas kebijakan tersebut menjadi penting untuk mengetahui apakah terdapat perbaikan kualitas udara dalam beberapa tahun setelah implementasi kebijakan. Selain itu, faktor meteorologi seperti suhu, curah hujan, dan kecepatan angin juga diketahui memengaruhi konsentrasi polutan di atmosfer dan dapat memperburuk atau mengurangi kondisi smog.

Dengan menggunakan data kualitas udara dari 12 stasiun pemantauan di Beijing selama periode 2013 - 2017, analisis ini bertujuan untuk mengevaluasi tren polusi udara, mengidentifikasi pola musiman smog, serta memahami hubungan antara faktor cuaca dan konsentrasi polutan utama.

PERTANYAAN BISNIS :

1. Apakah terjadi penurunan konsentrasi PM2.5 di Beijing setelah penerapan kebijakan pengendalian emisi sejak 2013?

2. Kapan periode dengan tingkat smog tertinggi terjadi, dan apakah terdapat pola musiman yang konsisten?

3. Sejauh mana kondisi meteorologi berhubungan dengan tingkat konsentrasi PM2.5?

4. Apakah terdapat perbedaan tingkat polusi yang signifikan antar wilayah (station) di Beijing?

## 📈 Conclusion sebagai Insight Utama

Penarikan kesimpulan dengan melihat latar belakang bahwa Beijing dikenal sebagai salah satu kota dengan tingkat polusi udara tinggi, episode smog berat, dan implementasi kebijakan pengendalian emisi sejak 2013. Kebijakan tersebut bertujuan menurunkan konsentrasi partikulat halus (PM2.5) yang berdampak langsung pada kesehatan masyarakat.

Analisis ini menjawab empat pertanyaan utama terkait efektivitas kebijakan, pola musiman, pengaruh meteorologi, dan perbedaan spasial antar wilayah.

**Conclution pertanyaan 1 : Tren Tahunan**
Dari tren rata-rata tahunan yang diperoleh, ada penurunan bertahap hingga 2016 tetapi pada 2017 terjadi lonjakan signifikan. Artinya, kebijakan kemungkinan memberi dampak awal (2014–2016), tetapi efeknya tidak konsisten dalam jangka panjang.

**Conclution pertanyaan 2 : SMOG Tertinggi**
Dari analisis bulanan dan heatmap ditemui bahwa konsentrasi tertinggi PM2.5 terjadi pada Desember–Februari dan terendah pada Agustus. Selanjutnya, pola ini konsisten setiap tahun. Artinya, faktor pembakaran pemanas, stabilitas atmosfer, dan minimnya dispersi angin berperan besar.

**Conclution pertanyaan 3 : Hubungan Meteorologi dengan PM2.5**
Dari korelasi dan scatterplot diperoleh faktor paling berpengaruh yaitu kecepatan angin (WSPM). Artinya, kondisi atmosfer dan sirkulasi udara memiliki peran penting dalam pembentukan smog.

**Conclution pertanyaan 4 : Perbedaan Antar Wilayah (Spasial)**
Diperoleh dari visualisasi bahwa selisih antar station sekitar ±19 dengan wilayah pusat kota cenderung lebih tinggi dan wilayah pinggiran kota relatif lebih rendah. Artinya, masalah polusi bersifat kota-wide, bukan hanya lokal di satu wilayah.

**REKOMENDASI Berdasarkan EDA:**

1. Fokus pada Musim Dingin : Regulasi tambahan saat periode Des - Feb; Pembatasan industri sementara; Pengawasan emisi pemanas domestik

2. Kebijakan Adaptif Berbasis Cuaca dikarenalam WSPM berpengaruh besar: Menggunakan early warning system berbasis prediksi angin; menerapkan pembatasan lalu lintas saat angin rendah

3. Perlu Pendekatan Kota-Wide: kebijakan tidak cukup hanya lokal dan harus menyasar seluruh metropolitan

Monitoring Berkelanjutan karena lonjakan 2017 menunjukkan: evaluasi kebijakan harus periodik; masih perlu adaptasi strategi jangka panjang


---

## 👩‍💻 Author

Rahayu  
Project Data Analysis Submission  

