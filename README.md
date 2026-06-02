# CustomerReviewTopicModeling
Testing out Claude Code for personal learning by applying an NLP TF-IDF and K-Means algorithm to group similar reviews together.

# Dataset Source
Dataset from Kaggle here: [E-Commerce Purchases & Reviews](https://www.kaggle.com/datasets/pruthvirajgshitole/e-commerce-purchases-and-reviews)

Place the downloaded CSVs in `data/raw/` before running the notebooks.

# Get Started

**1. Install dependencies**
```bash
pip install -r requirements.txt
```

**2. Run the data pipeline**

Open and run `notebooks/01_data_pipeline.ipynb`. This cleans the raw review text and saves a compressed dataset to `data/processed/reviews.npz`.

**3. Run topic modeling**

Open and run `notebooks/02_topic_modeling.ipynb`. Inspect the elbow plot to choose K, set it in cell 4, then run the rest to see cluster topics, a PCA scatter plot, and sample reviews per cluster.