# 💰 ForeMas - Forecast Harga Emas Berbasis Machine Learning

**ForeMas** adalah aplikasi web interaktif untuk memprediksi harga emas berdasarkan data historis menggunakan model **LSTM (Long Short-Term Memory)**. Aplikasi ini bertujuan membantu pengguna membuat keputusan investasi lebih cerdas dengan memanfaatkan teknologi **Machine Learning** dan **visualisasi data**.

![Banner](./public/chart.png)

---

## 🌟 Fitur Utama

🔍 **Prediksi Harga Emas Akurat**  
Model LSTM dilatih menggunakan data harian dari 2015–2021 untuk memprediksi harga emas di masa depan.

📆 **Timeframe Prediksi Fleksibel**  
Pilih jangka waktu prediksi:  
- 1 Minggu  
- 1 Bulan  
- 3 Bulan  
- 6 Bulan  
- 1 Tahun

📈 **Visualisasi Interaktif**  
Grafik harga aktual dan prediksi ditampilkan secara elegan dan mudah dipahami.

💡 **Saran Investasi Otomatis**  
ForeMas memberikan rekomendasi investasi berdasarkan tren harga emas hasil prediksi.

📨 **Form Kontak**  
Fitur untuk mengirim feedback atau pertanyaan langsung ke tim pengembang.

---

## 📊 Sumber Data

Dataset yang digunakan diperoleh dari Kaggle:

📎 **Daily Gold Price (2015–2025) Time Series**  
📍 Link: [https://www.kaggle.com/datasets/nisargchodavadiya/daily-gold-price-20152021-time-series](https://www.kaggle.com/datasets/nisargchodavadiya/daily-gold-price-20152021-time-series)  
Dataset ini mencakup harga emas harian selama 6 tahun dalam berbagai satuan ukuran (Gram, Ounce, dll).

---

## 🧠 Teknologi & Arsitektur

### 🖥️ Frontend
- HTML, CSS, JavaScript
- Webpack untuk bundling
- Hosting: [Vercel](https://vercel.com)

### 🔙 Backend
- Node.js + Express
- API untuk prediksi (`/api/predict.js`) dan form kontak (`/api/contact.js`)
- Hosting: [Railway](https://railway.app)

### 🤖 Machine Learning
- Model LSTM dibuat dengan TensorFlow/Keras
- Format model: `.h5`
- Implementasi & training model dilakukan dalam Google Colab (`.ipynb`)

### 🗂️ Arsitektur Proyek

```bash
foremas/
├── api/                  # API endpoints (predict & contact)
├── dist/                 # Bundle hasil build
├── public/               # Static assets
├── src/                  # Source code utama frontend
├── ss/                   # Screenshot aplikasi
├── *.ipynb               # Notebook ML training & evaluasi
├── webpack.config.js     # Webpack configuration
├── package.json          # Dependency & script
└── vercel.json           # Config deployment ke Vercel
