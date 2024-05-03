# BT5153-GP06
This repository is for BT5153 Course Project Group 6

## Description
This project focuses on multi-label text classfication task, leveraging various natural lanuage processing techniques to predict LinkedIn skills based on profile texts.

## Features
- The data is sourced through LinkedIn's API, third-party API, and supplementary web scraping techniques. The dataset consists of 6,000 LinkedIn profiles, primarily from equity research analysts. Sample data is provided.
- Utilize traditonal NLP techniques and pre-trained model (RoBERTa).
- Evaluate model performance on various averaged F1-score.

## File List
- Data Preprocessing.ipynb: merge, clean, preprocessed raw data.
- Model 1.ipynb: RoBERTa based model.
- Model 2.ipynb: Utilize traditional NLP methods to preprocess text data and machine learning models to study their pattern. All text columns are treated as a single string. Two feature extraction techniques (Bag of Words, TF-IDF), three dimension reduction techniques (PCA, TruncatedSVD, set ```max_features```=300 in CounterVectorizer), and two ML models (RandomForest, LightGBM) are evaluated.
- Model 3.ipynb: DistilBERT Tokenizer and PCA with various ```n_estimator``` from 0.5 to 0.95, classifier models are RandomForest and LightGBM.
- Model 4.ipynb: Focuses on enhancing model performance through specialized embeddings and advanced ensemble methods. Key profile columns such as summary, education, and experience are individually processed using 'all-MiniLM-L6-v2' for targeted semantic extraction. The combined_text column undergoes feature extraction with TF-IDF, setting max_features to 300 and ngram_range to (1, 2). The model integrates MLSMOTE (with 200 synthetic samples and quantile limits for tail labels set between 0.05 and 1) to balance class distribution, and employs a combination of Random Forest and Stacking Classifier to leverage multiple predictive strengths.
