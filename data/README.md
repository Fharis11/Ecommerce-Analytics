# Data

File CSV mentah **tidak disertakan** di repo ini (salah satunya berukuran ±59 MB, terlalu besar untuk disimpan di Git secara langsung dan lebih baik diunduh langsung dari sumber aslinya agar repo tetap ringan).

## Sumber Data

Dataset yang digunakan berasal dari **Brazilian E-Commerce Public Dataset by Olist** (Kaggle):
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## File yang dibutuhkan

Letakkan file berikut di dalam folder `data/` ini sebelum menjalankan notebook:

| Nama file di notebook | Deskripsi | Ukuran (approx.) |
|---|---|---|
| `dataset_ecomerce_analytics.csv` | Data gabungan order, customer, produk, pembayaran, dan review | ~20 MB |
| `olist_sellers_dataset.csv` | Data penjual (seller) beserta lokasi | ~170 KB |
| `olist_geolocation_dataset.csv` | Data koordinat lat/lng berdasarkan kode pos | ~59 MB |

## Cara mendapatkan data

1. Buat akun / login di [Kaggle](https://www.kaggle.com).
2. Download dataset dari link di atas (perlu Kaggle API atau download manual sebagai ZIP).
3. Ekstrak file CSV yang relevan ke dalam folder `data/`.
4. Sesuaikan nama file jika perlu, atau ubah path di sel pertama notebook (`pd.read_csv(...)`) agar sesuai dengan nama file hasil download.

> Catatan: `dataset_ecomerce_analytics.csv` merupakan hasil penggabungan (merge) beberapa tabel asli Olist (orders, order_items, order_payments, order_reviews, customers, products, product_category_name_translation). Jika Anda hanya mengunduh dataset mentah dari Kaggle, Anda perlu melakukan proses join/merge sendiri sebelum menjalankan notebook ini.
