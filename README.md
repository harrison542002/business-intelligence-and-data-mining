
# 📘 README – BI Group Work Notebook

## 📌 Overview
This Jupyter Notebook is part of a group project focusing on building a **hybrid recommendation system** and performing **data analysis** on the Olist e-commerce dataset. Key components include:
- Exploratory Data Analysis (EDA)
- Customer segmentation using KMeans
- Sentiment analysis with VADER and Hugging Face Transformers
- Recommender systems using LightFM and Surprise (SVD)

## ⚙️ Requirements
Make sure to install the required libraries before running the notebook:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightfm surprise nltk transformers wordcloud
```

You may also need to download NLTK resources:
```python
import nltk
nltk.download('vader_lexicon')
```

## 📂 Data
- The notebook expects **Olist dataset CSV files** (e.g., `orders.csv`, `products.csv`, etc.).
- These files are loaded using a relative file path variable defined as:

```python
relative_file_path = "/content/drive/MyDrive/olist_data"
```

- 📌 **Important:** If your data is stored in a different location, **please update the `relative_file_path` variable accordingly** to point to your dataset folder.

## 🚨 Important Notes
- Some models (e.g., Hugging Face transformers) may require internet access and may take time to load.
- Running LightFM and SVD models can be computationally intensive. Consider using a machine with sufficient memory and CPU.
- Watch for **data preprocessing cells**—ensure they complete successfully before moving forward.

## ✅ Output
The notebook produces:
- Visualizations (customer behavior, clusters, sentiment)
- Word clouds
- Recommendation performance metrics (e.g., AUC, Precision@K)
