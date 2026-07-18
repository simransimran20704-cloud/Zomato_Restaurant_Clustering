# Zomato_Restaurant_Clustering

ZOMATO RESTAURANT CLUSTERING & SENTIMENT ANALYSIS
===================================================

PROJECT OVERVIEW
-----------------
This project analyzes Zomato restaurant data to understand customer
sentiment from reviews and to segment restaurants into meaningful
clusters using unsupervised machine learning. The goal is to help
customers find the best restaurants in their locality and help the
company identify areas where restaurants are lagging.

DATASET
-------
1. Zomato Restaurant names and Metadata.csv
   - Name        : Name of the restaurant
   - Links       : URL link of the restaurant
   - Cost        : Estimated per-person dining cost
   - Collections : Zomato category tags
   - Cuisines    : Cuisines served by the restaurant
   - Timings     : Restaurant operating hours

2. Zomato Restaurant reviews.csv
   - Restaurant : Name of the restaurant
   - Reviewer   : Name of the reviewer
   - Review     : Review text
   - Rating     : Rating given by the reviewer
   - Metadata   : Reviewer's total reviews and followers
   - Time       : Date and time of the review
   - Pictures   : Number of pictures posted with the review

PROJECT STRUCTURE
------------------
1. Zomato_EDA.ipynb
   - Data loading, cleaning, and exploratory data analysis
   - Missing value and duplicate handling
   - Visualizations: rating distribution, cost analysis,
     cuisine popularity, correlation analysis, etc.

2. Zomato_ML.ipynb
   - Sentiment analysis on review text (TextBlob polarity)
   - Restaurant-level feature engineering
   - Feature scaling and encoding (cuisines, cost, sentiment)
   - KMeans clustering with Elbow method and Silhouette score
   - PCA-based cluster visualization
   - Cluster profiling and business insights

TECH STACK
----------
- Python 3
- Pandas, NumPy       : Data manipulation
- Matplotlib, Seaborn : Visualization
- Scikit-learn        : Feature scaling, KMeans, PCA
- TextBlob            : Sentiment analysis

HOW TO RUN
----------
1. Install dependencies:
   pip install -r requirements.txt

2. Download TextBlob corpora (only needed once):
   python -m textblob.download_corpora

3. Place both CSV files in the same directory as the notebooks.

4. Run Zomato_EDA.ipynb first, then Zomato_ML.ipynb, in Jupyter Notebook
   or JupyterLab.

RESULTS
-------
- Restaurants segmented into distinct clusters based on cost, rating,
  sentiment, and cuisine variety.
- Insights on which restaurant segments are performing well and which
  need improvement.
- Sentiment trends identified across customer reviews.

AUTHOR
------
[Simran]
