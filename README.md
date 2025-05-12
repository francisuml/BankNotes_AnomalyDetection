# BankNotes_AnomalyDetection

## Objective
This analysis focuses on authenticating banknotes using machine learning techniques. The dataset contains features extracted from images of genuine and forged banknotes, with the goal of identifying patterns and anomalies that distinguish real from fake currency.

## Dataset
Data were extracted from images that were taken from genuine and forged banknote-like specimens. For digitization, an industrial camera usually used for print inspection was used. The final images have 400x 400 pixels. Due to the object lens and distance to the investigated object gray-scale pictures with a resolution of about 660 dpi were gained. Wavelet Transform tool were used to extract features from images.

The dataset consists of 1372 instances with 4 features and a binary class label (0 for genuine, 1 for forged):

Additional Information on this dataset
variance of Wavelet Transformed image (continuous)
skewness of Wavelet Transformed image (continuous)
curtosis of Wavelet Transformed image (continuous)
entropy of image (continuous)
class (integer)
You can download this dataset thru:
Banknote Authentication - UCI Machine Learning Repository

NOTE This dataset has no missing value

## Methodology

1. **Exploratory Data Analysis**
   - Feature distributions and correlations
   - Class imbalance analysis

2. **Feature Engineering**
   - Created interaction features:
     - Variance/Entropy ratio
     - Skewness-Kurtosis difference
     - Variance-Skewness product
   - Added distance-to-cluster features

3. **Model Development**
   - Isolation Forest with hyperparameter tuning
   - Local Outlier Factor (LOF)
   - One-Class SVM
   - Hybrid K-means + Isolation Forest approach
   - Ensemble of best performing models

4. **Evaluation**
   - Multiple metrics: Accuracy, Precision, Recall, F1, ROC AUC
   - Confusion matrices
   - Feature importance analysis

## Results

Our best performing model (ensemble approach) achieved:
- **F1-score**: 0.92
- **Accuracy**: 93.5%
- **Precision**: 91.2%
- **Recall**: 92.8%

Visualizations available in the notebook show clear separation between genuine and forged notes in the engineered feature space.


### Author

Francis Carl Sumile 
Machine Learning Practitioner | Data Scientist
GitHub: github.com/francisuml