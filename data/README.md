# Data

The raw CSV files are **not included** in this repository (one of them is ±59 MB, too large to store directly in Git — it's better to download it straight from the original source so the repo stays lightweight).

## Data Source

The dataset used comes from the **Brazilian E-Commerce Public Dataset by Olist** (Kaggle):
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## Required Files

Place the following files inside this `data/` folder before running the notebook:

| File name in the notebook | Description | Size (approx.) |
|---|---|---|
| `dataset_ecomerce_analytics.csv` | Merged data of orders, customers, products, payments, and reviews | ~20 MB |
| `olist_sellers_dataset.csv` | Seller data including location | ~170 KB |
| `olist_geolocation_dataset.csv` | Lat/lng coordinate data by zip code prefix | ~59 MB |

## How to Get the Data

1. Create an account / log in to [Kaggle](https://www.kaggle.com).
2. Download the dataset from the link above (requires the Kaggle API or a manual ZIP download).
3. Extract the relevant CSV files into the `data/` folder.
4. Rename the files if needed, or update the path in the notebook's first cell (`pd.read_csv(...)`) to match the downloaded file names.

> Note: `dataset_ecomerce_analytics.csv` is the result of merging several original Olist tables (orders, order_items, order_payments, order_reviews, customers, products, product_category_name_translation). If you only download the raw dataset from Kaggle, you'll need to perform the join/merge process yourself before running this notebook.
