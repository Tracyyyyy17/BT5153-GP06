# BT5153-GP06
This repository is for BT5153 Course Project Group 6

## Description
This project focuses on multi-label text classfication task, leveraging various natural lanuage processing techniques to predict LinkedIn skills based on profile texts.

## Features
- The data is sourced through LinkedIn's API, third-party API, and supplementary web scraping techniques. The dataset consists of 6,000 LinkedIn profiles, primarily from equity research analysts. Sample data is provided.
- Utilize traditonal NLP techniques and pre-trained model (RoBERTa).
- Evaluate model performance on various averaged F1-score.

## File List
```please help modify file list description here ```

- Data Preprocessing.ipynb: merge, clean, preprocessed raw data.
- Model 1.ipynb: RoBERTa based model.
- Model 2.ipynb: All text as a single string.
- Model 3.ipynb: All text as a single string.
- Model 4.ipynb: Specific embedding on the summary, education and experience columns, with MLSMOTE for upsampling and using the resembling technique. 
