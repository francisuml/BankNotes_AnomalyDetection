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


### Author

Francis Carl Sumile 
Machine Learning Practitioner | Data Scientist
GitHub: github.com/francisu.ml