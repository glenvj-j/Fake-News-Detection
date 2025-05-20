# Fake News Detection with NLP & Machine Learning


![Cover](https://github.com/user-attachments/assets/0fa71977-91e6-4800-8c17-fa70a81b3b87)


> [!NOTE]
> **Created by:** [Glen Valencius](https://github.com/glenvj-j)  
**Dataset Source:** [Kaggle](https://www.kaggle.com/datasets/mahdimashayekhi/fake-news-detection-dataset/data) <p>
**Slides:** [Google Slides](https://docs.google.com/presentation/d/124N4-jHtYNBUpURUTWdVgKDqY9as_xAJQ7DdKLAEEw8/edit?slide=id.p#slide=id.p)



An educational project demonstrating how to build a pipeline for classifying news articles as real or fake using a synthetically generated dataset. The focus is on minimizing false negatives (fake news misclassified as real) through tailored feature engineering and model selection.

## ⚠️ Disclaimer
> This dataset has been synthetically generated to closely resemble real-world news content. While suitable for modeling and experimentation, the results should be validated on real data before any production deployment.


## 🚀 Key Highlights
- **Data:** Synthetic news corpus with `title`, `text`, `source`, `author`, `category`, and publication date.
- **Feature Engineering:**  
  - **Text Vectorization:** TF–IDF on titles and full articles  
  - **Categorical Encoding:** One-Hot for `source` & `category`, Binary/Ordinal for `author`  
  - **Numeric Scaling:** RobustScaler for word-count metrics  
- **Modeling:**  
  - Logistic Regression baseline achieving F2 score of 0.6935  
  - Resampling techniques like SMOTE and oversampling/undersampling pipelines  
- **Evaluation:** Emphasis on F2-score to prioritize recall (catching fake news) while balancing precision.
- **Insights:**  
  1. Fake news articles are slightly shorter than real ones  
  2. Top fake-news authors include James Smith and Christopher Johnson  
  3. Peak fake-news publishing occurred in November 2022 by outlets such as Daily News, NY Times, and CNN  
- **Future Work:**  
  - Use real-world news snippets instead of synthetic data  
  - Explore deep learning models with Keras/TensorFlow  
  - Incorporate word embeddings for deeper semantic analysis  
