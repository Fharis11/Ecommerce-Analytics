# 📊 E-Commerce Analytics - Brazilian Olist Dataset

Analisis data end-to-end terhadap dataset e-commerce Brazil (Olist) untuk menggali insight bisnis: tren pendapatan, kategori produk paling menguntungkan, segmentasi pelanggan (RFM), performa logistik, kepuasan pelanggan, dan perilaku pembayaran.

## 🎯 Tujuan Proyek

Proyek ini bertujuan menjawab beberapa pertanyaan bisnis utama:

- Bagaimana tren pendapatan bulanan perusahaan dari waktu ke waktu?
- Kategori produk apa yang paling menguntungkan?
- Bagaimana sebaran geografis pelanggan dan penjual?
- Siapa pelanggan paling bernilai (segmentasi RFM: Recency, Frequency, Monetary)?
- Apakah waktu pengiriman memengaruhi rating ulasan pelanggan?
- Bagaimana pola metode pembayaran yang digunakan pelanggan?
- Seberapa besar toleransi pelanggan terhadap ongkos kirim dibanding harga barang?

## 🗂️ Struktur Repository

```
ecommerce-analytics/
├── notebooks/
│   └── ecommerce_analytics.ipynb   # Notebook utama analisis
├── data/
│   └── README.md                   # Info & cara mendapatkan dataset (data mentah tidak di-push)
├── requirements.txt                # Dependensi Python
├── .gitignore
├── LICENSE
└── README.md
```

## 🧰 Tech Stack

- Python 3
- pandas & numpy - manipulasi dan agregasi data
- matplotlib & seaborn - visualisasi data
- Jupyter Notebook

## 📁 Dataset

Menggunakan **Brazilian E-Commerce Public Dataset by Olist** dari Kaggle: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Dataset mentah **tidak disertakan** di repo ini karena ukurannya cukup besar. Lihat [`data/README.md`](data/README.md) untuk detail file yang dibutuhkan dan cara mengunduhnya.

## 🔍 Alur Analisis

1. **Import & Load Data** - memuat data order, seller, dan geolocation
2. **Data Cleaning & Preprocessing** - konversi tipe datetime, penanganan missing value
3. **Revenue Over Time** - tren pendapatan bulanan
4. **Top Profitable Product Categories** - 10 kategori produk dengan pendapatan tertinggi
5. **Geospatial Analysis** - distribusi pelanggan & penjual per state
6. **Customer Segmentation (RFM Analysis)** - segmentasi pelanggan berdasarkan Recency, Frequency, Monetary
7. **Logistics Performance & Customer Satisfaction** - korelasi waktu pengiriman dengan review score
8. **Logistics Density Map** - pemetaan geospasial titik lokasi di peta Brazil
9. **Financial & Payment Behavior** - analisis metode pembayaran
10. **Order Economics** - rasio ongkos kirim terhadap harga barang

## 🚀 Cara Menjalankan

1. Clone repository ini:
   ```bash
   git clone https://github.com/<username-anda>/ecommerce-analytics.git
   cd ecommerce-analytics
   ```

2. (Opsional tapi disarankan) buat virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate        # Windows: venv\Scripts\activate
   ```

3. Install dependensi:
   ```bash
   pip install -r requirements.txt
   ```

4. Unduh dataset sesuai instruksi di [`data/README.md`](data/README.md) dan letakkan file CSV di folder `data/`.

5. Jalankan notebook:
   ```bash
   jupyter notebook notebooks/ecommerce_analytics.ipynb
   ```

## 📌 Catatan

Notebook ini dibuat untuk tujuan eksplorasi dan pembelajaran data analytics. Kontribusi, saran, atau pull request sangat terbuka.

## 📄 Lisensi

Proyek ini menggunakan lisensi [MIT](LICENSE).
