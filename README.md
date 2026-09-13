# 📊 E-Commerce Analytics - Brazilian Olist Dataset

End-to-end data analysis on the Brazilian e-commerce dataset (Olist) to uncover business insights: revenue trends, the most profitable product categories, customer segmentation (RFM), logistics performance, customer satisfaction, and payment behavior.

## 🎯 Project Goals

This project aims to answer several key business questions:

- How has the company's monthly revenue trended over time?
- Which product categories are the most profitable?
- What's the geographic distribution of customers and sellers?
- Who are the most valuable customers (RFM segmentation: Recency, Frequency, Monetary)?
- Does delivery time affect customer review ratings?
- What payment method patterns do customers use?
- How much shipping cost are customers willing to tolerate relative to item price?

## 🗂️ Repository Structure

```
ecommerce-analytics/
├── notebooks/
│   └── ecommerce_analytics.ipynb   # Main analysis notebook
├── data/
│   └── README.md                   # Dataset info & download instructions (raw data not pushed)
├── requirements.txt                # Python dependencies
├── .gitignore
├── LICENSE
└── README.md
```

## 🧰 Tech Stack

- Python 3
- pandas & numpy - data manipulation and aggregation
- matplotlib & seaborn - data visualization
- Jupyter Notebook

## 📁 Dataset

Uses the **Brazilian E-Commerce Public Dataset by Olist** from Kaggle: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

The raw dataset is **not included** in this repo due to its size. See [`data/README.md`](data/README.md) for details on the required files and how to download them.

## 🔍 Analysis Workflow

1. **Import & Load Data** - load order, seller, and geolocation data
2. **Data Cleaning & Preprocessing** - datetime type conversion, missing value handling
3. **Revenue Over Time** - monthly revenue trend
4. **Top Profitable Product Categories** - top 10 product categories by revenue
5. **Geospatial Analysis** - customer & seller distribution by state
6. **Customer Segmentation (RFM Analysis)** - customer segmentation based on Recency, Frequency, Monetary
7. **Logistics Performance & Customer Satisfaction** - correlation between delivery time and review score
8. **Logistics Density Map** - geospatial mapping of location points across Brazil
9. **Financial & Payment Behavior** - payment method analysis
10. **Order Economics** - shipping cost to item price ratio

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/ecommerce-analytics.git
   cd ecommerce-analytics
   ```

2. (Optional but recommended) create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate        # Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Download the dataset following the instructions in [`data/README.md`](data/README.md) and place the CSV files in the `data/` folder.

5. Run the notebook:
   ```bash
   jupyter notebook notebooks/ecommerce_analytics.ipynb
   ```

## 📌 Notes

This notebook was built for data analytics exploration and learning purposes. Contributions, suggestions, and pull requests are very welcome.

## 📄 License

This project is licensed under [MIT](LICENSE).
